---
title: Modular Robotics With Swarm Intelligence

description: |
  MultiAgent RL based planner with swarm intelligance in a Modular robots setup.

people:
  - somnathsendhil
  - surabhitgupta
  - tharungowda
  - kritikabansal
  - niranthsai
  - lokeshkrishna

layout: project
image: "/img/swarm-robo/iota_intro_randomness.gif"
last-updated: 2019-08-15
---
Swarm Robotics is a very vast but less popular domain of robotics as the main challenges faced are increased State complexity of the system for an Agent to learn, and computational expense that exist in a classical planning algorithm. These problems are not something new but exist in a lot of places and are also solved to certain degrees seperately.

![iota BRoll](/img/swarm-robo/iota_broll.gif)

Coming to the computational cost of most classical algorithms are quite high as they exhaustively or atleast smartly search a big region of the State Space and Configuration Space, For our system this is very true as so many robot's state and configuration with respect to one another just makes the space increase exponentially making exhaustive search or similar methods really expensive. Some more classical work suggests approximations and iterative solutions, which falls short in assuraning in the optimal plan for a large test case. Other and quite popular methods are heuristic approachs that is which learns by itself they are the ones which learns about the environment and then smartly work in an online setup that is makes decision without having to exhaustively search all future state-tree. We decided to choose Reinforcement learning as one such heuristic algorithm to do planning in this modular bots setup.

The decision of choosing Reinforcement learning is not easy as this is still a MultiAgent system if each robot makes the decision for its own trajectory, this would classify this as MultiAgent Reinforcement learning problem which means there are its own set of problem to tackle. One being the computational expense ( which is lesser than classical algorithms for a MultiAgent system but is still considerable), and mainly world representation. The latter may sound silly but considering the policy is literaly the same for all the robots making the observation space the key point of decision for its policy in tackling the objective and in colaborating with other bots aswell. Representing the world is really a tough task and the solutions that are proposed in literature are really specific to there own problem statement, but one general concept is to use a shrunken or encoded world representation and extrapolating it using algorithms.

![Trial Run](/img/swarm-robo/Trial_run.gif)

The other problem that this system had was the State complexity which is also in the sync with the keypoint world representation. Hence we propose a solution of clustering the bots and having two planners one being a cluster level planner and the other bot level planner, by doing this we have a MultiAgent Reinforcement learning problem for the cluster level planner as there would be more than one cluster. By doing this we would have one representation for each cluster making it easier to represent a tentative policy for a localized group of robots (i.e., the ones inside the particular cluster). Then we see that while one policy solves one sub problem and the other solves another heirarchially superior problem in tandom to solve a central problem is nothing new and is known as heirarchial Reinforcement learning. But this again brings its own set of problems to the table hence our approach has comprised of simply mutating a given reward function to facilitate both the policie's learning.

![Cluster Wireframe](/img/swarm-robo/cluster_wireframe.png)
![Cluster Multishots](/img/swarm-robo/cluster_multishots.gif)

For implementation we chose to design our own modular robot platform as we felt most of the existing one had a very high state complexity or didnt have any design details for using them. Hence we designed a cost effective platform named 'iOTA' more details about the bot is given in the gym enviroment's github page itself. It basically contains simple catpillar tracks for its locomotion and two simple docking plates for docking two bots together.

Other smaller details of the projects are that we used a low level control( PD controller ) to follow the trajectory given by the low level trajectory planner (Potential Field Algorithm with cubic spline trajectory) with obstacle avoidance whose setpoint is given by the bot level planner policy by choosing a optimal point on a constellation(this is a shape like star, square, circle etc.) where the constellation and its parameter (like size and soon) is given by the Cluster level planner which gives the optimal constellation that the cluster must form into.

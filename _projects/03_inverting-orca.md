---
title: "I-ORCA: Implicitly Nudging Human Trajectories"
excerpt: "In this project, we look at the inverse of the social navigation problem. Social Navigation deals with generating trajectories for mobile robots that minimally invade human trajectories. <br/><img src='/images/I-ORCA-example.gif'> <br/>We try to see if we can leverage the obstacle avoidance nature of humans to generate trajectories for robots that minimally nudge the humans toward desired directions..."
collection: projects
---

# I-ORCA: Implicitly Nudging Human Trajectories

<img src='/images/I-ORCA-example.gif'>

In this project, we want to answer the question - "How can we design trajectories for mobile robots that optimally nudge some human around them in desired directions while minimally affecting other humans in the surroundings?". We try to invert the popular Optimal Reciprocal Collision Avoidance [(ORCA)](https://gamma.cs.unc.edu/ORCA/) algorithm to achieve this. The figure below represents the I-ORCA algorithm geometrically. It uses the Reciproval Velocity Obstacles (RVOs) for 2D circular agents to geometrically compute velocities for the robot that nudge the human in the desired direction by leveraging their collision avoidance behavior.

<img src = '/images/i-orca-geometrically.png'>

We developed a 2-D multi-agent simulation environment using the [Farama Gymnasium](https://gymnasium.farama.org/) (formerly OpenAI Gym) framework that shows the top-view of the agents. 

Through simulations, we compute the "nudge efficiency" metric, which showed that the best way to nudge an agent in a desired direction is to "lead" them towards that direction. The figure below shows this nudge efficiency metric around the target agent. 

<img src = '/images/nudge-efficiency.png>

Below are the formal definitions of the algorithms we developed.

<img src = '/images/i-orca-algs.png'>

All work was done during my summer internship at the [Honda Research Institute](https://usa.honda-ri.com/) in 2025.

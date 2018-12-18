### Algorithm
We implemented a DQN as proposed by [Mnih, Kavukcuoglu, Silver, et. al.](http://www.nature.com/articles/nature14236). Our implementation makes use of their two famous key concepts that make convergence during training feasible:
 - Experience Replay to reduce correlation in observation sequences
 - Fixed Q-Target to reduce correlation with the target Q-Network (we used a soft q-target update)
 
### Learning Curve

Score plot of our best attempt: An agent that solved the environment in 177 episodes.

![scores](images/scores.png)

The score (cumulated reward per episode) is increasing over time - the agent learns to play.

### Hyperparameters
We took a rather heuristic approach for finding the right configuration of our agent. The main ingredients of our model are:

 - Neural network: We tested several configurations, starting from only 1 hidden layer up to 3 hidden layers, with number of hidden units ranging from 32 to 64 (always with a ReLu activation). Two hidden layers with 32 units worked best.
  - Learning rate: Choosing an aggressive learning rate of 0.96 was the most relevant parameter for reducing the number of episodes needed to solve the game.

### Improvements / Ideas for Future Work
Further improvements could be:
 - Try other DQN approaches (Double DQN, Dueling Networks, Rainbow) or some Policy Gradient Method
 - Try learning from Pixels 
 - Do a more systematic hyperparameter search/tuning

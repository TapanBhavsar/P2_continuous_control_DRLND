DDPG(Deep Deterministic policy gradient) is policy-gradient actor-critic algorithm which is off policy and model free method. In this method One can create neural network for actor and critic both.

The achitecture for both as structured below:

Actor NN achitecute:

***Input state(33) -> hidden_1 (400) -> hidden_2 (300) -> output_action (4)***

Critic NN architecture:

***Input state (33) -> concat_with_action (400+4) -> hidden (300) -> output_action (4)***

The hyperparameters:

  * Buffer size: 100,000
  * Batch size: 128
  * Actor nn learning rate: 0.001
  * Critic nn learning rate: 0.001
  * discount factor: 0.99
  * weight decay: 0
  * tau: 0.001

![alt text](plot.png)

The NAF algorithm allows training in continuous state and action space environments, adding a great deal of versatility in terms of possible applications. Reinforcement learning algorithms for continuous environments
such as NAF are commonly used in the field of control, especially in robotics, because they are able to train in environments that more closely represent reality.

![image](https://github.com/AkshayKulkarni3467/NAF_DQN/assets/129979542/4449b4ed-4b61-41e5-b37e-d5730683fc87)

Since Q returns the benefit of taking a certain action in a state, while V returns the benefit of being in a state, the difference of both returns information about how advantageous it is to take a certain action
in a state with respect to the rest of actions, or the extra reward that the agent will receive by taking that action with respect to the rest of actions.

![image](https://github.com/AkshayKulkarni3467/NAF_DQN/assets/129979542/9d864ae6-ae54-4823-8e1e-3b5663e860c2)

The NAF algorithm makes use of a neural network that obtains as separate outputs a value for the State-Value Function V and for the Advantage Function A. The neural network obtains these outputs since, as 
previously explained, the result of the Action-Value Function Q can be later obtained as the sum of V and A.

![image](https://github.com/AkshayKulkarni3467/NAF_DQN/assets/129979542/8f7cb449-bc0b-4f02-a3ba-a78feb42fc16)

By looking at the different components that make up the Q-Function, it can be seen that the neural network will have three different outputs: one to estimate the Value Function, another to obtain the action that 
maximizes the Q-Function (argmax Q(s, a) or 𝜇(x|𝜃)), and another to calculate the matrix P.


Here, the NAF algorithm is used to solve the lunar-lander-contineous environment in openai-gym.

The returns and loss after 22k steps are:

![nafdqn_return](https://github.com/AkshayKulkarni3467/NAF_DQN/assets/129979542/cc4416e2-09bd-4174-844a-fb9af046b5e6)


![nafdqn_loss](https://github.com/AkshayKulkarni3467/NAF_DQN/assets/129979542/8531f894-1a91-4d7e-983b-d66d0a6e2229)

Lunar-Lander after 1000 iterations:


https://github.com/AkshayKulkarni3467/NAF_DQN/assets/129979542/c1c2ed9e-e46e-4590-a964-ba6e1d24df9

Lunar-Lander after 20000 iterations:


https://github.com/AkshayKulkarni3467/NAF_DQN/assets/129979542/5714092d-8fcb-4063-a3a9-20ea40f630d0




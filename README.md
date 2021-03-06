# RL gym

Implementing different reinforcement learning algorithms on different gym environments. 

These algorithms are implemented in this repo:

* [A2C](#A2C)
* [DDPG](#DDPG)
* [Double DQN](#Double_DQN)
* [Dueling DQN](#Dueling_DQN)
* [TD3](#TD3)

And tested on these environments.

| <div align="center"><img src="assets/CP-final_reinforce.gif" /></div> | <div align="center"><img src="assets/Pend_final_DDPG.gif"  /></div> | <div align='center'><img src="assets/AB-final_A2C.gif" /></div> | <div align="center"><img src="assets/LLC-final_DDPG.gif"  /></div> |
| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| <div align="center">**Cartpole**</div>                       | <div align="center">**Pendulum**</div>                       | <div align="center">**Acrobat**</div>                        | <div align="center">**Lunar Lander Continuous**</div>        |

## A2C

**A2C** is a on-policy, model-free reinforcement learning algorithm. Here is the pseudo code for **A3C** which is almost similar to **A2C**.

<div align="center"><img src="assets/A2C.jpg" width="80%"/></div>

<table align='center'>
  <tr>
    <tb><div align="center"><img src="assets/AB-final_A2C.gif"/></div></tb>
  </tr>
   <tr>
       <tb><div align="center">Agent trained using A2C playing Acrobat game.</div></tb>
  </tr>
</table>



## DDPG

**DDPG** is a off-policy, model-free reinforcement learning algorithm. Here is the pseudo code for **DDPG**

<div align="center"><img src="assets/DDPG.jpg" width="80%"/></div>

<br>

<table align='center'>
  <tr>
    <tb><div align="center"><img src="assets/LLC-final_DDPG.gif"/></div></tb>
  </tr>
  <tr>
       <tb><div align="center">Agent trained using DDPG playing lunar lander game.</div></tb>
  </tr>
</table>


## Double_DQN

**Double DQN** is a off-policy, model-free reinforcement learning algorithm. Here is the pseudo code for **Double DQN**

<div align="center"><img src="assets/Double_DQN.jpg" width="80%"/></div>

<table align='center'>
  <tr>
    <tb><div align="center"><img src="assets/CP-final_DDQN.gif"/></div></tb>
  </tr>
   <tr>
       <tb><div align="center">Agent trained using Double DQN playing Cartpole game.</div></tb>
  </tr>
</table>

## Dueling_DQN

Similar to DDQN, dueling network contains two separate estimators: one for the state value function and one for the state-dependent action advantage function. 

Formula for the decomposition of Q-value:

<div align="center"><img src="assets/Duel_DQN.jpg"/></div>

-  **θ** is shared parameter for the network.
- **α** parameterizes output stream for advantage function **Α**.
- **β** parameterizes output stream for value function **V**.

<table align='center'>
  <tr>
    <tb><div align="center"><img src="assets/AB-final.gif" /></div></tb>
  </tr>
   <tr>
       <tb><div align="center">Agent trained using Dueling DQN playing Acrobat game.</div></tb>
  </tr>
</table>

## TD3

**TD3** is a off-policy, model-free reinforcement learning algorithm. Here is the pseudo code for **TD3**

<div align="center"><img src="assets/TD3.jpg" width="80%"/></div>

<br>

<table align='center'>
  <tr>
    <tb><div align="center"><img src="assets/Pend-final_TD3.gif"  /></div></tb>
  </tr>
   <tr>
       <tb><div align="center">Agent trained using TD3 playing Pendulum game.</div></tb>
  </tr>
</table>

## References

* [Reinforcement Learning - Goal Oriented Intelligence](https://www.youtube.com/playlist?list=PLZbbT5o_s2xoWNVdDudn51XM8lOuZ_Njv)
* [Reinforcement Learning by Sentdex](https://www.youtube.com/playlist?list=PLQVvvaa0QuDezJFIOU5wDdfy4e9vdnx-7)
* [OpenAI's Spinning Up Docs](https://spinningup.openai.com/)
* [Wang et al., Dueling Network Architectures for Deep Reinforcement Learning](https://arxiv.org/pdf/1511.06581.pdf)
* [Dueling Deep Q Networks](https://towardsdatascience.com/dueling-deep-q-networks-81ffab672751)
* [Deriving Policy Gradients and Implementing REINFORCE](https://medium.com/@thechrisyoon/deriving-policy-gradients-and-implementing-reinforce-f887949bd63)
* [Understanding Actor Critic Methods and A2C](https://towardsdatascience.com/understanding-actor-critic-methods-931b97b6df3f)
* [Keras DDPG Example](https://keras.io/examples/rl/ddpg_pendulum/)

<div align="center"><small><a href="https://github.com/vstark21">&copy V I S H W A S</a></small></div>
# Hindsight Experience Replay (HER)

This repository contains a tensorflow HER implementation and a bit flipping environment as described in [OpenAI's paper](https://arxiv.org/pdf/1707.01495.pdf)

The implementation includes :
1.  A DQN and a DDQN agent (which also works on other traditional [gym](https://gym.openai.com/) environments)
2.  A bit flipping environment
3.  Pre-trained models for 30-bits and 40-bits flipping environments

## Customize
Check the "Training" cell to adjust training parameters and enable/disable HER.

## TODO
- [ ] Optimize the way to concatenate transitions
- [ ] Parallelize training
- [x] Train on bit length > 30
- [ ] Implement DDPG

# Hindsight Experience Replay (HER)

This repository contains a tensorflow HER implementation and a bit flipping environment as described in [OpenAI's paper](https://arxiv.org/pdf/1707.01495.pdf)

The implementation includes :

1. In `Hindsight Experience Replay.ipynb` :
    1.  A DQN and a DDQN agent (which also work on other traditional [gym](https://gym.openai.com/) environments)
    2.  A bit flipping environment
    3.  Pre-trained models for 30-bits, 40-bits and 50-bits flipping environments
2. In `ChaseEnv.ipynb` :
    1. A DDPG agent
    2. A `ChaseEnv` environment, where a chaser is initialized at a random position in
       a 2d plane and has to reach a goal in another random position within a certain threshold.

## Benchmarks

*  100% success rate for 30 and 40-bits environments
*  95% success rate for 50-bits environment (average on 100 tests)
*  90% success rate for size=5 ChaseEnv (average on 100 tests)

## Customize
Check the "Training" cell to adjust training parameters and enable/disable HER.

## TODO
- [x] Optimize the way to concatenate transitions
- [ ] Parallelize training
- [x] Train on bit length > 30
- [x] Implement DDPG

# Retrace-Algorithm-in-Reinforcement-Learning

Safe and efficient off-policy reinforcement learning

Author: ​Remi Munos, Thomas Stepleton, Anna Harutyunyan, Marc G. Bellemare
Year: 2016 
In this paper, they have showed that learning from returns need not be at cross-purposes with off-policy learning.

Naive off-policy policy evaluation, without correcting for the “off-policyness” of a trajectory, still converges
to the desired Q(pi) value function provided the behavior and target policies are not too far apart
difficult to uphold in the control case, where the target policy is greedy with respect to the current
Q-function.
Tree-backup (TB(lambda)) algorithm (Precup et al., 2000) tolerates arbitrary target/behavior discrepancies
by scaling information (here called traces) from future temporal differences by the product of target policy
probabilities.
It is not efficient because as traces may be cut prematurely, blocking learning from full returns.
Retrace(lambda), which is both safe and efficient, enjoying convergence guarantees for off-policy policy
evaluation and – more importantly – for the control setting.
Retrace(lambda) can learn from full returns retrieved from past policy data.
Two related off-policy learning problems. In the policy evaluation setting, we are given a fixed policy whose
value Q we wish to estimate from sample trajectories drawn from a behaviour policy. In the control setting,
we consider a sequence of policies that depend on our own sequence of Q-functions (such as "-greedy
policies), and seek to approximate Q.

Research Paper: [Safe and Efficient Off-Policy Reinforcement Learning](https://arxiv.org/abs/1606.02647)


---
layout: post
title:  "Dissecting Reinforcement Learning-Part.4"
date:   2017-01-29 07:00:00 +0000
description: This blog series explains the main ideas and techniques used in reinforcement learning. In this post Actor-Criti models. It includes complete Python code.
author: Massimiliano Patacchiola
comments: false
published: false
---

Here you are, the fourth episode of the "Dissecting Reinforcement Learning" series. In this post I will introduce the last group of techniques used in reinforcement learning: **Actor-Critic (AC) methods**. I often define Actor-Critic as a **meta-technique** which uses the methods introduced in the previous posts in order to learn. 

Policy-gradient-based actor-critic algorithms are among the most popular algorithms in the reinforcement learning framework. For example, the [Deep Determinist Policy Gradient](https://arxiv.org/abs/1509.02971) algorithm (DDPG) introduced recently by some researchers of Google DeepMind is an actor-critic, model-free algorithm. The AC approach has many links with neuroscience and animal learning, in particular with models of basal ganglia. Nevertheless AC methods are not described 


[Numerous models have addressed the basal ganglia's role in learning, based on the uncanny resemblance of dopaminergic cell firing to the requirements of an error signal in temporal difference (TD) learning. Such models map the Actor-Critic implementation of TD learning on to the basal ganglia (Barto, 1995; Houk, Adams & Barto, 1995; Montague, Dayan & Sejnowski, 1996; Schultz, Dayan & Montague, 1997), where, roughly, the Actor is mapped on to the selection function of the basal ganglia, and the Critic is mapped on to the RL circuit in Figure 2. As such the dopamine signal is envisaged as the teaching signal that alters the Actor's responses to maximise future reward.
Joel, Niv and Ruppin (2002) evaluated both anatomical and computational perspectives of Actor-Critic models. They review several models and conclude that they are not compatible with current anatomical data.
Though computationally elegant in approach, critics of these models have variously argued for its biological implausibility, citing:
- dopamine cells increase firing to aversive, neutral, and rewarding stimuli, and thus cannot uniquely signal reward prediction error (Pennartz, 1996, however, see Ungless et al. 2004 for claims that the neurons responding to aversive stimuli are, in fact, not dopaminergic)
- dopamine cells fire before the stimulus can be fully perceived, and thus its value cannot be known at the time (Redgrave, Gurney & Prescott, 1999b)
- stimulus-reward learning can take place in the absence of dopamine, and thus it is not necessary for learning (Berridge, 2007)]


Actor-Critic methods (and monkeys)
-----------------------------------



Conclusions
-----------


Index
------

1. [[First Post]]((https://mpatacchiola.github.io/blog/2016/12/09/dissecting-reinforcement-learning.html)) Markov Decision Process, Bellman Equation, Value iteration and Policy Iteration algorithms.
2. [[Second Post]](https://mpatacchiola.github.io/blog/2017/01/15/dissecting-reinforcement-learning-2.html) Monte Carlo Intuition, Monte Carlo methods, Prediction and Control, Generalised Policy Iteration, Q-function. 
3. [[Third Post]](https://mpatacchiola.github.io/blog/2017/01/29/dissecting-reinforcement-learning-3.html) Temporal Differencing intuition, Animal Learning, TD(0), TD(λ) and Eligibility Traces, SARSA, Q-learning.

Resources
----------

- The **complete code** for MC prediction and MC control is available on the [dissecting-reinforcement-learning](https://github.com/mpatacchiola/dissecting-reinforcement-learning) official repository on GitHub.

- Dadid Silver's course (DeepMind) in particular **lesson 4** [[pdf]](http://www0.cs.ucl.ac.uk/staff/d.silver/web/Teaching_files/MC-TD.pdf)[[video]](https://www.youtube.com/watch?v=PnHCvfgC_ZA&t=438s) and **lesson 5** [[pdf]](http://www0.cs.ucl.ac.uk/staff/d.silver/web/Teaching_files/control.pdf)[[video]](https://www.youtube.com/watch?v=0g4j2k_Ggc4&t=2s)

- **Christopher Watkins** doctoral dissertation, which introduced the **Q-learning** for the first time [[pdf]](https://www.researchgate.net/profile/Christopher_Watkins2/publication/33784417_Learning_From_Delayed_Rewards/links/53fe12e10cf21edafd142e03/Learning-From-Delayed-Rewards.pdf)

- **Machine Learning** Mitchell T. (1997) [[web]](http://www.cs.cmu.edu/~tom/mlbook.html)

- **Artificial intelligence: a modern approach. (chapters 17 and 21)** Russell, S. J., Norvig, P., Canny, J. F., Malik, J. M., & Edwards, D. D. (2003). Upper Saddle River: Prentice hall. [[web]](http://aima.cs.berkeley.edu/) [[github]](https://github.com/aimacode)

- **Reinforcement learning: An introduction.** Sutton, R. S., & Barto, A. G. (1998). Cambridge: MIT press. [[html]](https://webdocs.cs.ualberta.ca/~sutton/book/ebook/the-book.html)

- **Reinforcement learning: An introduction (second edition).** Sutton, R. S., & Barto, A. G. (in progress). [[pdf]](https://webdocs.cs.ualberta.ca/~sutton/book/bookdraft2016sep.pdf)



References
------------


Joel, D., Niv, Y., & Ruppin, E. (2002). Actor–critic models of the basal ganglia: New anatomical and computational perspectives. Neural networks, 15(4), 535-547.


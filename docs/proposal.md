---
layout: default
title: proposal
---

## Summary of the project
Quantum computers are machines that use quantum phenomena such as superposition and entanglement to perform computation. They are believed to solve certain problems substantially faster than classical computers. The most famous quantum algorithm is Shor’s factoring algorithm which has exponential speed-up over any existing classical algorithm [1].

For our project, we will implement a quantum variant of Markov Decision Process (MDP)-based Reinforcement Learning (RL), or Quantum Reinforcement Learning (QRL). We will implement the algorithm in Qiskit, a Python-based language for IBM superconducting qubits. Although Qiskit already has a collection of quantum machine learning (QML) methods, including Quantum Generative Adversarial Network (qGAN), Quantum Neural Network (QNN), Quantum Support Vector Machine (QSVM), and so on, there haven’t been modules for QRL. Our project thus fills this gap.

Specifically, we will review the QRL models proposed so far, pick the most promising one (or a combination of them), and code them into Qiskit. In [2] the authors are able to derive a QRL algorithm that takes advantage of Grover’s amplitude amplification [3]. Some more advanced models take advantage of the quantum processing capability of the agent [4] or the possibility to probe the environment in superpositions [5]. In addition, we can improve the models by using well-known algorithmic primitives like Quantum Random Access Memory (QRAM) [6] or Quantum Singular Value Transform (QSVT) [7].

## AI/ML Algorithms
MDP-based Quantum Reinforcement Learning

## Evaluation Plan
We will write a series of unit tests and integration tests to verify the correctness of the algorithm. The number of unit tests should ideally be at least as many as the functions we have, and the number of integration tasks should be equal to the number of integrated tasks we need to perform. We will also feed the algorithm on small tasks to real quantum devices (such as IBM-Melbourne) and record the fidelity of the outputs. We can then examine how quantum noises, including error per gate, decoherence, qubit relaxation, and so on, affect the performance of the algorithm.

For the sanity case, we can benchmark the model against a classical RL algorithm on a practical task such as maze-solver, and compare them in terms of two metrics: the speed and the performance (sum of discounted rewards). We will simulate the quantum algorithm through parallel processing and record the overall time. In principle, the number of processers needed grows exponentially to the number of qubits, but since our task is small it's durable by a classical computer.

## Citations
[1] P. W. Shor, SIAM Journal on Computing 26, 1095-7111 (1997) \
[2] D. Dong, et al, IEEE Transactions on Systems, Man, and Cybernetics, Part B (Cybernetics), 1207–1220 (2008) \
[3] L. K. Grover, 28th Annual ACM Symposium on the Theory of Computing, 212 (1996) \
[4] G. D. Paparo, et al, Physical Review X. 4 (2014) \
[5] V. Dunjko, et al, Physical Review Letters, 117 (2016) \
[6] G. Vittorio, et al, Physical Review Letters, 1079-7114 (2007) \
[7] A. Gilyén, Proceedings of the 51st Annual ACM SIGACT Symposium on Theory of Computing (2019)

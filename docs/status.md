---
layout: default
title: status
---

## Project Summary
Quantum computers are machines that use quantum phenomena such as superposition and entanglement to perform computation. They are believed to solve certain problems substantially faster than classical computers. The most famous quantum algorithm is Shor’s factoring algorithm which has exponential speed-up over any existing classical algorithm [1].

For our project, we will implement a quantum variant of Reinforcement Learning (RL), which employs the Parametrized/Variational Quantum Circuits (PQCs or VQCs). In contrast to most quantum algorithms that require fault-tolerant large-scale quantum computers, this algorithm employs small and low-depth circuits and is flexible under noises, thus it is believed to be useful already on near-term quantum computers. While Google already had a full implementation of the algorithm in tensorflow using Cirq [2], the other widely used quantum programming language Qiskit from IBM hasn’t. Therefore, we would like to fill this gap and have a working PQC-based QRL algorithm in Qiskit.

While the most promising direction is to run the algorithm implemented in Qiskit on real IBM quantum devices, investigate the effects of quantum noises, and demonstrate quantum advantage, it is not realistic due to several reasons: 1. The PQC-based QRL requires thousands of circuit re-runs, which IBM devices disallow. 2. There are many layers of classical processing on IBM’s side, which would be very slow and hinder the accurate benchmark of speed. 3. The circuit requests are usually queued, and there is no guarantee when our requests will be finished (sometimes takes months). Therefore, our work will be a proof of concept, where we use classical simulations of quantum circuits to demonstrate this algorithm works. 

## Approach

![image](https://user-images.githubusercontent.com/31495624/142090910-1eea063b-cda0-44aa-a4fd-59252fa381f4.png)

![image](https://user-images.githubusercontent.com/31495624/142090880-37d8fc91-dcd4-434b-b2f3-2f04293f503f.png)

![image](https://user-images.githubusercontent.com/31495624/142091522-7133f584-8b47-4ddc-bbd4-098e4287f90d.png)

![image](https://user-images.githubusercontent.com/31495624/142091840-f2ecfb57-ff1a-4277-a909-6e1efd13aab7.png)

<img width="500" alt="1637118928(1)" src="https://user-images.githubusercontent.com/31495624/142129427-1fe6b77c-1388-4279-8c67-160a1cf99b6d.png">

![image](https://user-images.githubusercontent.com/31495624/142129465-3afa6c50-7b32-4a8d-a27d-8bc02e25d9ad.png)

![image](https://user-images.githubusercontent.com/31495624/142129372-c1113da3-f4ae-4334-8923-811888f9888f.png)

<img width="621" alt="1637119800(1)" src="https://user-images.githubusercontent.com/31495624/142129586-68deee56-f5dc-4bb3-8691-0657c838caa5.png">

## Evaluation

![3291d6b8-2636-4b27-aff7-048633c172e1](https://user-images.githubusercontent.com/31495624/142091337-b081bc49-ab30-4fa5-8923-3b1a465206e4.png)

![image](https://user-images.githubusercontent.com/31495624/142092049-e78b4376-d81e-4987-9341-b0c651d3112d.png)

## Remaining Goals and Challenges

## Resources Used

[//]: <> (Wed Feb 17 23:24:04 EST 2021)

# Homework 3

### Author: [Simon Chu](http://simonchu.org)

### Paper: [Dynamic Adaptation of Software-defined Networks for IoT Systems: A Search-based Approach](https://arxiv.org/pdf/1905.12763)

# Description of the Problem, Gap and Hook

## Problems

With the proliferation of IoT devices that all rely on communication networks, the networks are subject to congestion when network traffic increases, such as when an emergency is unfolding. This can cause serious problems and consequences for safety-critical systems like emergency management systems (EMS). Therefore, the author claims that communication systems should be able to adapt to changes in the (network) environment and maintain reasonable service quality, and this is a challenge that can be tackled by reconfiguring the system.

## Gap

None of the research in software-defined networks (SDN) optimize the configuration for multiple quality of service criteria simultaneously.

None of the research in optimizing configuration for multiple criteria addressed the online (dynamic-reconfiguring) SDN, instead, most of them addressed offline, and in the domain of system design or architecture.

## Hook

The proposed method fills in the gap by enabling resolving the congestion of SDN in an online manner on multiple criteria, while minimizing data transmission delays and reconfiguration costs.

# Research Questions

- RQ1 (efficiency and effectiveness): Can their approach resolve congestion caused by changes in network requests over time?

- RQ2 (scalability): Can our approach resolve congestion promptly for large-scale networks?

- RQ3 (comparison with baselines): How does our approach perform compared with baseline approaches?

# Overview of Study Design and Methods

The study uses quasi-experiments to perform the study on two classes of subjects, a group of synthetic networks, and emergency management systems (EMS) -- a large-scale industry system.

The group of synthetic networks is used to evaluate RQ1 and RQ2 on the efficiency, effectiveness, and scalability of the SDN algorithm by adjusting the network request, network size, and whether it can computing and apply a reconfiguration promptly.

An industry large-scale EMS is used to evaluate RQ3 on the scalability of the system, by using corresponding metrics to compare the new algorithm with the baseline configuration and measure the extent to which the EMS is affected when a disaster near the mobile communication facility with both the new and regular SDN system deployed.

# Critique of All of Above

## Description of the Problem, Gap and Hook
- The author's description makes it sound like reconfiguring the network is the only way to ensure the reliability of the network. Are there alternative options in tackling the congestion problems (maybe by deploying new network congestion algorithms, upgrade the network infrastructure for safety-critical systems, etc), and what makes the adaptive configuration superior to alternative approaches? Is it cost-effective to deploy the new approach rather than alternative methods?

## Research Questions

- RQ1: What does it mean for the approach to "resolve congestion", what level of "changes in network request" is necessary, and how long specifically is "overtime"?

- RQ2: again, what does it mean to "resolve congestions", and what kind of systems are considered "large-scale"?

- RQ3: What is the "baseline approach"? Is the baseline approach specific to each safety-critical system being evaluated, or is it consistent across the board?

## Study Design and Methods

- The quasi-experiment did not establish a cause and effect relationship for the reconfigurability of the system and the system performance, since not all independent variables are strictly controlled.

- The lack of realistic experiments. The author has only tested the new SDN algorithm on one particular EMS during an occurrence of a real disaster. Although EMS is a safety-critical system, it is not representative of the space of the safety-critical systems space, thus the positive outcome in EMS may be weak in claiming that the algorithm can work well in all safety-critical systems.


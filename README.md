Paper Title : Elastic Workload Balancing over the 6G Collaborative Continuum: A Distributed Agent-Based Control Framework"


**ABSTRACT** The sixth generation (6G) of mobile networks is expected to operate as a connected and collaborative Internet of Things (IoT)-Edge-Cloud continuum, in which communication, computing, and control are jointly orchestrated to serve time-critical and energy-sensitive applications. A central problem in this paradigm is workload placement, namely dynamically deciding where each computational task is executed across heterogeneous and multi-domain compute nodes. Centralized schedulers and reactive heuristics scale poorly and cannot anticipate how the continuum evolves between the decision and its execution. This article presents a distributed control framework for elastic workload balancing over the 6G continuum based on Deep Reinforcement Learning (DRL). We introduce a reference architecture in which a clustered Resource Telemetry Orchestration scheme shares continuum-wide state through a publish-subscribe model, while each edge computational node hosts an autonomous Intelligent Controller. The controller couples short-horizon load forecasting with a DRL policy to make proactive migration decisions that jointly optimize latency, energy, and reliability through a single tunable cost function. Performance evaluation demonstrates that the proposed distributed scheme enables more efficient workload orchestration than conventional baseline approaches with respect to key system metrics, reducing workload drops under intermediate to heavy traffic conditions, while proactively balancing the load across the continuum.


How to use :

In order to run the default version one just needs to run the command 
```
python main.py
```

This will create a new run and will store it in a folder called *log_folder*. If ones wants to change the default values for the simulations, they need to tun the hyperparameters script, with the appropriated command line arguments, as shown below

```
python hyperparameters --number_of_servers 10 
```
After that they need to rerun the main script.

Note that one must rename the folder, or else the weights of the previous run will be loaded.

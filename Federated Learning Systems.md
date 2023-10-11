## **1. 概述**

![[Pasted image 20231011110350.png]]

> The main research directions (also the main challenge) of FL are to improve the effectiveness, efficiency, and privacy, which are also three important metrics to evaluate an FLS.

[[A Survey on Federated Learning Systems.pdf#page=11&selection=39,7,40,82|A Survey on Federated Learning Systems, page 11]]

## **2.开源项目**
![[Pasted image 20231011111001.png]]

Federated AI Technology Enabler (FATE)
https://github.com/FederatedAI/FATE
>  FATE is a powerful and easy-to-use FLS. Users can simply set the parameters to run a FL algorithm. Moreover, FATE provides detailed documents on its deployment and usage. However, since FATE provides algorithm-level interfaces, practitioners have to modify the source code of FATE to implement their own federated algorithms

[[A Survey on Federated Learning Systems.pdf#page=21&selection=57,21,60,40|A Survey on Federated Learning Systems, page 21]]

Google TensorFlow Federated (TFF)
https://github.com/tensorflow/federated
> TFF is a lightweight system for developers to design and implement new FL algorithms. Currently, TFF does not consider consider any adversaries during FL training. It does not provide privacy mechanisms. TFF can only deploy on a single machine now, where the federated setting is implemented by simulation.

[[A Survey on Federated Learning Systems.pdf#page=21&selection=79,24,82,29|A Survey on Federated Learning Systems, page 21]]

OpenMined PySyft
https://github.com/OpenMined/PySyft
> PySyft provides multiple optional privacy mechanisms including secure multi-party computation and differential privacy. Thus, it can support running on honest-but-curious parties. Moreover, it can be deployed on a single machine or multiple machines, where the communication between different clients is through the websocket API [168 ]. However, while PySyft provides a set of tutorials, there is no detailed document on its interfaces and system architecture.

[[A Survey on Federated Learning Systems.pdf#page=22&selection=55,16,62,60|A Survey on Federated Learning Systems, page 22]]

Baidu PaddleFL
https://github.com/PaddlePaddle/PaddleFL
>  The system structure of PaddleFL is shown in Figure 6. In the compile time, there are four components including FL strategies, user defined models and algorithms, distributed training configuration, and FL job generator. The FL strategies include the horizontal FL algorithms such as FedAvg. Vertical FL algorithms will be integrated in the future. 

[[A Survey on Federated Learning Systems.pdf#page=22&selection=73,30,76,68|A Survey on Federated Learning Systems, page 22]]


FedML
https://github.com/FedML-AI/FedML
> FedML supports three computing paradigms, namely standalone simulation, distributed computing and on-device training, which provides a simulation environment for a broad spectrum of hardware requirements. Reference implementations for all supported FL algorithms are provided. Although there are still gaps between some of the experiment results and the optimal results, they provide useful information for further development.

[[A Survey on Federated Learning Systems.pdf#page=23&selection=50,87,54,107|A Survey on Federated Learning Systems, page 23]]

![[Pasted image 20231011120217.png]]

## **3.系统设计**

![[Pasted image 20231011120322.png]]
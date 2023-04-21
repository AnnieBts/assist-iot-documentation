.. _DLT-based FL enabler:

############
DLT-based FL enabler
############

.. contents::
  :local:
  :depth: 1

***************
Introduction
***************
The FL-DLT enabler is a system that provides a secure reputation mechanism for all local operators in a federated learning (FL) system. The reputation mechanism serves as a safeguard against free-riders and malicious adversaries, ensuring that only reputable local operators can contribute to the global model.
 

***************
Features
***************
 The integration of the DLT enabler with the FL baseline system involves the calculation of reputation scores for each FL local operator instance, which is stored on a permissioned blockchain network that allows only authorized users to access the scores and participate in the consensus algorithm that updates them. The final reputation score for each local operator is calculated using the cosine similarity between the weights of FL local operations and the aggregated weight. The FL training collector queries the reputation scores and reputation set to decide on penalties or incentives for the FL local operations. 

The FL-DLT enabler consists of three components: the DLT communicator, the reputation score calculator, and the DLT storage. The DLT communicator is a RESTful API that receives weights from the training collector and fetches reputation scores and reputation sets from the DLT storage. The reputation score calculator applies the reputation mechanism and calculates scores for each local operator in each training round. The DLT storage component stores the reputation scores and the reputation set to the Distributed Ledger.


*********************
Place in architecture
*********************
The DLT-based FL enabler is part of the vertical plane DLT enablers.

***************
User guide
***************
The user guide will be determined after the release of the enabler.


***************
Prerequisites
***************
Hyperledger Fabric 2.2, Hyperledger Fabric CA 1.4

***************
Installation
***************
The installation procedure is under development.

*********************
Configuration options
*********************
The enabler is prepared to run in a K8S environment. The creation is prepared to be autonomous in such a working environment.
The service consumer will be required to communicate with the server using the described Rest interface.

***************
Developer guide
***************
The  DLT-based FL  enabler is build using  Hyperledger Fabric Framework. Smart contracts are written in Go.

***************************
Version control and release
***************************
Gitlab will be used as a version control and release tool.

***************
License
***************
Will be determined after the release of the enabler.

********************
Notice(dependencies)
********************
Dependency list and licensing information will be provided

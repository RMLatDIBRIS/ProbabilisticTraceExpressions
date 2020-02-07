# ProbabilisticTraceExpressions

Probabilistic Trace Expressions (PTEs) are an extension of Trace Expressions (TEs) where the types of events that can take place in a state are associated with a probability. 

TEs are a powerful formalism suitable to model languages that are more than context-free. 

They have been adopted to model and dynamically verify  behavioural patterns involving interaction with the environment in remote patient monitoring domains, IoT systems, programs developed in Node.js and Node-RED. 

PTEs have proven useful for verifying that agents in a Multiagent System (MAS) interact in compliance with an Agent Interaction Protocol (AIP) modelled as a PTE, even when gaps are observed (namely, even when the monitor associated with the agent realises that an interaction took place in the MAS, but it was not correctly observed). 

We have explored the connection between PTEs and Hidden Markov Models (HMM). This opens up the possibility to learn HMMs from observed interactions using existing algorithms, translate the learned HMM into a PTE, and use the PTE as a protocol specifications.

Also, thanks to TE built-in operators suitable for checking that two different PTEs can perform the same transitions, and to algorithms for transforming Linear time Temporal Logic (LTL) properties into PTEs, verifying that a LTL property is met by an AIP represented by a PTE can be addressed in an elegant and natural way.

Besides theoretical results, we have developed centralised and decentralised implemented algorithms to dynamically verify the behaviour of the MAS under scrutiny. The code is available, as it is, in this repository. According to our experiments, the decentralised approach is more efficient and scalable than the centralised one. 

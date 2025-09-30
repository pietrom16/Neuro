# Project presentation: *Neuro* 4

Author: Pietro Mele <pietrom16@gmail.com>

Copyright (C) 2019-2025 Pietro Mele

### Abstract

Ongoing personal project to develop a flexible system integrating different approaches to 
solve a generic problem, having the nervous system as an inspiration. The system 
is iterative, dynamically partitioning the input space-time, and assigning each partition to a 
specific module (*Mixture of Experts*), picked on the basis of its performance. This allows to 
combine multiple strategies to solve the same problem, providing improved performance, fault 
tolerance, efficiency, and reducing its overall cost. The modules are completely generic, e.g. 
from hard coded sets of rules to time-dependent neural networks (e.g. *Spiking Neuron Model*). 
Genetic algorithms are used for configuration, optimization, network structure design, formula 
evolution; focus on efficiency; extraction of symbolic information from raw data.

## Project purpose

*Note: this project is still in its early design and development stages.*

Development of a system with the following features:

- Adaptive.
- Modular, multi-approach:
    - Supervised, reinforcement and unsupervised learning.
    - Modularity in space and time.
    - Plug-in architecture: modules can be added/removed at runtime.
    - Each module can have its own license.
    - Modules can be both software and hardware based.
- Fault tolerant.
- High performance.
- Power efficient.
- Extensible.
- Compact.
- Training set efficient.

The environment it has to operate in can be a real-time one.

The approach is a combination of:

- *Mixture of Experts* model, to implement the modular architecture.
- Any kind of algorithms in the experts:
    - Classic algorithms.
    - Classic neuron models.
    - *Spiking neuron* models (modified for better efficiency on conventional systems).
- Genetic Algorithms, for the evolution of specific parameters only (e.g. not the synaptic weights).
- *Neural microcircuits*: higher level functional blocks (~ logic gates).
- *Cortical columns*: complete processing of a small subset of the input.
- Dynamical cell assemblies.

## Learning approaches

- Development of Experts for low level tasks.
- Use the developed experts as building blocks for higher level tasks.
    - Create a *tree/graph-like experts structure*.
    - *Once a higher level expert is formed and tested, store it as
      another basic building block.*
    - *Computation time and energy consumption optimizations.*
- *Learn in phases, like kids do:*
    - Simple concepts first.
    - Complex concepts can be decomposed in simple concepts.
- Average neuron activation in the human brain:
    - Considering whole brain energy consumption, single neuron energy 
        consumption, and total number of neurons, we get that the brain works as a 
        sparse system.
- *Training sets*
    - *Cannot be too vast* (use a size compatible with what a human can
      see in his first n years of his life).
    - Vectorization (or other transformations) to get more efficient learning.

## Integration with other projects

- Neuro relation with other third-party projects:
    - Make Neuro a module of a third-party project.
    - Make a third-party project a module of Neuro.
- Candidate external projects: PyTorch, TensorFlow.

## Links

Please, go to the `NeuroOverview.pdf` file in this repository for an overview of this project.



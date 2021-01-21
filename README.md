# MLAdy - Autonomy for Established Vehicles and Machinery <!-- omit in toc -->

## Executive summary

MLAdy offers a budget-oriented way to rapidly autonomize established vehicles and machinery in public and industrial applications, using a retrofitting approach with scalable complexity, scope and size.

## Table of Contents <!-- omit in toc -->

- [Executive summary](#executive-summary)
- [Abbreviations](#abbreviations)
- [Background](#background)
- [Problem Statement](#problem-statement)
- [Goals and Objectives](#goals-and-objectives)
- [Limitations](#limitations)
- [Project Implementation](#project-implementation)
  - [Project Checklist](#project-checklist)
- [Theory and Key Concepts](#theory-and-key-concepts)
  - [Artificial Intelligence](#artificial-intelligence)
  - [Neural network](#neural-network)
  - [Machine learning](#machine-learning)
  - [Classification](#classification)
  - [Reinforcement Learning](#reinforcement-learning)
  - [Model (Machine Learning)](#model-machine-learning)
  - [Transfer Learning](#transfer-learning)
  - [Composition Learning](#composition-learning)
  - [Computer Vision](#computer-vision)
  - [Retrofit](#retrofit)
  - [Real-Time Development Platform](#real-time-development-platform)
- [Technical Review](#technical-review)
  - [Similar offerings](#similar-offerings)
  - [Similar offerings](#similar-offerings-1)

## Abbreviations

- AI: Artificial intelligence
- RC: Radio controlled
- PoC: Proof of concept
- MVP: Minimum viable product
- MCU: Microcontroller unit
- NMBU: Norwegian University of Life Sciences (Norges Miljø- og Biovitenskapelige Universitet)

## Background

The idea for MLAdy was born out of a discussion in 2019, regarding automation of forklifts at a factory where part of the core team does software development. Lacking in available technology and competence, the project was put on hold, but recent advancements in reinforcement learning and computer vision has made the challenge possible to tackle for a small engineering team. These new-found tools and methods facilitates the creation of a framework for quick prototyping, enabling implementation in a wide variety of areas.

Most robotics firms develop expensive and custom-made robots entirely from scratch, and as a result adoption of the technology suffers. The main challenge in combining AI and robotics is often not the hardware, but the digital brain that operates it. Most tasks already have suitable machinery, all the they need is just the autonomy. That's why MLAdy exists - to develop a framework that allows for quick, cheap and accessible realization of autonomous robots.

Take farm and construction vehicles for example; this range of vehicles are made to handle any task on any budget, while being mass produced and widely available industrial solutions tested in the real world for a long time. By using this hardware over from-scratch-solutions, complex and time-consuming development is cut to a minimum.

As a bonus, if the task does not require full size vehicles, scaled down RC variants can be used. They are lot safer to develop and deploy than heavy machinery. The other way around? Not a problem - a generalized abstract reinforcement learning approach will work just as well with custom hardware facing highly complex tasks. This way, MLAdy proposes a way to scale complexity as needed.

MLAdy's long-term vision is to be an AI- and robotics foundation intended for a wide variety of use-cases.

## Problem Statement

Operations utilizing vehicles, machinery and physical labor are resource-intensive and present serious health risks.

MLAdy offers a highly generalized and scalable way to apply reinforcement learning to existing hardware, offloading direct operation of heavy machinery and physical tasks without the need for hardware replacement.

## Goals and Objectives

MLAdy's overall goal is to speed up the adoption of autonomous robots for the betterment of humanity, by fusing existing hardware with modern AI.

To do this, a framework that allows speedy and scalable implementation with any hardware is need.

In order to develop such a framework, the following objectives and activities must be met and performed:

- Theoretical framework and technical review
  - Identify key theoretical concepts in order to establish foundational knowledge
  - Research phase for establishing the framework
    - Identify key research work
    - Technical review
      - Identify key experimental work and data
      - Obtain an overview of existing platforms
      - Establish key framework components
      - Identify framework constraints
  - Summary suggesting way forward
- Develop platform 
  - Prototypes
    - PoC (proving end-to-end feasibility of framework)
    - MVP (single vehicle)
    - MVP Fleet (multiple vehicles)
    - MVP Fleet (multiple vehicles)
- Evaluate framework
  - Design and plan out experiment
  - Experimental validation of framework
  - Gauge commercial interest of application of framework
- Recommendations and conclusion
  - Possible improvements
  - Feasible operations to automate
  - Potential clients to pursue


## Limitations

As possible applications of the framework can vary enormously, a clear and concise goal is needed to formulate the framework effectively. This should optimally be something that attracts developers, students and investors to the project, as it will help speed up the process further and increase overall chances of success.

The environmental challenges of this day and age is as relevant as ever, and garbage is piling up. Hence, MLAdy has decided that the first half of the project will consist of a deployment of a fleet of budget RC vehicles to collect garbage at the Norwegian University of Life Sciences (NMBU) and surrounding areas.

Given that an implementation of the framework together with an industrial partner follows, new limitations will be introduces organically based on the automation scope.

## Project Implementation

Project start: 1. January 2021

Based on stated goal and objectives, the project is divided into seven phases (see the [project checklist](#project-checklist) for more detailed milestones). Development, experimentation and evaluation is done for each prototype step (2-6), to promote pivoting as necessary. The most critical experiment will be an implementation with an industrial partner.

For safety, ease-of-development and budget-friendliness, RC-scale vehicles will be used up until phase 5.

1. Gauge feasibility  
2021 Q1  
Goal: Create overview of existing technology and competition 

1. Proof of concept  
2021 Q1  
Goal: Prove that real world application can be achieved with abstracted simulated training

1. MVP (Minimum Viable Product)  
2021 Q1-Q2  
Goal: Extend features to perform a complete task (trash removal)

1. Fleet prototype  
2021 Q2-Q3  
Goal: Scale to multiple vehicles, achieve autonomous cooperation with minimal interaction

1. Scale vehicle size  
2021 Q4  
Goal: Scale to true size vehicles for applications not in public areas, e.g. factories and warehouses

1. Implementation project  
2022 Q1-Q3  
Goal: Successfully apply framework in a useful real life application

1. Reflection and next-steps  
2022 Q3  
Goal: Document key findings throughout the project and propose possible next-steps

All phases will benefit greatly from funding. The most critical parts are the beginning of phase 3 and out, where a multitude of vehicles and equipment is needed.

The proof of concept is approximately halfway done at the time of writing.

### Project Checklist

- [x] Gauge feasibility
  - [x] Existing technology
  - [x] Competition
- [ ] Proof of concept
  - [x] Simulation
    - [x] Abstract* vehicle simulation  
    _By abstract we mean a simplified generalization with randomized parameters. This will enable the model to understand different vehicle properties and adjust output accordingly._
    - [x] Abstract environment simulation
    - [x] Easy-to-use reinforcement learning
    - [ ] Mental model
      - [x] Simplified mental model (perfect preprocessed data)
        - [x] Target position relative to vehicle
        - [x] Vehicle orientation (relative to gravity)
        - [ ] Traversable area detection
      - [ ] Complex mental model (same as noisy real world implementation)
  - [ ] Transfer simulated learning to the real world
    - [x] Vehicle
      - [x] RC-car equipped with [NVIDIA Jetson Nano](https://developer.nvidia.com/EMBEDDED/jetson-nano-developer-kit) (based on [DonkeyCar](https://www.donkeycar.com/))
    - [ ] Complex mental model
      - [ ] Sensory input
        - [x] Vision
          - [x] Object detection (trash)
          - [x] Depth map
        - [ ] Orientation
          - [ ] Gyroscope
      - [ ] Virtual map
        - [ ] Target position relative to vehicle
        - [ ] Vehicle orientation (relative to gravity)
        - [ ] Traversable area detection
    - [x] Extract learned model for real word application
  - [ ] Train in the real world
  - [ ] Successfully detect and drive to trash
- [ ] MVP
  - [ ] Add abstract excavator and wheel loader vehicles to simulation
    - [ ] Create abstract arm
    - [ ] Add abstract arm to abstract vehicle
  - [ ] Simulated training
    - [ ] Detect trash
    - [ ] Drive to trash
    - [ ] Pick up trash
    - [ ] Place trash where told
  - [ ] Retrofit a microcontroller unit (MCU) and necessary sensors on a radio controlled excavator and/or wheel loader
  - [ ] Real world training
  - [ ] Successfully do steps necessary for removing trash
    - [ ] Detect trash
    - [ ] Drive to trash
    - [ ] Pick up trash
    - [ ] Place trash where told
- [ ] Fleet prototype
  - [ ] Extend sensory inputs
    - [ ] GPS
  - [ ] Scale MVP to deploy a fleet of minimum 10 vehicles cooperating
  - [ ] Charging
    - [ ] Stations
    - [ ] Routines
  - [ ] Autonomous operation with minimal interaction 24/7
- [ ] Scale vehicle size
  - [ ] Successfully use framework with a one-to-one scale vehicle (e.g. forklift, car, wheel loader, excavator)
- [ ] Implementation project
  - [ ] Make deal with a suited candidate for implementation  
  _Some of MLAdy's core members has already contacted their workplace regarding testing at their factory facilities. The contact person likes the idea and will likely propose an implementation when MLAdy is ready._
  - [ ] Formulate detailed plan for implementation
  - [ ] Implement
- [ ] Documentation  
_As the time-frame for documentation coincides with the core team's final semester, this project may be a possible subject for a master's thesis._
  - [ ] Key findings
  - [ ] Next-steps

## Theory and Key Concepts

_Note: If no source is cited, definition is formulated by the core team._

### Artificial Intelligence

[**Investopedia** defines artificial intelligence as follows](https://www.investopedia.com/terms/a/artificial-intelligence-ai.asp#:~:text=Artificial%20intelligence%20(AI)%20refers%20to,as%20learning%20and%20problem%2Dsolving.): 

> Artificial intelligence (AI) refers to the simulation of human intelligence in machines that are programmed to think like humans and mimic their actions. The term may also be applied to any machine that exhibits traits associated with a human mind such as learning and problem-solving

### Neural network

A neural network is an interconnected web of nodes, each layer consisting of weights and biases affecting how input to the network will be transformed to an output.

### Machine learning

[**TechTarget**'s definition of machine learning](https://searchenterpriseai.techtarget.com/definition/machine-learning-ML#:~:text=Machine%20learning%20(ML)%20is%20a,to%20predict%20new%20output%20values.):

> Machine learning (ML) is a type of artificial intelligence (AI) that allows software applications to become more accurate at predicting outcomes without being explicitly programmed to do so. Machine learning algorithms use historical data as input to predict new output values.

### Classification

Classification is a way of organizing input/stimuli in categories. 

### Reinforcement Learning

Reinforcement learning is a way to utilize machine learning to reinforce an agents behaviors in an environment, based on rewards.

### Model (Machine Learning)

A multi-input and multi-output function, most commonly consisting of a conventional neural network, created (trained) with machine learning techniques.

### Transfer Learning

Using part of a model to train a new model. For example, the introductory layers of object detection is often extracting fundamental features, and can be used to detect cats or dogs, depending on the following layers.

### Composition Learning

A form of composition, where multiple machine learning models can be connected to each other. An example is a classification model that finds traversable areas, feeding the output to a behavior decision model, that activates a model responsible for movement, if it decides to move.

### Computer Vision

Using sensory input (often for some wavelength - camera, lidar, radar) to perceive. Concept can be extended to producing a mental model or map.

A mental model may be useful for reinforcement learning agents, as it provides a deeper understanding of inputs and outputs, as well as a better foundation for developers to assign rewards and other logic.

### Retrofit

To apply something new to an existing object.



### Real-Time Development Platform

Software made for real-time simulation. May be interchanged with the term "game engine", depending on application of the software.

## Technical Review

### Similar offerings


### Similar offerings
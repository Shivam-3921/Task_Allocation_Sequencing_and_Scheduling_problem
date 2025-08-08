# Task Scheduling Problem
This repository contains a Jupyter Notebook that addresses a robot team task allocation, sequencing, and scheduling optimization problem. The goal is to minimize the total mission completion time (makespan) for a team of identical robots performing tasks at various target locations.

## Project Description
The problem involves:

- A set of target locations (excluding a depot), each with an associated processing time for a task.
- Travel paths with known distances connecting these locations.
- A team of identical robots starts from a central depot.

Robots must travel to targets and perform tasks. The mission completion time is determined by both travel and processing durations.

The key decision variables are:

- Assignment of target locations to robots.

- Sequence of visits for each robot.

The objective is to minimize the total mission completion time, subject to constraints on robot travel and precedence between travel and processing.

## Repository Structure
The project is contained within a single Jupyter Notebook file:

- Task_Scheduling_Problem.ipynb: This notebook includes:

  - Importing Libraries: Essential Python libraries like numpy, random, networkx, matplotlib, pandas, itertools, and time.

  - Defining the Problem: A detailed formulation of the task scheduling problem.

  - Parameters: Customizable parameters such as:

    - TARGETS: Number of target locations.

    - ROBOTS: Number of robots.

    - MAX_PATH_LENGTH: Maximum distance between any two locations.

    - MAX_PROCESSING_TIME: Maximum processing time for any task.

- Creating Paths: Generation of a symmetric adjacency matrix representing random travel distances between target locations, including handling of absent routes (infinite distances) and connections to the depot.

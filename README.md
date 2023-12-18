# Dining Philosophers Problem Solution
This repository contains a solution to the Dining Philosophers Problem, a classic synchronization and concurrency problem often discussed in parallel programming courses. The problem revolves around a scenario where a number of philosophers sit around a dining table, and each philosopher alternates between thinking and eating. The challenge is to avoid deadlock and contention for resources, particularly the forks each philosopher needs to eat.

## Background
The Dining Philosophers Problem was assigned as part of our coursework in the parallel programming course at Celal Bayar University. The goal was to apply synchronization concepts to resolve the challenges posed by concurrent access to shared resources.

## Team Collaboration
To tackle this problem effectively, we formed a collaborative team. The team worked together to design a solution that prevents deadlock and race conditions, employing synchronization mechanisms to ensure the proper sharing of forks among philosophers.

## How it Works

### 1) Assigning Priorities:

Each fork is given a unique identifier or priority. This can be as simple as assigning sequential numbers to the forks.
### 2) Picking Up Forks:

Philosophers must adhere to a rule when picking up forks: they should always pick up the fork with the lower priority first before attempting to pick up the higher-priority fork.
### 3) Releasing Forks:

Similarly, when releasing forks, philosophers follow the reverse order: the higher-priority fork is put down before the lower-priority one.

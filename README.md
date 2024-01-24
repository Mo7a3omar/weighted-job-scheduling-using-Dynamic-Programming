# Weighted Job Scheduling with Dynamic Programming and Binary Search

This Python program implements the Weighted Job Scheduling algorithm using Dynamic Programming and Binary Search.

## Contents

1. [Introduction](#introduction)
2. [Implementation Details](#implementation-details)
3. [Usage](#usage)
4. [Example](#example)

## Introduction

The program solves the Weighted Job Scheduling problem, where each job has a start time, finish time, and a corresponding profit. The goal is to find the maximum total profit by selecting non-overlapping jobs.

## Implementation Details

- The program defines a `Job` class representing a job with start time, finish time, and profit.
- It utilizes a binary search function to find the latest job that doesn't conflict with the current job.
- The main scheduling function sorts the jobs by finish time and uses dynamic programming to calculate the maximum profit.

## Usage

- Define a list of `Job` instances, each representing a job with start time, finish time, and profit.
- Call the `schedule` function with the list of jobs to get the maximum total profit.

## Example

```python
# Driver code to test the Weighted Job Scheduling algorithm
job = [Job(1, 2, 50), Job(3, 5, 20),
       Job(6, 19, 100), Job(2, 100, 200)]
print("Optimal profit is"),
print(schedule(job))
```

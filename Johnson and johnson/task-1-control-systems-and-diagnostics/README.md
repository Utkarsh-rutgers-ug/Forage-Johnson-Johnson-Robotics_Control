# Task 1 - Introduction to Control Systems and Diagnostics

## Simulation context

The task focuses on diagnosing response-time delays in a surgical robotic arm.
The core engineering loop is to observe a command, measure how long each stage
takes, isolate the slow stage, improve it, and verify the result without
changing the intended behavior.

## Learning objectives

By the end of this task, you should be able to:

- explain the input -> processing -> output path of a robotic control system;
- distinguish open-loop control from closed-loop control;
- identify the roles of sensors, the processing unit, and actuators;
- recognize signal delays, processing bottlenecks, and coding inefficiencies;
- measure elapsed time in Python and compare results across repeated runs;
- isolate a slow section of code and validate an optimization.

## Supplied guide: key ideas

The guide describes closed-loop control as the appropriate model for surgical
robotics because sensor feedback lets the system correct movement in real time.
It identifies three common responsiveness problems: signal delays, processing
bottlenecks, and coding inefficiencies. It also introduces Python timing and
iterative testing as diagnostic techniques.

The timing snippet in the guide is an illustrative example, not a complete task
solution. For actual measurements, we will discuss appropriate clocks,
repeatability, warm-up effects, and how to avoid measuring unrelated work.

## Working structure

```text
task-1-control-systems-and-diagnostics/
|-- references/     # Supplied Forage material
|-- src/            # Control or diagnostic code
|-- tests/          # Tests and timing checks
|-- deliverables/   # Final submission artifacts
|-- notes.md        # Your reasoning and observations
`-- README.md
```

## Current status

- [x] Review the introductory guide.
- [x] Prepare the task workspace.
- [ ] Add the official Task 1 prompt and starter code.
- [ ] Establish a baseline response-time measurement.
- [ ] Locate the source of delay.
- [ ] Implement and validate an improvement.
- [ ] Prepare the final deliverable.


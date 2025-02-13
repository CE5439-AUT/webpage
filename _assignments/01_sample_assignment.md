---
type: assignment
date: 2025-02-13T4:00:00+4:30
title: 'Assignment #1 - Ch2. Continuous Dynamics'
pdf: /static_files/assignments/HW1/HW1_Ch2.pdf
# attachment: /static_files/assignments/asg.zip
# solutions: /static_files/assignments/asg_solutions.pdf
due_event: 
    type: due
    date: 2025-02-18T23:59:00+3:30
    description: 'Assignment #1 due'
---

## Problems:

### 2. 
Show that if a system ![equation](https://latex.codecogs.com/png.image?A^\mathbb{R}%20\rightarrow%20B^\mathbb{R}) is strictly causal and memoryless, then its output is constant. Constant means that the output ![equation](https://latex.codecogs.com/png.image?(S(x))(t)) at time \( t \) does not depend on \( t \).



### 3. 
This exercise studies linearity.
* Show that the helicopter model defined in Example 2.1 is linear if and only if the initial angular velocity ![equation](https://latex.codecogs.com/png.image?\dot{\theta}_{y}(0) = 0)
* Show that the cascade of any two linear actors is linear.
* Augment the definition of linearity so that it applies to actors with two input signals and one output signal. Show that the adder actor is linear.


### 4. 
Consider the helicopter of Example 2.1, but with a slightly different definition of the input and output. Suppose that, as in the example, the input is ![equation](https://latex.codecogs.com/png.image?T_y: \mathbb{R} \rightarrow \mathbb{R}), as in the example, but the output is the position of the tail relative to the main rotor shaft. Specifically, let the \( x-y \) plane be the plane orthogonal to the rotor shaft, and let the position of the tail at time \( t \) be given by a tuple \( ((x(t), y(t))) \)  Is this model LTI? Is it BIBO stable?



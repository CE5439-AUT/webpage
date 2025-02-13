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

### Q2. 
Show that if a system ![equation](https://latex.codecogs.com/png.image?A^\mathbb{R}%20\rightarrow%20B^\mathbb{R}) is strictly causal and memoryless, then its output is constant. Constant means that the output ![equation](https://latex.codecogs.com/png.image?(S(x))(t)) at time \( t \) does not depend on \( t \).



### Q3. 
This exercise studies linearity.
* Show that the helicopter model defined in Example 2.1 is linear if and only if the initial angular velocity ![equation](https://latex.codecogs.com/png.image?\dot{\theta}_{y}(0) = 0)
* Show that the cascade of any two linear actors is linear.
* Augment the definition of linearity so that it applies to actors with two input signals and one output signal. Show that the adder actor is linear.


### Q4. 
Consider the helicopter of Example 2.1, but with a slightly different definition of the input and output. Suppose that, as in the example, the input is ![equation](https://latex.codecogs.com/png.image?T_y: \mathbb{R} \rightarrow \mathbb{R}), as in the example, but the output is the position of the tail relative to the main rotor shaft. Specifically, let the \( x-y \) plane be the plane orthogonal to the rotor shaft, and let the position of the tail at time \( t \) be given by a tuple \( ((x(t), y(t))) \)  Is this model LTI? Is it BIBO stable?


### Q5:
Consider a rotating robot where you can control the angular velocity around a fixed axis.

* Model this as a system where the input is angular velocity ![equation](https://latex.codecogs.com/png.image?\dot{\theta}) and the output is angle ![equation](https://latex.codecogs.com/png.image?\theta) Give your model as an equation relating the input and output as functions of time.
* Is this model BIBO stable?
* Design a proportional controller to set the robot onto a desired angle. That is, assume that the initial angle is ![equation](https://latex.codecogs.com/png.image?\theta(0)=0), and let the desired angle be ![equation](https://latex.codecogs.com/png.image?\psi(t)=au(t)) where \( u \) is the unit step function. Find the actual angle as a function of time and the proportional controller feedback gain \( K \). What is your output at \( t=0 \)? What does it approach as \( t \) gets large?


### Q6:
A DC motor produces a torque that is proportional to the current through the windings of the motor. Neglecting friction, the net torque on the motor, therefore, is this torque minus the torque applied by whatever load is connected to the motor. Newton’s second law (the rotational version) gives

![equation](https://latex.codecogs.com/png.image?k_{T}i(t)-x(t)=I\frac{d}{dt}\omega(t))

where \( k_T \) is the motor torque constant, \( i(t) \) is the current at time \( t \), \( x(t) \) is the torque applied by the load at time \( t \), \( I \) is the moment of inertia of the motor, and ![equation](https://latex.codecogs.com/png.image?\omega(t)) is the angular velocity of the motor.

* Assuming the motor is initially at rest, rewrite (2.15) as an integral equation.
* Assuming that both \( x \) and \( i \) are inputs and ![equation](https://latex.codecogs.com/png.image?\omega(t)) is an output, construct an actor
* In reality, the input to a DC motor is not a current, but is rather a voltage. If we assume that the inductance of the motor windings is negligible, then the relationship between voltage and current is given by

![equation](https://latex.codecogs.com/png.image?v(t)=R_i(t)+k_b\omega(t))

where \( R \) is the resistance of the motor windings and \( k_b \) is a constant called the motor back electromagnetic force constant. The second term appears because a rotating motor also functions as an electrical generator, where the voltage generated is proportional to the angular velocity.

Modify your actor model so that the inputs are \( v \) and \( x \) rather than \( i \) and \( x \).

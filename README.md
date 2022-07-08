# Rule-based-Fuzzy-System
A robot is navigating in an environment where there are obstacles it needs to avoid. The robot is equipped with sensors that can detect the obstacle. It also relays the distance and angle relative to the robot. Using these measurements, create a fuzzy inferencing system to decide the Speed and Steering.

The following fuzzy quantities are defined, with their corresponding states:
D 	Distance from obstacle 	N=Near, F=Far, VF=Very Far
A 	Angle with obstacle 	  S=Small, M=Medium, L=Large
S 	Speed         					SS= Slow Speed, MS=Medium Speed, FS=Fast Speed, MS= Maximum Speed
ST 	Steering Turn     			MST= Mild Turn, SST=Sharp Turn, VST= Very Sharp Turn

The universe of each of the quantities are defined below
Fuzzy Quantity Minimum Value Maximum Value Step
	D 				0 				10 		0.5
	A 				0 				90 		 1
	S 				0 				5 		0.2
	ST 				0 				90 		 1

Assume that the angles and steering are the same for both right and left directions. For example, a reading of angle=-55° is the same as angle=55° for your fuzzy system.

In your design, please consider the following preliminary behavior as a guide. Note that the system’s behavior is not limited to these actions but must include them:
• When an obstacle is detected, avoid it: does not matter which direction; left or right
• When there is no obstacle move forward
• Speed is reduced when turning away from an obstacle
• Speed is increased when cruising (when there is no obstacle)

1. Design a fuzzy system including:
	a. The membership functions for each of the fuzzy quantities (following the provided states)
	b. The rule base that will be used for inferencing
	c. The inferencing system that will be used (Mamdani, Sugeno, etc…)
	d. The defuzzification method
2. Explain your choices in 1-c and 1-d with details.
3. Provide at least 2 examples of inputs and show your system’s output control command.

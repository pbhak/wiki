# Intake Control


## Working with Design for Initial Design
The original design for the arm includes a main claw controlled by pistons opening and closing. Then, there are attached motors to circular grippers so that it rotates when the cone is grabbed so that it is rotated to an upright position.

Intake Responsibilities: 
1. Code to allow driver to manually extend arm.
whenHeldRightBumper(extendArm(speed:1))
2. Code to allow driver to manually close piston.
whenClickedRightTrigger(extendPiston())
3. Code to allow driver to manually retract arm.
whenHeldLeftBumper(retractArm(speed:1)
4. Possibly code to automate process (depends on other subteams choices)
whenClickedB(runIntakeProcess(cone))
whenClickedA(runIntakeProcess(cube))
5. Open piston to width of cube and more.
6. In 3 seconds (say) close piston around cube.

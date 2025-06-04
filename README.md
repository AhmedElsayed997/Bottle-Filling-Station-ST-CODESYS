# Bottle-Filling-Station-ST-CODESYS

## Description:
This project controls a bottle filling station using a state machine logic with timers, sensors, and actuators (valves and conveyors). The system detects bottles, fills them for a specific time, and then moves them out.

## Main States:

## IDLE
Starts the process when a start condition is detected.
Activates CONVEYOR_LINE1 and transitions to the next state.

## DETECTION
Checks if a bottle is detected via a sensor.
Stops the conveyor and opens the filling valve if a bottle is present.

## FILLING
Activates a filling timer (FILLING_TIME).
Once the timer finishes, closes the valve and restarts the conveyor.


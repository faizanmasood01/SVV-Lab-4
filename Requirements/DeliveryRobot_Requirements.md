| Req_Id | Description                                                                                              | Priority |
| ------ | -------------------------------------------------------------------------------------------------------- | -------- |
| R1     | When powered on with no active delivery request, the robot shall remain in the IDLE state.               | High     |
| R2     | When a delivery request is received while the robot is IDLE, the robot shall transition to NAVIGATING.   | High     |
| R3     | While NAVIGATING, the robot shall continuously monitor its surroundings for obstacles.                   | High     |
| R4     | When an obstacle is detected during navigation, the robot shall transition to AVOIDING_OBSTACLE.         | High     |
| R5     | When the obstacle has been successfully avoided, the robot shall return to NAVIGATING.                   | High     |
| R6     | When the destination is reached, the robot shall transition from NAVIGATING to DELIVERING.               | High     |
| R7     | After successful delivery, the robot shall transition from DELIVERING to RETURNING.                      | High     |
| R8     | When the battery becomes critically low during navigation, the robot shall transition to RETURNING.      | High     |
| R9     | When the robot reaches the warehouse, it shall transition from RETURNING to IDLE.                        | High     |
| R10    | The robot shall not transition directly from IDLE to DELIVERING or from AVOIDING_OBSTACLE to DELIVERING. | Critical |



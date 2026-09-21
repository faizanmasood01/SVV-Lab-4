| State_Id | State_name        | Description                                                        | Entry_condition                                               | Exit_condition                                              |
| -------- | ----------------- | ------------------------------------------------------------------ | ------------------------------------------------------------- | ----------------------------------------------------------- |
| S1       | IDLE              | Robot is at the warehouse and waiting for a delivery request.      | Robot is powered on, or warehouse is reached after returning. | Delivery Request Received                                   |
| S2       | NAVIGATING        | Robot is travelling toward the requested destination.              | Delivery Request Received, or Obstacle Avoided.               | Destination Reached, Obstacle Detected, or Critical Battery |
| S3       | AVOIDING_OBSTACLE | Robot temporarily stops normal navigation and handles an obstacle. | Obstacle Detected during navigation.                          | Obstacle Avoided                                            |
| S4       | DELIVERING        | Robot performs the package delivery at the destination.            | Destination Reached.                                          | Delivery Successful                                         |
| S5       | RETURNING         | Robot travels back to the warehouse.                               | Delivery Successful or Critical Battery.                      | Warehouse Reached                                           |


| Req. ID | Description | Priority |
| :--- | :--- | :--- |
| **R1** | The system shall remain in the **IDLE** state upon startup, awaiting a valid delivery request. | **High** |
| **R2** | The system shall transition from **IDLE** to **NAVIGATING** immediately upon receiving a delivery request. | **High** |
| **R3** | The system shall continuously monitor its surroundings for obstacles while actively navigating. | **High** |
| **R4** | The system shall temporarily pause normal navigation and transition to **AVOIDING_OBSTACLE** upon detecting an obstacle. | **High** |
| **R5** | The system shall resume normal navigation back to the **NAVIGATING** state once an obstacle has been successfully bypassed. | **High** |
| **R6** | The system shall initiate the delivery process when the robot successfully arrives at the destination. | **High** |
| **R7** | The system shall begin its return journey to the warehouse once the package delivery is completed. | **Medium** |
| **R8** | The system shall abort the current delivery mission and return to the warehouse immediately if the battery level becomes critically low. | **High** |
| **R9** | The system shall return to the **IDLE** state upon successfully reaching the warehouse. | **Medium** |
| **R10** | The system shall strictly prohibit illegal state transitions, specifically preventing direct movement from **IDLE** to **DELIVERING** or from **AVOIDING_OBSTACLE** to **DELIVERING**. | **High** |

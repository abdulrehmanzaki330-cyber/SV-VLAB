## Task 2 — Identify States

Here is the detailed state model for the autonomous delivery robot, defining each state with its ID, name, description, entry condition, and exit condition:

| State ID | State Name | Description | Entry Condition | Exit Condition |
| :--- | :--- | :--- | :--- | :--- |
| **S1** | `IDLE` | The robot is powered on and waiting at the warehouse for a new task assignment. | System startup OR warehouse reached successfully from a previous trip. | Receipt of a valid delivery request. |
| **S2** | `NAVIGATING` | The robot is actively traveling from its current location toward the target destination. | Transition from `IDLE` after receiving a request OR successful avoidance of an obstacle. | Obstacle detected OR destination reached OR battery level becomes critically low. |
| **S3** | `AVOIDING_OBSTACLE` | The robot halts normal path planning to maneuver around a physical obstruction in its path. | An obstacle is detected by the robot's surrounding sensors during navigation. | Obstacle successfully avoided/bypassed. |
| **S4** | `DELIVERING` | The robot performs the package drop-off process at the target destination. | Destination is successfully reached from the `NAVIGATING` state. | Package delivery process completed successfully. |
| **S5** | `RETURNING` | The robot aborts or completes its task and travels back to the warehouse base. | Delivery successfully completed OR critical battery level triggered during navigation. | Warehouse base successfully reached. |

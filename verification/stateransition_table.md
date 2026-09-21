## Task 3 — State Transition Table

Here is the transition table detailing the relationship between states, events, resulting states, and their corresponding requirement IDs:

| Transition ID | From State | Event / Condition | To State | Req. ID |
| :--- | :--- | :--- | :--- | :--- |
| **T1** | `IDLE` | Delivery Request Received | `NAVIGATING` | **R2** |
| **T2** | `NAVIGATING` | Obstacle Detected | `AVOIDING_OBSTACLE` | **R4** |
| **T3** | `AVOIDING_OBSTACLE` | Obstacle Avoided | `NAVIGATING` | **R5** |
| **T4** | `NAVIGATING` | Destination Reached | `DELIVERING` | **R6** |
| **T5** | `DELIVERING` | Delivery Successful | `RETURNING` | **R7** |
| **T6** | `NAVIGATING` | Critical Battery | `RETURNING` | **R8** |
| **T7** | `RETURNING` | Warehouse Reached | `IDLE` | **R9** |

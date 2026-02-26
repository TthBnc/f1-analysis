# Attribute Registry

> Master list of all attributes used in the analysis system.
> Updated as weekend agents propose and confirm new attributes.
>
> **Purpose:** This registry defines the vocabulary of the prediction algorithm.
> Every attribute here is a dimension the algorithm can score against.
> Attributes must be observable, measurable through session results, and
> relevant to predicting future performance.

## Driver Attributes

| Attribute                     | Type  | Scale | Description                                    | Introduced |
| ----------------------------- | ----- | ----- | ---------------------------------------------- | ---------- |
| `rain_performance`            | scale | 1-5   | Performance in wet/mixed conditions            | Baseline   |
| `qualifying_specialist`       | scale | 1-5   | Outperforms race pace in qualifying            | Baseline   |
| `race_craft`                  | scale | 1-5   | Wheel-to-wheel, overtaking, defending          | Baseline   |
| `tyre_management`             | scale | 1-5   | Stint extension, tyre preservation             | Baseline   |
| `home_race_boost`             | scale | 1-5   | Performance lift at home GP                    | Baseline   |
| `form_trajectory`             | scale | 1-5   | Recent form direction (1=declining, 5=peaking) | Baseline   |
| `first_lap_aggression`        | scale | 1-5   | Positions gained/lost on lap 1                 | Baseline   |
| `consistency`                 | scale | 1-5   | Low error rate, low self-inflicted DNFs        | Baseline   |
| `pressure_performance`        | scale | 1-5   | High-stakes / championship moment performance  | Baseline   |
| `starts`                      | scale | 1-5   | Launch quality off the line                    | Baseline   |
| `recovery_drive`              | scale | 1-5   | Performance when starting out of position      | Baseline   |
| `street_circuit_performance`  | scale | 1-5   | Street circuit vs permanent track aptitude     | Baseline   |
| `traffic_management`          | scale | 1-5   | Handling lapped traffic or midfield battles    | Baseline   |
| `adaptability_to_car_changes` | scale | 1-5   | Performance after regulation/setup shifts      | Baseline   |
| `team_order_compliance`       | scale | 1-5   | Response to team orders                        | Baseline   |

## Car/Team Attributes

| Attribute                         | Type  | Scale | Description                               | Introduced |
| --------------------------------- | ----- | ----- | ----------------------------------------- | ---------- |
| `high_downforce_efficiency`       | scale | 1-5   | Competitiveness on high-df circuits       | Baseline   |
| `low_drag_straight_speed`         | scale | 1-5   | Top speed on power circuits               | Baseline   |
| `mechanical_grip`                 | scale | 1-5   | Slow-speed corner performance             | Baseline   |
| `reliability`                     | scale | 1-5   | Mechanical DNF frequency (5=bulletproof)  | Baseline   |
| `pit_stop_consistency`            | scale | 1-5   | Pit stop speed and error rate             | Baseline   |
| `strategy_quality`                | scale | 1-5   | Tyre, weather, undercut/overcut decisions | Baseline   |
| `upgrade_trajectory`              | scale | 1-5   | Season development direction              | Baseline   |
| `wet_weather_setup`               | scale | 1-5   | Car competitiveness in rain               | Baseline   |
| `tyre_degradation_characteristic` | scale | 1-5   | Tyre preservation (5=gentle)              | Baseline   |
| `dirty_air_sensitivity`           | scale | 1-5   | Performance loss following (5=unaffected) | Baseline   |
| `power_unit_performance`          | scale | 1-5   | Straight-line and deployment              | Baseline   |
| `cool_condition_performance`      | scale | 1-5   | Cold ambient/track temp performance       | Baseline   |
| `hot_condition_performance`       | scale | 1-5   | Hot ambient/track temp performance        | Baseline   |

## Circuit Attributes

| Attribute                | Type     | Scale       | Description                           | Introduced |
| ------------------------ | -------- | ----------- | ------------------------------------- | ---------- |
| `favours_downforce`      | scale    | 1-5         | Downforce requirement level           | Baseline   |
| `overtaking_difficulty`  | scale    | 1-5         | How hard to pass (5=very hard)        | Baseline   |
| `safety_car_probability` | scale    | 1-5         | Historical SC likelihood              | Baseline   |
| `weather_variability`    | scale    | 1-5         | Rain/changing condition likelihood    | Baseline   |
| `altitude`               | value    | meters      | Elevation (engine performance impact) | Baseline   |
| `surface_abrasiveness`   | scale    | 1-5         | Tyre wear aggression                  | Baseline   |
| `street_circuit`         | category | yes/no/semi | Circuit type                          | Baseline   |
| `pit_lane_time_loss`     | value    | seconds     | Time cost of pit stop                 | Baseline   |
| `traction_zone_density`  | scale    | 1-5         | Slow-speed traction zone count        | Baseline   |
| `track_evolution`        | scale    | 1-5         | Grip improvement through sessions     | Baseline   |
| `drs_effectiveness`      | scale    | 1-5         | DRS overtaking power                  | Baseline   |

## Agent-Proposed Attributes

_(Appended by weekend agents as new patterns emerge. Format:)_

| Attribute                            | Category | Type | Scale | Description | Proposed After | Evidence |
| ------------------------------------ | -------- | ---- | ----- | ----------- | -------------- | -------- |
| _(populated during season analysis)_ |          |      |       |             |                |          |

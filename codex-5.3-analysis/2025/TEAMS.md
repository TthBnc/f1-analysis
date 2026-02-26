# 2025 Teams & Car Attributes

> Last updated: R01 Australian Grand Prix (post-weekend integration)

## Attribute Scale

All attributes scored **1.0 - 5.0** (one decimal). 3.0 = grid average.

## Calibration Reference

Same scale as DRIVERS.md. The distribution across 10 teams is centered near 3.0.

---

### McLaren Mercedes

**Power Unit:** Mercedes
**Drivers:** Lando Norris, Oscar Piastri
**Previous Season Constructor Standing:** P1 (666 pts)
**Notable Changes:** Stable driver line-up and regulations; no major 2025 technical reset.

#### Current Attributes

| Attribute                         | Score | Confidence | Basis |
| --------------------------------- | ----- | ---------- | ----- |
| `high_downforce_efficiency`       | 4.1   | high       | 2024 title-winning package strong in medium/high-speed corners. |
| `low_drag_straight_speed`         | 3.9   | high       | Competitive terminal speed across 2024 power tracks. |
| `mechanical_grip`                 | 4.0   | high       | Strong traction and rotation in low-speed sectors. |
| `reliability`                     | 3.7   | high       | Low mechanical retirement rate through 2024. |
| `pit_stop_consistency`            | 3.8   | high       | Generally fast and low-error pit execution in 2024. |
| `strategy_quality`                | 3.8   | med        | Improved tactical calls vs earlier seasons. |
| `upgrade_trajectory`              | 3.0   | med        | Neutral at initialization by framework rule. |
| `wet_weather_setup`               | 3.9   | med        | Competitive in mixed/wet weekends late 2024. |
| `tyre_degradation_characteristic` | 3.9   | high       | Usually strong long-run tyre control. |
| `dirty_air_sensitivity`           | 3.5   | med        | Better than average while following traffic. |
| `power_unit_performance`          | 3.1   | high       | Mercedes PU remained upper-grid in aggregate performance. |
| `cool_condition_performance`      | 3.7   | med        | Stable pace in low ambient conditions. |
| `hot_condition_performance`       | 3.8   | med        | Car showed broad operating window in heat. |

#### Changelog

| After Round                             | Attribute | Old | New | Reason |
| --------------------------------------- | --------- | --- | --- | ------ |
| R01 AustralianGrandPrix | `wet_weather_setup` | 3.7 | 3.9 | Norris win and Piastri front-running pace confirmed strong mixed-condition setup window. |
| R01 AustralianGrandPrix | `strategy_quality` | 3.7 | 3.8 | Lead car handled late crossover and final restart sequence cleanly. |

---

### Ferrari

**Power Unit:** Ferrari
**Drivers:** Charles Leclerc, Lewis Hamilton
**Previous Season Constructor Standing:** P2 (652 pts)
**Notable Changes:** Hamilton joined from Mercedes; stable regulations increase carry-over relevance.

#### Current Attributes

| Attribute                         | Score | Confidence | Basis |
| --------------------------------- | ----- | ---------- | ----- |
| `high_downforce_efficiency`       | 3.8   | high       | SF-24 baseline was strong on high-df tracks in 2024. |
| `low_drag_straight_speed`         | 3.7   | high       | Consistently competitive straight-line package in 2024. |
| `mechanical_grip`                 | 3.6   | high       | Good traction profile, especially in qualifying trim. |
| `reliability`                     | 3.5   | high       | Better reliability trend than early ground-effect era. |
| `pit_stop_consistency`            | 3.4   | med        | Mixed pit-stop pace and occasional operational errors. |
| `strategy_quality`                | 3.0   | med        | Tactically improved but still variable weekend to weekend. |
| `upgrade_trajectory`              | 3.0   | med        | Neutral at initialization by framework rule. |
| `wet_weather_setup`               | 3.2   | med        | Wet pace can fluctuate with setup window. |
| `tyre_degradation_characteristic` | 3.4   | med        | Usually solid tyre life but not class-leading everywhere. |
| `dirty_air_sensitivity`           | 3.3   | med        | Above-average following performance, still setup-sensitive. |
| `power_unit_performance`          | 3.1   | high       | Ferrari PU remained strong in deployment and top speed. |
| `cool_condition_performance`      | 3.5   | med        | Generally robust in cooler weekends. |
| `hot_condition_performance`       | 3.5   | med        | More stable than earlier years, still track-dependent. |

#### Changelog

| After Round                             | Attribute | Old | New | Reason |
| --------------------------------------- | --------- | --- | --- | ------ |
| R01 AustralianGrandPrix | `strategy_quality` | 3.1 | 3.0 | Ferrari converted P7/P8 starts only into P8/P10 in transition-heavy race. |
| R01 AustralianGrandPrix | `wet_weather_setup` | 3.3 | 3.2 | Lacked mixed-condition pace/conversion versus McLaren and Mercedes. |

---

### Red Bull Racing Honda RBPT

**Power Unit:** Honda RBPT
**Drivers:** Max Verstappen, Liam Lawson (R01-R02), Yuki Tsunoda (R03-R24)
**Previous Season Constructor Standing:** P3 (589 pts)
**Notable Changes:** Lawson started in second seat; Tsunoda promoted from Racing Bulls for R03 onward.

#### Current Attributes

| Attribute                         | Score | Confidence | Basis |
| --------------------------------- | ----- | ---------- | ----- |
| `high_downforce_efficiency`       | 3.8   | high       | 2024 car retained strong aero load generation. |
| `low_drag_straight_speed`         | 3.9   | high       | Strong speed-trap and efficiency profile in 2024. |
| `mechanical_grip`                 | 3.4   | med        | More variable than 2023 at low-speed venues. |
| `reliability`                     | 3.4   | med        | Slightly less bulletproof vs peak prior seasons. |
| `pit_stop_consistency`            | 4.0   | high       | Elite pit-stop execution remains team strength. |
| `strategy_quality`                | 3.7   | high       | Usually decisive and coherent race strategy. |
| `upgrade_trajectory`              | 3.0   | med        | Neutral at initialization by framework rule. |
| `wet_weather_setup`               | 3.6   | med        | Strong baseline in variable conditions. |
| `tyre_degradation_characteristic` | 3.4   | med        | Tyre management strong but no longer clear best. |
| `dirty_air_sensitivity`           | 3.2   | med        | Following performance not as dominant as 2023. |
| `power_unit_performance`          | 3.2   | high       | Honda RBPT package remained front-running. |
| `cool_condition_performance`      | 3.5   | med        | Solid all-weather baseline. |
| `hot_condition_performance`       | 3.7   | med        | Generally strong in higher track temperatures. |

#### Changelog

| After Round                             | Attribute | Old | New | Reason |
| --------------------------------------- | --------- | --- | --- | ------ |
| _(empty -- populated by weekend agents)_ |           |     |     |        |

---

### Mercedes

**Power Unit:** Mercedes
**Drivers:** George Russell, Kimi Antonelli
**Previous Season Constructor Standing:** P4 (468 pts)
**Notable Changes:** Hamilton departed; Antonelli debuted as rookie. Stable technical regulations.

#### Current Attributes

| Attribute                         | Score | Confidence | Basis |
| --------------------------------- | ----- | ---------- | ----- |
| `high_downforce_efficiency`       | 3.4   | med        | 2024 package improved but remained track-sensitive. |
| `low_drag_straight_speed`         | 3.4   | med        | Competitive but not consistently class-best. |
| `mechanical_grip`                 | 3.5   | med        | Good low-speed behaviour at several late-2024 rounds. |
| `reliability`                     | 3.7   | high       | Strong finishing reliability through 2024. |
| `pit_stop_consistency`            | 3.4   | med        | Mostly stable, occasional execution losses. |
| `strategy_quality`                | 3.6   | med        | Generally sound race management in 2024. |
| `upgrade_trajectory`              | 3.0   | med        | Neutral at initialization by framework rule. |
| `wet_weather_setup`               | 3.5   | med        | Wet pace depended heavily on setup window. |
| `tyre_degradation_characteristic` | 3.4   | med        | Usually around front-group average on long runs. |
| `dirty_air_sensitivity`           | 3.3   | med        | Some pace loss in traffic compared with leaders. |
| `power_unit_performance`          | 3.1   | high       | Mercedes PU remained upper-grid in output/recovery. |
| `cool_condition_performance`      | 3.7   | med        | Cooler events tended to suit Mercedes package. |
| `hot_condition_performance`       | 3.2   | med        | Heat management less consistent than best teams. |

#### Changelog

| After Round                             | Attribute | Old | New | Reason |
| --------------------------------------- | --------- | --- | --- | ------ |
| R01 AustralianGrandPrix | `strategy_quality` | 3.4 | 3.6 | Russell P3 and Antonelli P4 reflected strong transition-phase timing calls. |
| R01 AustralianGrandPrix | `wet_weather_setup` | 3.3 | 3.5 | Both cars remained competitive across wet/drying/wet transitions. |

---

### Aston Martin Aramco Mercedes

**Power Unit:** Mercedes
**Drivers:** Fernando Alonso, Lance Stroll
**Previous Season Constructor Standing:** P5 (94 pts)
**Notable Changes:** Driver line-up unchanged; 2024 decline sets conservative baseline.

#### Current Attributes

| Attribute                         | Score | Confidence | Basis |
| --------------------------------- | ----- | ---------- | ----- |
| `high_downforce_efficiency`       | 2.8   | med        | 2024 pace trended toward lower midfield over season. |
| `low_drag_straight_speed`         | 2.8   | med        | Straight-line package around midfield average. |
| `mechanical_grip`                 | 2.7   | med        | Mixed low-speed rotation and traction outcomes. |
| `reliability`                     | 3.1   | med        | Generally acceptable reliability profile. |
| `pit_stop_consistency`            | 3.0   | med        | Operations mostly clean with occasional time loss. |
| `strategy_quality`                | 2.7   | med        | Tactical calls broadly average in 2024. |
| `upgrade_trajectory`              | 3.0   | med        | Neutral at initialization by framework rule. |
| `wet_weather_setup`               | 2.8   | med        | No clear edge in wet scenarios recently. |
| `tyre_degradation_characteristic` | 2.6   | med        | Long-run tyre life often below top teams. |
| `dirty_air_sensitivity`           | 2.6   | med        | Car tended to lose more pace while following. |
| `power_unit_performance`          | 3.1   | high       | Mercedes PU remains a team strength. |
| `cool_condition_performance`      | 2.7   | med        | Performance variable in cool sessions. |
| `hot_condition_performance`       | 2.8   | med        | Slightly better in warmer races, still midfield. |

#### Changelog

| After Round                             | Attribute | Old | New | Reason |
| --------------------------------------- | --------- | --- | --- | ------ |
| _(empty -- populated by weekend agents)_ |           |     |     |        |

---

### Alpine Renault

**Power Unit:** Renault
**Drivers:** Pierre Gasly, Jack Doohan (R01-R06), Franco Colapinto (R07-R24)
**Previous Season Constructor Standing:** P6 (65 pts)
**Notable Changes:** Doohan started season; Colapinto replaced him from Emilia-Romagna weekend onward.

#### Current Attributes

| Attribute                         | Score | Confidence | Basis |
| --------------------------------- | ----- | ---------- | ----- |
| `high_downforce_efficiency`       | 2.6   | med        | 2024 aero competitiveness was lower-midfield. |
| `low_drag_straight_speed`         | 2.6   | med        | Lacked speed consistency on power-sensitive circuits. |
| `mechanical_grip`                 | 2.7   | med        | Reasonable low-speed balance on selected tracks. |
| `reliability`                     | 2.5   | med        | Reliability concerns persisted through 2024. |
| `pit_stop_consistency`            | 2.7   | med        | Pit execution close to midfield average. |
| `strategy_quality`                | 2.6   | med        | Tactical decisions sometimes reactive under pressure. |
| `upgrade_trajectory`              | 3.0   | med        | Neutral at initialization by framework rule. |
| `wet_weather_setup`               | 2.6   | low        | Wet baseline uncertain entering 2025. |
| `tyre_degradation_characteristic` | 2.6   | med        | Tyre life generally midfield-to-lower-midfield. |
| `dirty_air_sensitivity`           | 2.5   | med        | Pace drop in traffic frequently visible. |
| `power_unit_performance`          | 1.9   | high       | Renault PU output deficit remained notable. |
| `cool_condition_performance`      | 2.7   | low        | No strong consistent signal from 2024 data. |
| `hot_condition_performance`       | 2.7   | low        | Similar to cool conditions: broadly neutral baseline. |

#### Changelog

| After Round                             | Attribute | Old | New | Reason |
| --------------------------------------- | --------- | --- | --- | ------ |
| _(empty -- populated by weekend agents)_ |           |     |     |        |

---

### Haas Ferrari

**Power Unit:** Ferrari
**Drivers:** Esteban Ocon, Oliver Bearman
**Previous Season Constructor Standing:** P7 (58 pts)
**Notable Changes:** New line-up with Ocon and rookie Bearman.

#### Current Attributes

| Attribute                         | Score | Confidence | Basis |
| --------------------------------- | ----- | ---------- | ----- |
| `high_downforce_efficiency`       | 2.4   | med        | 2024 results indicate lower-midfield aero ceiling. |
| `low_drag_straight_speed`         | 2.9   | med        | Ferrari PU and low-drag setup helped on straights. |
| `mechanical_grip`                 | 2.4   | med        | Slow-speed traction remained inconsistent. |
| `reliability`                     | 2.7   | med        | Better reliability trend than 2023 baseline. |
| `pit_stop_consistency`            | 2.5   | med        | Operational execution still below top-midfield. |
| `strategy_quality`                | 2.4   | med        | Strategy variance higher than grid average. |
| `upgrade_trajectory`              | 3.0   | med        | Neutral at initialization by framework rule. |
| `wet_weather_setup`               | 2.4   | low        | Limited robust wet evidence at front-running pace. |
| `tyre_degradation_characteristic` | 2.6   | med        | Tyre overheating/wear remained common issue. |
| `dirty_air_sensitivity`           | 2.6   | med        | Car often struggled following closely. |
| `power_unit_performance`          | 3.1   | high       | Ferrari power unit is a relative team advantage. |
| `cool_condition_performance`      | 2.5   | low        | Conditions sensitivity remains uncertain. |
| `hot_condition_performance`       | 2.6   | low        | Slightly better than cool baseline, still limited. |

#### Changelog

| After Round                             | Attribute | Old | New | Reason |
| --------------------------------------- | --------- | --- | --- | ------ |
| _(empty -- populated by weekend agents)_ |           |     |     |        |

---

### Racing Bulls Honda RBPT

**Power Unit:** Honda RBPT
**Drivers:** Yuki Tsunoda (R01-R02), Liam Lawson (R03-R24), Isack Hadjar
**Previous Season Constructor Standing:** P8 (46 pts)
**Notable Changes:** Tsunoda promoted to Red Bull from R03; Lawson moved back to Racing Bulls from R03.

#### Current Attributes

| Attribute                         | Score | Confidence | Basis |
| --------------------------------- | ----- | ---------- | ----- |
| `high_downforce_efficiency`       | 2.7   | med        | Solid midfield aero package in 2024 comparison set. |
| `low_drag_straight_speed`         | 2.9   | med        | Competitive speed profile with Honda RBPT PU. |
| `mechanical_grip`                 | 2.7   | med        | Near-grid-average low-speed behaviour. |
| `reliability`                     | 2.8   | med        | Reliability generally acceptable in 2024. |
| `pit_stop_consistency`            | 2.7   | med        | Operationally around midfield mean. |
| `strategy_quality`                | 2.5   | med        | Strategy outcomes mixed but usually coherent. |
| `upgrade_trajectory`              | 3.0   | med        | Neutral at initialization by framework rule. |
| `wet_weather_setup`               | 2.6   | low        | Wet baseline uncertain with changing line-up context. |
| `tyre_degradation_characteristic` | 2.7   | med        | Tyre wear profile close to midfield average. |
| `dirty_air_sensitivity`           | 2.7   | med        | Moderate pace loss when following. |
| `power_unit_performance`          | 3.1   | high       | Honda RBPT PU remains above grid average. |
| `cool_condition_performance`      | 2.8   | low        | Limited robust trend signal in 2024 data. |
| `hot_condition_performance`       | 2.8   | low        | Broadly similar to cool-condition baseline. |

#### Changelog

| After Round                             | Attribute | Old | New | Reason |
| --------------------------------------- | --------- | --- | --- | ------ |
| R01 AustralianGrandPrix | `strategy_quality` | 2.7 | 2.5 | Tsunoda dropped from P5 to P12 through crossover timing loss; zero race laps for Hadjar. |
| R01 AustralianGrandPrix | `wet_weather_setup` | 2.8 | 2.6 | Team failed to convert strong qualifying positions in mixed-race conditions. |

---

### Williams Mercedes

**Power Unit:** Mercedes
**Drivers:** Carlos Sainz, Alexander Albon
**Previous Season Constructor Standing:** P9 (17 pts)
**Notable Changes:** Sainz joined from Ferrari; team still in lower-midfield baseline from 2024 points.

#### Current Attributes

| Attribute                         | Score | Confidence | Basis |
| --------------------------------- | ----- | ---------- | ----- |
| `high_downforce_efficiency`       | 2.6   | med        | 2024 package struggled more on high-load tracks. |
| `low_drag_straight_speed`         | 3.1   | med        | Straight-line efficiency remained key strength. |
| `mechanical_grip`                 | 2.6   | med        | Low-speed rotation/traction often limited. |
| `reliability`                     | 2.7   | med        | Reliability was serviceable but not standout. |
| `pit_stop_consistency`            | 2.4   | med        | Pit operations frequently lost small margins. |
| `strategy_quality`                | 2.7   | med        | Strategy execution generally below top-midfield. |
| `upgrade_trajectory`              | 3.0   | med        | Neutral at initialization by framework rule. |
| `wet_weather_setup`               | 2.8   | low        | Wet pace highly variable by circuit. |
| `tyre_degradation_characteristic` | 2.5   | med        | Tyre wear tended to be above midfield average. |
| `dirty_air_sensitivity`           | 2.5   | med        | Following another car significantly hurt lap time. |
| `power_unit_performance`          | 3.1   | high       | Mercedes PU is clear positive vs chassis baseline. |
| `cool_condition_performance`      | 2.6   | low        | Limited stable signal entering 2025. |
| `hot_condition_performance`       | 2.5   | low        | Similar uncertainty, slightly better in some hot rounds. |

#### Changelog

| After Round                             | Attribute | Old | New | Reason |
| --------------------------------------- | --------- | --- | --- | ------ |
| R01 AustralianGrandPrix | `wet_weather_setup` | 2.6 | 2.8 | Albon converted mixed conditions into P5 despite repeated disruption phases. |
| R01 AustralianGrandPrix | `strategy_quality` | 2.5 | 2.7 | Strong Albon race execution and timing in crossover windows delivered high-value points. |
| R01 AustralianGrandPrix | `cool_condition_performance` | 2.4 | 2.6 | Competitive race pace at 16-17°C ambient outperformed prior baseline. |

---

### Kick Sauber Ferrari

**Power Unit:** Ferrari
**Drivers:** Nico Hulkenberg, Gabriel Bortoleto
**Previous Season Constructor Standing:** P10 (4 pts)
**Notable Changes:** New line-up with Hulkenberg from Haas and rookie Bortoleto; Audi transition phase.

#### Current Attributes

| Attribute                         | Score | Confidence | Basis |
| --------------------------------- | ----- | ---------- | ----- |
| `high_downforce_efficiency`       | 2.4   | med        | 2024 team baseline was back-of-grid in downforce tracks. |
| `low_drag_straight_speed`         | 2.5   | med        | Better on straights than in corners, still below average. |
| `mechanical_grip`                 | 2.4   | med        | Persistent low-speed weakness in 2024 reference data. |
| `reliability`                     | 2.5   | med        | Reliability not catastrophic, but below midfield standard. |
| `pit_stop_consistency`            | 2.6   | med        | Operational consistency remained weaker than peers. |
| `strategy_quality`                | 2.5   | med        | Tactical outcomes often constrained by starting position. |
| `upgrade_trajectory`              | 3.0   | med        | Neutral at initialization by framework rule. |
| `wet_weather_setup`               | 2.7   | low        | Sparse strong wet data, baseline kept conservative. |
| `tyre_degradation_characteristic` | 2.6   | med        | Tyre wear generally above grid average. |
| `dirty_air_sensitivity`           | 2.4   | med        | High pace loss in turbulent air. |
| `power_unit_performance`          | 3.0   | high       | Ferrari PU mitigates some chassis deficits. |
| `cool_condition_performance`      | 2.4   | low        | Limited high-confidence signal entering season. |
| `hot_condition_performance`       | 2.6   | low        | Slightly weaker trend in hot races vs cool races. |

#### Changelog

| After Round                             | Attribute | Old | New | Reason |
| --------------------------------------- | --------- | --- | --- | ------ |
| R01 AustralianGrandPrix | `wet_weather_setup` | 2.6 | 2.7 | Hulkenberg advanced P17 to P7 in mixed conditions, indicating improved wet operability. |

---

## Source Notes

- 2024 constructor standings and points from Formula1.com official results page.
- 2025 driver movements from official Formula1.com 2025 line-up and driver-change articles.
- Sprint weekend and mid-season swap context from FIA/Formula1.com announcements.
- Car attribute scores are calibrated initialization estimates using 2024 results trend + known team changes (not race-by-race telemetry models).

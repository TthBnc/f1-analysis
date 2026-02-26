# F1 Analytical Framework — Attribute System

## Overview

This framework defines the scoring attributes used to rate cars, drivers, and circuits across the 2021–2025 F1 seasons. All attributes are scored on a **1–10 scale** (10 = elite) unless otherwise noted. Scores are cumulative and evolve race-by-race via delta updates (e.g., "+1", "-0.5").

---

## 1. Car (Constructor) Attributes

### Aerodynamic Performance
| Attribute | Description |
|-----------|-------------|
| `straight_line_speed` | Top speed and speed trap performance; raw power + drag balance |
| `cornering_downforce` | Mechanical + aero grip through medium/high-speed corners |
| `low_speed_traction` | Grip and stability in slow-speed corners (hairpins, chicanes) |
| `high_speed_stability` | Rear-end confidence at 250+ km/h; resistance to snap oversteer |
| `aero_efficiency` | Downforce-to-drag ratio; ability to be fast on straights AND corners |
| `drs_effectiveness` | Delta gained from DRS activation relative to field average |
| `ground_effect_performance` | Floor-generated downforce consistency; sensitivity to ride height changes |

### Mechanical Performance
| Attribute | Description |
|-----------|-------------|
| `mechanical_grip` | Grip from suspension geometry, weight distribution, tire contact patch |
| `brake_stability` | Consistency and confidence under heavy braking; resistance to lock-ups |
| `ride_quality` | Ability to handle bumps, curbs, and uneven surfaces without losing grip |
| `tire_degradation_management` | How gently the car treats tires over a stint |
| `cooling_efficiency` | Thermal management of brakes, PU, and tires in hot conditions |

### Power Unit
| Attribute | Description |
|-----------|-------------|
| `pu_performance` | Raw power output; acceleration zones and deployment |
| `pu_reliability` | Freedom from mechanical/electrical failures |
| `energy_deployment` | Hybrid system efficiency; harvesting and deployment strategy |
| `high_altitude_pu_efficiency` | PU performance at altitude (Mexico City, Interlagos) — turbo and ICE |

### Adaptability
| Attribute | Description |
|-----------|-------------|
| `wet_weather_balance` | Car balance and predictability in wet/mixed conditions |
| `setup_window` | How easily the car can be tuned for different circuit types |
| `development_rate` | In-season upgrade effectiveness and trajectory |
| `sprint_format_adaptability` | Performance in parc fermé conditions with limited setup changes |

---

## 2. Driver Attributes

### Speed
| Attribute | Description |
|-----------|-------------|
| `qualifying_pace` | Raw one-lap speed; ability to extract maximum from the car |
| `race_pace` | Long-run consistency and speed over a full race distance |
| `wet_weather_prowess` | Skill and confidence in rain/mixed conditions |

### Racecraft
| Attribute | Description |
|-----------|-------------|
| `overtaking_ability` | Wheel-to-wheel aggression and execution on attack |
| `defensive_driving` | Ability to hold position under pressure without contact |
| `race_craft` | General race intelligence; positioning, timing of moves |
| `starts_and_launches` | Reaction time and first-lap positioning |
| `track_position_management` | Ability to create/maintain gaps; undercut/overcut awareness |

### Mental & Consistency
| Attribute | Description |
|-----------|-------------|
| `consistency` | Lap-to-lap variation; freedom from unforced errors |
| `mental_resilience` | Performance under pressure, after setbacks, in championship fights |
| `error_rate` | Frequency of mistakes (spins, crashes, penalties) — INVERSE: lower = better |
| `clutch_performance` | Ability to deliver when it matters most (final laps, title deciders) |

### Technical
| Attribute | Description |
|-----------|-------------|
| `tire_management` | Ability to extend stints and preserve tire performance |
| `strategic_adaptability` | How well the driver adjusts to changing race strategies mid-race |
| `feedback_and_development` | Quality of technical feedback; contribution to car development |
| `fuel_and_energy_management` | Efficiency in managing fuel load and hybrid deployment |

### Situational (Unlocked dynamically)
| Attribute | Description |
|-----------|-------------|
| `recovery_drive_ability` | Performance when starting out of position or recovering from incidents |
| `team_leadership` | Influence on team morale and strategic decisions |
| `inter_team_battle` | Head-to-head performance vs. teammate |

---

## 3. Circuit Attributes

### Physical Characteristics
| Attribute | Description |
|-----------|-------------|
| `track_type` | `street` / `permanent` / `hybrid` / `oval-inspired` |
| `track_length_km` | Lap distance in kilometers |
| `number_of_corners` | Total corner count |
| `number_of_drs_zones` | DRS zones available |

### Performance Demands
| Attribute | Description |
|-----------|-------------|
| `downforce_demand` | How much downforce is rewarded (`low` / `medium` / `high`) |
| `power_sensitivity` | How much straight-line speed matters (`low` / `medium` / `high`) |
| `tire_severity` | Degradation level (`low` / `medium` / `high` / `extreme`) |
| `brake_demand` | Braking intensity and frequency (`low` / `medium` / `high`) |

### Racing Factors
| Attribute | Description |
|-----------|-------------|
| `overtaking_difficulty` | How hard it is to pass (`easy` / `medium` / `hard` / `very_hard`) |
| `safety_car_probability` | Likelihood of SC/VSC (`low` / `medium` / `high`) |
| `pit_stop_time_loss` | Seconds lost per pit stop (affects strategy) |
| `track_evolution_rate` | How much grip improves across a session (`low` / `medium` / `high`) |

### Environmental
| Attribute | Description |
|-----------|-------------|
| `weather_variability` | Chance of rain/changeable conditions (`low` / `medium` / `high`) |
| `altitude_m` | Track altitude in meters (affects PU performance) |
| `night_race` | `true` / `false` — affects track temperature and grip |
| `abrasive_surface` | Surface roughness (`low` / `medium` / `high`) |

---

## 4. Scoring Protocol

### Initial Baselines
- At the start of the 2025 analysis, all entities start with **baseline scores** informed by pre-season expectations and historical data.
- Baseline scores are set in `analysis/2025/00-baselines.md`.

### Delta Updates
- Each session file contains an **Attribute Point Updates** section.
- Deltas are expressed as `+X` or `-X` relative to the entity's current score.
- Example: `Max Verstappen: wet_weather_prowess +1 (masterclass in Brazil rain)`

### Cumulative Tracking
- Running totals are maintained in season summary files: `analysis/YYYY/season-summary.md`
- These are updated periodically (every 4-5 races) to checkpoint the attribute evolution.

### New Attribute Discovery
- Sub-agents can propose new attributes when they identify unique performance factors.
- New attributes are flagged with `[NEW ATTRIBUTE]` and integrated into this framework.
- Example: A sub-agent analyzing Monaco might propose `narrow_street_spatial_awareness`.

---

## 5. Predictive Modeling Schema

The attribute data is structured to support "What-If" scenarios:

```
P(success) = f(driver_attributes, car_attributes, circuit_attributes, form_vector)
```

Where:
- `form_vector` = recent 3-race rolling average of performance deltas
- `circuit_match` = correlation between car/driver strengths and circuit demands
- `historical_affinity` = past performance at the specific circuit

This enables queries like:
- "What is Verstappen's probability of pole at Spa given Red Bull's current aero efficiency?"
- "If it rains at Silverstone, which driver has the highest expected finish?"

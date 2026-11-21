# Muscle Fatigue During Effort and Rest

Final project for **Master IEAP, Mathematical Modeling** (Group C).
We study a two-variable model of the balance between fatigue and recovery during sustained exercise such as stationary cycling.

> The parameter values are illustrative and not fitted to an athlete. `F` is not muscle force, `R` is not recovery time, and `P` is not power in watts.

## The model

```
dF/dt = alpha * P * (1 - F) - beta * F * R
dR/dt = gamma * (1 - R) - delta * F * R - epsilon * P * R
```

| Symbol | Meaning | Value |
|---|---|---|
| `F` in [0, 1] | normalised fatigue (0 = no fatigue) | state variable |
| `R` in [0, 1] | normalised recovery capacity (1 = full capacity) | state variable |
| `P >= 0` | dimensionless effort intensity | prescribed (1 and 1.6) |
| alpha | rate of fatigue build-up | 0.60 min^-1 |
| beta | fatigue removal through recovery | 0.80 min^-1 |
| gamma | natural regeneration of recovery capacity | 0.30 min^-1 |
| delta | recovery loss caused by fatigue | 0.25 min^-1 |
| epsilon | recovery loss caused by effort | 0.15 min^-1 |

Time is in minutes.

## Repository structure

```
muscle-fatigue-model/
├── README.md
├── .gitignore
├── main.ipynb                        # Main notebook with all sections
├── report/                           # final report 
```
## Team

| Name | Section(s) |
|---|---|
| Shunan | section 1 |
| Ayesha | section 2 |
| Batoul | section 3 |
| Shunan | section 4 |

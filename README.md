# Dataset schema

The analysis expects a file at `data/olympia2016_athletes.csv` with 11,538 rows
(one row per athlete) and these columns:

| Column | Type | Meaning |
|---|---|---|
| `id` | integer | unique athlete id |
| `name` | text | athlete name |
| `nationality` | text | three-letter country code (`USA`, `GER`, ...) |
| `sex` | text | `male` / `female` |
| `dob` | text | date of birth, e.g. `10/17/69` |
| `height` | float | height in metres |
| `weight` | float | weight in kilograms |
| `sport` | text | sport the athlete competed in |
| `gold` | integer | gold medals recorded for this athlete |
| `silver` | integer | silver medals recorded for this athlete |
| `bronze` | integer | bronze medals recorded for this athlete |

The raw file is not committed to this repository: it was distributed as course
material for CISC7204 Tutorial 09 and is not redistributed here. Drop your copy
into this folder and the notebook will run unchanged.

Note that the medal columns are **athlete-level**: a team gold is recorded once
for every member of the squad, not once per event.

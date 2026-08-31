# Crane School — educational cache

Teaching library for three attached programs:

1. **Red Seal Tower Crane Operator** (SkilledTradesBC 2024, 175 h L1 + 140 h L2)
2. **Mobile RT** (rough-terrain hydraulic; Fulford MH80 / SkilledTradesBC mobile competencies)
3. **Rigging** (Fulford L1 / L2 / load turning; required for BC Crane Safety provisional)

This is course material only. Drop decks in `lesson/`, stills in `slides/`, tests in `assessments/`. Empty folders are placeholders for lessons the program still needs.

Sources used to build the tree: [Red Seal Tower Crane RSOS 2023](https://red-seal.ca/eng/trades/towercrane_op/overview.shtml), [SkilledTradesBC TCO 2024](https://skilledtradesbc.ca/tower-crane-operator) (OPSN 2024 018), [BC Crane Safety](https://bccranesafety.ca/), [Fulford](https://fulford.ca/), [WorkSafeBC OHSR Part 14 / 15](https://www.worksafebc.com/), [NCCCO/CCO](https://www.nccco.org/) tower exam domains.

---

## How BC certification actually works

| Step | Who | What this library covers |
|---|---|---|
| Rigging theory (required to apply) | Fulford L1 or equivalent | `03-rigging/L1-fundamentals/` |
| Provisional (Level B) | BC Crane Safety + Fulford 40-question exam | `00-shared-core/00-provisional-theory/` |
| Tower L1 / L2 technical training | SkilledTradesBC 2024 outline | `01-tower-crane/L1/` and `L2/` |
| Tower practical | Fulford: 10-q load chart & rigging (8 chart + 2 rigging, pass 7/10) + signals + on-crane | `01-tower-crane/exams/fulford-practical/` |
| Red Seal IP exam | 100 questions: A 11 / B 21 / C 23 / D 17 / E 28 | `01-tower-crane/exams/red-seal-ip/` |
| Mobile RT ticket | Typically MH80 (hydraulic ≤80 t, includes RT) | `02-mobile-rt/` |

Hours (tower): **2,685** work-based, including **1,000 rigging** and **1,000 operating** a mast ≥ 90 ft. Tower Crane becomes a compulsory Skilled Trades Certification trade on **5 July 2027**.

---

## Folder map

```
00-shared-core/     signals, powerlines, WorkSafeBC, provisional theory
01-tower-crane/     Red Seal / SkilledTradesBC TCO L1 + L2
02-mobile-rt/       RT hydraulic program + MH80 practical
03-rigging/         Fulford L1, L2, load turning, inspector
04-reference/       manufacturer charts, photos, downloaded standards
```

Shared lessons live in `00-shared-core/` so tower, RT, and rigging do not duplicate the same deck. Tower `A1–A5` folders are still there so they match the SkilledTradesBC exam breakdown — put tower-specific examples there, and point at shared-core for the common lesson.

---

## 01 Tower Crane — lessons required

Codes match **SkilledTradesBC Tower Crane Operator (2024)** and Red Seal MWAs.

### Level 1 (175 hours)

| Folder | Lesson | Why |
|---|---|---|
| `A1` | Regulations, policies, manuals | WorkSafeBC, CSA Z248, manufacturer manuals |
| `A2` | Safe work environment | Site hazards, exclusion zones, no loads over people |
| `A3` | Emergency procedures | Shutdown, rescue, two-blocking, malfunction |
| `A4` | Energized systems / limits of approach | OHSR powerline tables |
| `A5` | Communications | Hand signals, radio, who is in charge of the lift |
| `B1` | Crane types | Hammerhead, luffing, self-erect |
| `B2` | Terminology | Mast, jib, trolley, slewing, reeving, radius |
| `C1–C4` | Systems | Structure, support/ties, rail travel, cab/safety/access |
| `D1–D4` | Rigging (basic) | Teach from `03-rigging/L1`; tower D4 = rig a basic load |
| `E1` | Load weights | Volume × density, COG, hook + rigging deductions |
| `E2/hammerhead` | Capacity charts | **Existing course.** Fulford rounding: next longer radius. CCO Domain “Manufacturers’ Load Charts” (~25%) |
| `F1–F5` | Inspection & maintenance | Pre-op, logbook, wire rope rejection |
| `G1` | Ordinary lift planning | Site, radius, net vs gross, signaller |
| `H1–H4` | Operate & secure | Manuals, trolley/slew/hoist, wind (WorkSafeBC 50 km/h + anemometer), weathervane |
| `J1` intro | Personnel platform awareness | Critical lift; 50% capacity; 10:1 rigging |

### Level 2 (140 hours)

| Folder | Lesson | Why |
|---|---|---|
| `A5` advanced | Mentoring / worksite communication | New in 2023 RSOS |
| `D4` | Non-symmetrical rigging | STBC L2: calculate and install on an offset load |
| `E1` | Complex load weights | Combined shapes, COG |
| `E2/luffing` | Luffing charts | **Existing course.** Boom angle + radius, not trolley |
| `F4` | Advanced pre-op | After climb / reconfigure |
| `G2` | Engineered & critical lifts | OHSR 14.42 / 14.42.1 written plan |
| `H2` | Advanced operations | Simultaneous functions, multi-crane site |
| `I1–I2` + `climbing-course` | Bottom / top climbing | **Existing C-7 course.** No production lifts during climb |
| `I3` | Reconfiguration | Jib length, counterweight, ties |
| `I4` | Self-erect assembly & transport | Own BC Crane Safety class |
| `J1–J3` | Manbasket, engineered lifts, tandem | OHSR 13.27, 14.42 |

### Exams to write material for

- SLE L1 and L2 (70%, no code book)
- Red Seal IP (100 questions)
- Fulford practical: 10-q chart/rigging exam, hand signals, pre-op, setup, operation

---

## 02 Mobile RT — lessons required

RT is a **telescopic hydraulic** mobile crane. In BC the usual ticket that covers jobsite RTs is **Mobile Hydraulic 80 t and under** (Fulford practical + SkilledTradesBC). Red Seal Mobile Crane Operator includes RT as a crane type.

### Core (from SkilledTradesBC Mobile Crane outline)

Safety, communications, types, hydraulic systems, rigging, load weights, **telescoping boom charts**, pre-op, ordinary + critical lift plans, outrigger setup, operations, secure, transport, assemble (counterweight / swing-away jib).

### RT-specific (must exist; not in the tower program)

| Folder | Lesson |
|---|---|
| `pick-and-carry` | On rubber vs on outriggers; chart notes |
| `quadrants-of-operation` | Over front / rear / side capacity |
| `range-diagrams` | Boom length × angle → radius |
| `ground-bearing-and-mats` | Float size, soil, outrigger load |
| `steering-modes-4ws-crab` | 2WS / 4WS / crab |
| `lmi-rci-anti-two-block` | Bypass rules, setup configuration |
| `travel-on-rubber-vs-outriggers` | When the chart allows travel |

### Fulford MH80 practical to prep

Hand signals → 60-minute load chart & rigging exam → pre-op (incl. rigging inspection, bring OHSR) → setup & hazards (pads/outriggers) → nine empty-hook targets + nine with load, boom ≥ 75% extended.

---

## 03 Rigging — lessons required

BC Crane Safety: **proof of rigging theory is required for provisional**. Tower Red Seal MWA D is **17%** of the IP exam. Fulford tower practical includes **two rigging-chart questions**.

| Block | Lessons |
|---|---|
| **L1 Fundamentals** (Fulford, ~8 h + assessment, 5-year card) | Signals, load weight, COG, hardware, inspection/rejection, sling charts & hitches, sling angle, storage, crane-side hazards, lift-plan awareness |
| **L2 Advanced** | Complex weights, combined COG, symmetrical tension, off-centre / unequal-height, spreader bars / beams / plate clamps, manbasket rigging, limits of approach |
| **Load turning & drifting** | Separate Fulford course |
| **Inspector** (optional) | ASME periodic inspection of slings, hardware, bars; designated person |

Put reusable sling tables in `03-rigging/charts-and-tables/`.

---

## 04 Reference

Manufacturer load charts used in class live under `datasheets/`. Drop downloaded PDFs of RSOS, STBC outlines, WorkSafeBC excerpts, Fulford guides, CSA Z150/Z248, ASME B30, and NCCCO/CCO outlines into `standards/`.

CCO tower written exam (55 q, 60 min) is **not** a BC ticket, but its four domains — Site, Operations, Technical Knowledge, Manufacturers’ Load Charts — are a useful check that a lesson is missing.

---

## What is already in the cache

- `01-tower-crane/L1/.../E2-capacity-charts/hammerhead/` — load-chart lesson + Liebherr / Potain / Terex tests
- `01-tower-crane/L2/.../E2-capacity-charts-advanced/luffing/` — luffing deck
- `01-tower-crane/L2/.../climbing-course/` — C-7 climbing deck, test, stills
- `04-reference/datasheets/` — Liebherr, Potain, Terex PDFs

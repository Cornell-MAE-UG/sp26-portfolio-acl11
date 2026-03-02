---
title: "Macadamia Nutcracker Design (HW4 Additional 2) -- ACL245"
excerpt: "Lever-based nutcracker sized for an average user and optionally actuated with a small linear actuator."
collection: projects
image: /assets/images/nutcracker-design.png
---

## Problem Statement (Find)
Design a feasible, useful nutcracker and determine key dimensions so an average user can crack an average macadamia nut.

## Constraints & Inputs (Given)
- Average required cracking load (macadamia): **225 kg** (https://doi.org/10.1007/s10071-007-0131-2)
- Average nut geometry: **~15 mm diameter, spherical** (https://www.worldmacadamia.com/style-guide/)
- Average grip strength: **49.7 kg** (https://doi.org/10.1016/j.jshs.2024.101014)
- Design grip force used: **33 kg** (chosen to be significantly less than maximum effort)

## Approach
1. Model the tool as a simple lever mechanism about the hinge.
2. Write a moment balance to relate user grip force to nut-cracking force.
3. Choose a reasonable handle length and solve for the required jaw lever arm.
4. Use similarity/geometry relationships from the sketch to estimate jaw opening / hand spacing.

## Calculations (Key Results)
- Moment balance: L1 * F_nut = L2 * F_gp
- Choose handle length: L2 = 200 mm
- Solve: L1 = (F_gp / F_nut) * L2 = (33 / 225) * 200 ≈ 29.3 mm
- Confirm resulting grip spacing is within average users’ hand width (<150 mm)


## Diagram
![Nutcracker diagram]({{ "/assets/images/nutcracker-design.png" | relative_url }})

## Usability Discussion
- The selected grip force (33 kg) is about **2/3 of average max**, making the action achievable without full-effort squeezing.
- The chosen handle length (200 mm) supports comfortable leverage and reasonable hand positioning.
- The jaw opening / grip spacing is sized to feel natural for a typical hand.

## Optional Actuation Concept (Linear Actuator)
A compact linear actuator can replace the hand-applied grip force if it can supply ~**72 lbf** over ~**1.34 in** stroke (based on the stroke and force targets from the design). The IP65 Mini Linear Actuator meet these requirements; the most aligned variant of this actuator would have a 2-inch stroke and a 112-pound force capacity. (https://www.progressiveautomations.com/products/pa-01?variant=43088662364340)

![Linear Actuator based nutcracker design]({{ "/assets/images/LA-nutcracker-design.png" | relative_url }})

## Credits / Sources
- Macademia nut specifications: (https://doi.org/10.1007/s10071-007-0131-2)
- Average nut geometry: (https://www.worldmacadamia.com/style-guide/)
- Average grip strength: (https://doi.org/10.1016/j.jshs.2024.101014)
- Linear Actuator: (https://www.progressiveautomations.com/products/pa-01?variant=43088662364340)
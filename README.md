# Tinashe Nedi — Solar & Energy Storage API Engineer

**Building the engineering infrastructure behind commercial solar, BESS, and BIPV analysis.**  
Every API I ship cites its source. No black boxes. No estimates without a named reference.

---

## What I Build

I develop **physics-based energy APIs** used by solar developers, energy consultants, ESCOs, and building compliance teams. Every calculation traces to a peer-reviewed paper, government dataset, or regulatory document — the same sources used by licensed engineers and financial underwriters.

**Live on RapidAPI → [rapidapi.com/user/bethelnedi](https://rapidapi.com/user/bethelnedi)**  
**Web tools → [solartruth.app](https://solartruth.app)**

---

## API Stack

| API | What it does | Standard / Source |
|-----|-------------|-------------------|
| [Solar + BESS Sizing API](https://rapidapi.com/bethelnedi/api/solar-bess-sizing-dispatch-optimization-api/playground/apiendpoint_6c8f05e9-0200-4078-9027-d36f4538ab61) | Commercial battery storage sizing, CAPEX, LCOS, NPV, IRR | NREL ATB 2024, PNNL-33283, IRA 2022 §48E |
| [BIPV Energy Yield API](https://rapidapi.com/bethelnedi/api/bipv-energy-yield-api/playground/apiendpoint_5eaaaf3d-592f-47df-99e3-a9fcdcd495d3) | Facade & rooftop PV yield, NASA POWER irradiance, LCOE | IEC 61724-1:2021, HDKR model, IEA PVPS Task 15 |
| [BIPV Structural Load API](https://rapidapi.com/bethelnedi/api/bipv-structural-load-api/playground/apiendpoint_a2bff55d-337c-4607-b765-4d8553a3692c) | Wind loads, bracket forces, ULS/SLS for facade PV | EN 1991-1-4:2005, ASCE 7-22, EN 1990:2002 |
| [Rooftop Solar Suitability API](#) | Building detection from lat/lng, usable area, solar score | OSM, NREL/TP-6A20-65298, IFC 2021 §1504.3 |
| [Solar O&M Performance API](https://rapidapi.com/bethelnedi/api/solar-o-m-performance-monitoring-api/playground/apiendpoint_9be8516f-e069-4f08-8222-c930e7c41a79) | IEC weather-corrected PR, fault diagnosis, revenue loss | IEC 61724-1:2021, Jordan & Kurtz 2013 |
| [Energy Audit Automation API](https://rapidapi.com/bethelnedi/api/energy-audit-automation-api/playground/apiendpoint_cbd5065f-a500-497b-9947-34c25bafbfdf) | EUI vs EPA median, LL97/BERDO/Denver BPS penalties | EPA ENERGY STAR, NYC LL97, ASHRAE 90.1 |
| [Residential Solar ROI API](https://rapidapi.com/bethelnedi/api/residential-solar-roi-api/playground/apiendpoint_42f4767b-fc03-4cae-b84c-fbb813b7cc29) | PVWatts V8, NASA POWER, NEM 3.0, 25-yr cashflow | NREL/TP-6A20-62641, DSIRE 2024, IRA 2022 |
| [Solar + EV Integration API](https://rapidapi.com/bethelnedi/api/solar-ev-integration-sizing-api/playground/apiendpoint_b338efee-3ca1-4b22-bb65-780e0186836c) | Solar+EV co-sizing, TOU arbitrage, V2H assessment | EPA fueleconomy.gov, NREL Solar+EV 2023 |
| [Solar Incentive Intelligence API](https://rapidapi.com/bethelnedi/api/solar-incentive-intelligence-api/playground/apiendpoint_b56c68a1-7545-4459-9acc-cebf9878b5ac) | IRA bonus adder stack, SREC markets, interconnection | IRS Notice 2023-29, IRS Notice 2023-38 |

---

## The Engineering Difference

Most solar calculators use rules of thumb. My APIs implement published models:

- **CAPEX**: NREL ATB 2024 two-component formula `[pack($/kWh) × duration] + BOS($/kW)` — not a flat $/kWh guess
- **Yield**: HDKR irradiance transposition (Reindl, Beckman & Duffie 1990), Sandia cell temperature model (King et al. 2004)
- **Performance Ratio**: IEC 61724-1:2021 §8.2 weather-corrected PR — removes seasonal temperature bias
- **Degradation**: Jordan & Kurtz (2013) median rates by module technology
- **Structural loads**: EN 1991-1-4:2005 Eq.(4.8), Miller & Kopp (2024) air permeability correction
- **Compliance**: NYC 1 RCNY §103-14, Boston BERDO 2.0 §7-2.2, Denver Municipal Code §§4-38

Every API response includes the equation used, the source it cites, and the confidence range. Energy consultants can put their stamp on these outputs.

---

## Tech Stack

![Python](https://img.shields.io/badge/Python-3.11-blue?style=flat-square&logo=python)
![FastAPI](https://img.shields.io/badge/FastAPI-0.111-009688?style=flat-square&logo=fastapi)
![Pydantic](https://img.shields.io/badge/Pydantic-v2-E92063?style=flat-square)
![Hugging Face](https://img.shields.io/badge/Hosted_on-Hugging_Face-FFD21E?style=flat-square&logo=huggingface)
![RapidAPI](https://img.shields.io/badge/Monetized_via-RapidAPI-0055DA?style=flat-square)

---

## Domain Keywords

`solar-api` `bess-sizing` `battery-storage` `bipv` `energy-yield` `pvwatts` `nrel` `iec-61724` `energy-audit` `building-performance-standards` `ll97` `ashrae` `ira-2022` `investment-tax-credit` `solar-roi` `demand-charge` `lcos` `npv-irr` `commercial-solar` `rooftop-detection` `openstreetmap` `nasa-power` `nem-policy` `solar-incentives` `srec` `ev-charging` `solar-ev` `fastapi` `python`

---

## Connect

- **RapidAPI**: [rapidapi.com/user/bethelnedi](https://rapidapi.com/user/bethelnedi)
- **Email**: support@solartruth.app
- **Web**: [solartruth-platform.vercel.app](https://solartruth-platform.vercel.app)

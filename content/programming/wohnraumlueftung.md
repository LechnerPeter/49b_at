+++
title = 'Decentralized Ventilation'
date = 2026-06-28T00:00:00+02:00
draft = false
image = '/images/wohnraumlueftung.svg'
+++

## Goals

- **Replicate original behaviour** — 50/50 on and off, reversing direction every minute
- **Finer control** than the 4 factory speed levels
- **Ventilate individual rooms** — all but one fan running in the same direction
- **Extractor fan booster** — all fans blowing inward (only works with an extractor that vents to the outside)
- **Silent ventilation** for individual rooms (e.g. bedroom) — one fan off, all others running in the same direction
- **Higher maximum number of fans**
- **Easier integration with Home Assistant**

---

Controlling the Buderus decentralized ventilation unit with a Shelly for more flexibility.\
 The fan has 3 pins: +, − and PWM. The PWM signal behaves as follows:

| Voltage | Behaviour |
|---|---|
| 0 V | 100 % reverse |
| 2.5 V | standstill |
| 5 V | 100 % forward |

## Materials

- Shelly Dimmer 0/1–10V PM Gen3 *(not the Shelly Dimmer or the Shelly RGBW)*
- 230V AC to 12V DC 1A transformer
- Buderus Logavent HRV126-43 D complete set
- 2× Wago 3-way terminal block

## Wiring

![Wiring diagram](/images/wohnraumlueftung-wiring.svg)

<small>*Diagram is AI-generated.*</small>

### 230V

- 230V N → Wago1
- 230V L → Dimmer L
- Wago1 → Dimmer N
- Wago1 → Transformer N
- Dimmer O → Transformer L *(allows cutting power to the transformer via the Shelly)*

### 12V

- Dimmer − → Wago2
- Wago2 → Transformer −
- Wago2 → Fan −
- Dimmer + → Fan PWM
- Transformer + → Fan +

<img src="/images/ShellyVentilator.jpg" alt="Shelly Ventilator Wiring" style="max-width: 400px; border-radius: 8px;">

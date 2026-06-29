+++
title = 'Dezentrale Wohnraumlüftung'
date = 2026-06-28T00:00:00+02:00
draft = false
image = '/images/wohnraumlueftung.svg'
+++

## Ziele

- **Originalverhalten duplizieren** — 50/50 ein und aus, wechseln alle Minute die Richtung
- **Genauere Einstellung** als die 4 Werkstufen
- **Einzelne Räume lüften** — alle bis auf einen Lüfter in die gleiche Richtung
- **Dunstabzug-Booster** — alle Lüfter nach innen (funktioniert nur bei einem Dunstabzug, der ins Freie geht)
- **Lautloses Lüften** einzelner Räume (z. B. Schlafzimmer) — ein Lüfter aus, alle anderen gleichgerichtet
- **Höhere maximale Anzahl an Lüftern**
- **Einfachere Integration mit Home Assistant**

---

Ansteuerung des Buderus dezentralen Wohnraumlüfters mit Shelly um mehr Flexibilität zu haben. \
Der Ventilator hat 3 Pins +, - und PWM, wobei das PWM-Signal wie folgt verhält:

| Spannung | Verhalten |
|---|---|
| 0 V | 100 % Rückwärts |
| 2,5 V | Stillstand |
| 5 V | 100 % Vorwärts |

## Material

- Shelly Dimmer 0/1–10V PM Gen3 *(nicht der Shelly Dimmer oder der Shelly RGBW)*
- 230V AC auf 12V DC 1A Trafo
- Buderus Logavent HRV126-43 D Komplettset
- 2× Wago 3er Klemme

## Verkabelung

![Verkabelungsdiagramm](/images/wohnraumlueftung-wiring.svg)

<small>*Diagramm ist KI-generiert.*</small>

### 230V

- 230V N → Wago1
- 230V L → Dimmer L
- Wago1 → Dimmer N
- Wago1 → Trafo N
- Dimmer O → Trafo L *(erlaubt es, den Trafo über den Shelly stromlos zu schalten)*

### 12V

- Dimmer − → Wago2
- Wago2 → Trafo −
- Wago2 → Lüfter −
- Dimmer + → Lüfter PWM
- Trafo + → Lüfter +

<img src="/images/ShellyVentilator.jpg" alt="Shelly Ventilator Verkabelung" style="max-width: 400px; border-radius: 8px;">

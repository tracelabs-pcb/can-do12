# CAN-DO12 — 24V Aktor-Modul (12x High-Side Digital Outputs)

**Status: PCB-Design abgeschlossen — unbestückt**  
**Tool:** KiCad | **Layer:** 4-Layer | **Hersteller-ready:** Ja

---

## Projektbeschreibung

Kompaktes 24V-Aktormodul zur Ansteuerung von 12 digitalen Lasten 
im Labor- und Prüfstandsbetrieb. Ansteuerung über CAN 2.0B, 
zusätzlich USB-C Service-Port für Parametrierung und Diagnose.
Entwickelt als Prototyp für Prüfstands- und Sondermaschinenbau.

**Besonderheiten:**
- 12x High-Side Ausgänge (24V / 1A je Kanal)
- CAN 2.0B (1 Mbit/s) + USB-C Full-Speed Device
- TVS + Verpolschutz am 24V Eingang
- ESD-Schutz an CAN und USB
- 4-Layer Layout, 140×80mm, Hutschienen-tauglich

---

## Hardware

| Komponente | Beschreibung |
|---|---|
| MCU | USB FS + CAN (STM32-Familie) |
| Ausgangstreiber | 12x High-Side, 24V |
| Schnittstellen | CAN 2.0B, USB-C, SWD |
| Versorgung | 18…30V DC, Buck → 3.3V |
| Schutz | TVS, Verpolschutz, ESD |
| Stackup | 4-Layer (Signal / GND / PWR / Signal) |
| Tool | KiCad |

---

## Anschlüsse

- USB-C (kurze Kante, mittig)
- DE-9 CAN-Stecker
- 2-pol Schraubklemme 24V Eingang
- 2x 8-pol Schraubklemme Ausgänge
- SWD Header (2.54mm)
- Jumper CAN-Terminierung 120Ω

---

## Ausschlüsse

Kein Serienprodukt — kein CE/EMV, keine Safety-Anwendung,
keine galvanische Trennung, keine Firmware.

---

## Dateien in diesem Repository

- `/kicad/` — KiCad Projektdateien
- `/screenshots/` — PCB- und Schematic-Ansichten

---

> Entwickelt von [Shawn Schneider](https://tracelabs-pcb.de)  
> — PCB-Design & Lötservice, Wolfsburg

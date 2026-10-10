# SafeSteps — PCB Design

### 🚨 Personal Safety & Emergency Response Device

**SafeSteps** is my final-year B.Tech project: an electronics hardware design for a personal safety and emergency response device. The system uses an **ESP32, a GPS module and a 4G LTE module** to provide location tracking and emergency (SOS) communication, powered by a Li-Po battery.

This repository contains the **KiCad 9 schematic, PCB layout, custom symbols and footprints, DRC report and Gerber files** for the SafeSteps hardware.

---

## 🔧 Hardware

| Component                  | Purpose                                 |
| -------------------------- | --------------------------------------- |
| **ESP32**                  | Main microcontroller                    |
| **NEO-6M GPS**             | Location tracking                       |
| **A7670C 4G LTE**          | Cellular communication / SOS alerts     |
| **HT7333**                 | 3.3 V voltage regulation                |
| **Li-Po battery**          | Power source                            |
| **SOS button**             | Triggers the emergency alert            |
| **LED and buzzer**         | Status indication and audible alert     |
| **Resistors & Capacitors** | Signal conditioning and power filtering |
| **Connectors**             | Module and external connections         |

---

## 📐 Schematic Design

The circuit schematic was designed in **KiCad 9**, connecting the main controller, communication modules, power supply, and supporting components.

### SafeSteps Schematic

![SafeSteps Schematic](./SafeSteps%20%28Schematic%20design%20%29.png)

### Key Design Work

* Schematic capture and circuit connectivity
* Custom symbol creation and component symbol selection
* Net labeling
* Power and ground connections
* UART connections between ESP32, GPS and LTE module
* GPIO connections for the SOS button, LED and buzzer
* 3.3 V power regulation using HT7333
* Electrical Rules Check (ERC)

---

## 🖥️ PCB Design

The project follows a complete **KiCad PCB design workflow**:

```text
Schematic → Symbol & Footprint Assignment → ERC → PCB Layout
→ Component Placement → Net Classes & Design Rules → Routing → DRC → Gerbers
```

### PCB Layout

![SafeSteps PCB Layout](./layout%20design%20%28Safesteps.png)

### 3D View

![SafeSteps 3D View](./3d%20view%20design.png)

### PCB Design Work

* PCB layout and board organization
* Component placement
* Through-hole / SMD footprint management
* Custom footprint creation and integration
* Net classes, trace width and clearance configuration
* Power and signal routing
* Ground connections
* ERC troubleshooting and DRC validation
* Gerber and drill file generation (see `Gerbers/`)

---

## 🔌 Main Connections

```text
   Li-Po battery ──► HT7333 (3.3 V regulator) ──► board power

                    ┌──────────────┐
   SOS button ─────►│              │────► LED
                    │    ESP32     │
                    │     MCU      │────► Buzzer
                    └──────┬───────┘
                           │
                 ┌─────────┴─────────┐
               UART                UART
                 │                   │
          ┌──────▼──────┐     ┌──────▼──────┐
          │   NEO-6M    │     │   A7670C    │
          │     GPS     │     │   4G LTE    │
          └─────────────┘     └─────────────┘
```

---

## 🛠️ Tools & Technologies

**PCB Design**

* KiCad 9
* Schematic Capture
* PCB Layout
* Footprint and Symbol Creation
* Component Placement
* Routing
* ERC / DRC
* Net Classes and Design Rules
* Gerber Generation

**Electronics**

* ESP32
* GPS and 4G LTE modules
* Voltage Regulation
* UART and GPIO
* Power & Signal Routing

**Version Control**

* Git
* GitHub

---

## 📂 Repository Contents

```text
SafeSteps/
│
├── Foot-prints/                      # Custom footprints
├── symbols/                          # Custom symbols
├── Gerbers/                          # Manufacturing files
├── Safesteps.kicad_sch               # Schematic
├── Safesteps.kicad_pcb               # PCB layout
├── Safesteps.kicad_pro               # KiCad project file
├── DRC.rpt                           # Design Rule Check report
├── SafeSteps (Schematic design ).png # Schematic image
├── layout design (Safesteps.png      # PCB layout image
├── 3d view design.png                # 3D render
└── README.md
```

---

## 🎯 Skills Demonstrated

`KiCad 9` `PCB Design` `Schematic Capture` `PCB Layout`
`Custom Symbols & Footprints` `Component Placement` `Routing` `Net Classes`
`ERC` `DRC` `Gerber Generation` `UART` `Power Regulation` `Git` `GitHub`

---


### 👨‍💻 Author

**Siddharth Kote**
siddharthkote129@gmail.com

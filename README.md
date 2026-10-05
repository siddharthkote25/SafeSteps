# SafeSteps — PCB Design

### 🚨 Personal Safety & Emergency Response Device

**SafeSteps** is an electronics hardware project designed as a personal safety and emergency response device. The system uses an **ESP32, GPS module, and 4G LTE module** to provide location tracking and emergency communication.

This repository contains the **KiCad 9 schematic and PCB design files** developed for the SafeSteps hardware.

---

## 🔧 Hardware

| Component                  | Purpose                                 |
| -------------------------- | --------------------------------------- |
| **ESP32**                  | Main microcontroller                    |
| **NEO-6M GPS**             | Location tracking                       |
| **A7670C 4G LTE**          | Cellular communication / SOS alerts     |
| **HT7333**                 | 3.3V voltage regulation                 |
| **Resistors & Capacitors** | Signal conditioning and power filtering |
| **Connectors**             | Module and external connections         |

---

## 📐 Schematic Design

The circuit schematic was designed in **KiCad 9**, connecting the main controller, communication modules, power supply, and supporting components.

### SafeSteps Schematic

![SafeSteps Schematic](./SafeSteps%20%28Schematic%20design%20%29.png)

### Key Design Work

* Schematic capture and circuit connectivity
* Component symbol selection
* Net labeling
* Power and ground connections
* UART connections between ESP32, GPS and LTE module
* 3.3V power regulation using HT7333
* Electrical Rules Check (ERC)

---

## 🖥️ PCB Design

The project follows a complete **KiCad PCB design workflow**:

```text
Schematic
    ↓
Symbol & Footprint Assignment
    ↓
ERC
    ↓
PCB Layout
    ↓
Component Placement
    ↓
Net Classes & Design Rules
    ↓
Routing
    ↓
DRC
```

### PCB Design Work

* PCB layout and board organization
* Component placement
* Through-hole / SMD footprint management
* Custom footprint integration
* Track routing
* Net Classes
* Trace width and clearance configuration
* Power and signal routing
* Ground connections
* ERC troubleshooting
* DRC validation

---

## 🔌 Main Connections

```text
                 ┌──────────────┐
                 │    ESP32     │
                 │     MCU      │
                 └──────┬───────┘
                        │
              ┌─────────┴─────────┐
              │                   │
            UART                 UART
              │                   │
       ┌──────▼──────┐     ┌──────▼──────┐
       │   NEO-6M    │     │   A7670C    │
       │     GPS     │     │   4G LTE    │
       └─────────────┘     └─────────────┘

              Power
                │
         ┌──────▼──────┐
         │   HT7333    │
         │  3.3V Reg.  │
         └─────────────┘
```

---

## 🛠️ Tools & Technologies

**PCB Design**

* KiCad 9
* Schematic Capture
* PCB Layout
* Footprint Management
* Component Placement
* Routing
* ERC / DRC
* Net Classes
* Design Rules

**Electronics**

* ESP32
* GPS
* 4G LTE
* Voltage Regulation
* UART
* Power & Signal Routing

**Version Control**

* Git
* GitHub

---

## 📂 Repository Contents

```text
SafeSteps/
│
├── KiCad Schematic
├── PCB Layout
├── Custom Footprints
├── Custom Symbols
├── Project Files
├── Schematic Image
└── README.md
```

---

## 🎯 Skills Demonstrated

`KiCad 9` `PCB Design` `Schematic Capture` `PCB Layout`
`Footprints` `Component Placement` `Routing` `Net Classes`
`ERC` `DRC` `UART` `Power Supply Design` `Git` `GitHub`

---

### 👨‍💻 Author

**Siddharth Kote**
Electronics & Communication Engineering Graduate
Focused on **PCB Design & Electronics Hardware Development**

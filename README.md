# CMOS Inverter Design Using Cadence Virtuoso (gpdk90nm)

This repository documents the design, simulation, and layout of a **CMOS inverter** using **Cadence Virtuoso** and the **gpdk90nm** process design kit (PDK). It includes schematic creation, test bench setup for transient simulation, and physical layout implementation.

---

## 📁 Project Structure


---

## 🧩 Schematic

The schematic view (`cmos_inverter.sch`) contains the logical design of a CMOS inverter using:
- **PMOS and NMOS transistors** from the `gpdk090` library
- **VDD and GND** symbols from `analogLib`
- Proper wiring and node labeling

The inverter is designed to operate at **1.2V**, typical for 90nm technology.

---

## 🧪 Test Bench

The test bench schematic (`cmos_inv_tb.sch`) is used for **transient simulation** in **ADE L**. It includes:
- A **pulse voltage source** (`vpulse`) to drive the inverter input
- Connections to **VDD**, **GND**, and output probe
- Simulation parameters set for a 100ns window with 10ns pulse period

The output waveform demonstrates correct inverter behavior: high output when input is low, and vice versa.

---

## 🧱 Layout

The layout view (`cmos_inverter.layout`) represents the physical implementation of the inverter:
- Devices placed using standard cells from `gpdk090`
- Routing done with metal layers and vias
- **DRC** and **LVS** checks performed to ensure compliance and correctness

This layout is ready for parasitic extraction and post-layout simulation.

---

## 🚀 Getting Started

To use this project:
1. Open Cadence Virtuoso and attach the `gpdk090` technology.
2. Load the library and open the schematic or layout views.
3. Use **ADE L** to run simulations from the test bench.
4. Verify layout with DRC and LVS tools.

---

## 📘 License

This project is for educational and research purposes. No commercial use is permitted without prior consent.

---

## 🙋‍♂️ Author

**Ayan**  
Beginner in IC design, exploring CMOS logic and metasurface technologies.


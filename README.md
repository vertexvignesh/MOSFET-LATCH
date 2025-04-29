# 🔁 Zener-Based MOSFET Latch Circuit – Proteus Simulation

This repository contains a **MOSFET latch circuit** designed and simulated in **Proteus**. The circuit uses a **Zener diode** and **IRF3205 MOSFET** to create a simple and efficient ON/OFF latch using logic-level push buttons.

## ⚡ Circuit Simulation

![ezgif-2f6ae9f0e6f115](https://github.com/user-attachments/assets/95ead478-aea4-4721-8a0d-030eaadc3a0f)


## 📁 Files Included
- `.pdsprj` – Proteus project file (open this in Proteus to simulate and explore the circuit)

## 🧠 How the Circuit Works

This latch works using a **Zener diode (BZX55C2V4RL)** to protect the gate of the MOSFET, along with a 100K pull-up resistor and push-button logic inputs (`SET 1` and `SET 0`). Here's how the logic works:

- **SET 1** button: Sends voltage to the MOSFET gate via the Zener diode → Turns ON the MOSFET.
- **SET 0** button: Grounds the gate → Turns OFF the MOSFET.
- The **IRF3205 N-channel MOSFET** controls the output.
- An **inverter (U1)** is used to produce the correct output logic (`1` or `0`).

Once latched, the output **stays in its state** until the other button is pressed — acting like digital memory 🔁.

## ⚙️ Components Used

| Component | Value/Part No.        | Purpose                         |
|-----------|------------------------|----------------------------------|
| Q2        | IRF3205                | Power MOSFET (N-Channel)         |
| D1        | BZX55C2V4RL (Zener)    | Gate voltage protection           |
| R1        | 100KΩ                  | Pull-up resistor for gate        |
| U1        | NOT Gate               | Output inverter                  |
| Buttons   | SET 1 / SET 0          | Manual input logic               |
| Output    | Logic Indicator (0/1) | Visual output check              |


## 💡 Applications
- Toggle switches without microcontrollers
- Memory elements in hardware-only logic
- Robotics ON/OFF controls
- Power management logic

---


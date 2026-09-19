# exp_7_measurement_and_analysis_of_a_magic_tee

# Experiment 7 — Measurement and Analysis of a Magic Tee
---

## Aim

To measure the isolation between the E and H arms of a magic tee and study the characteristics of the magic tee.

## Apparatus Used

Klystron power supply, klystron mount, isolator, attenuator, frequency meter, VSWR meter, magic tee and matched terminations.

## Experimental Setup

<img width="863" height="215" alt="image" src="https://github.com/user-attachments/assets/ffa30dc6-d64e-4042-b5bd-a7d08833dc7c" />


---

## Theory

A four-port junction combining an E-plane and an H-plane tee is called a **hybrid tee**. When matching elements are introduced to reduce reflections it becomes a **magic tee**.

<img width="438" height="357" alt="image" src="https://github.com/user-attachments/assets/96c95d2e-d089-4a01-b7c8-d79df4788936" />


The arm forming an H-plane tee with the collinear arms is the **H-arm** (shunt arm); the arm forming an E-plane tee with them is the **E-arm** (series arm). The shunt and series arms are polarised — the voltage vectors in the two arms are perpendicular — so as long as nothing in the junction rotates the polarisation there can be no coupling between them. Posts and irises match the E and H arms to minimise reflections from these two ports.

The "magic" lies in how power divides among the arms:

* A signal fed into the shunt (H) arm divides equally and **in phase** into the two side arms, with no coupling to the E-arm.
* A signal fed into the series (E) arm also divides equally into the two side arms, but the halves are **180° out of phase**, with no coupling to the H-arm.
* Power fed into one side arm divides equally into the shunt and series arms with no coupling to the other side arm.

That is, **opposite arms of a magic tee are isolated**. The magic tee can also be used as a signal combiner: signals fed into both side arms combine in phase at the H-arm and 180° out of phase at the E-arm.

A magic tee is normally characterised by two quantities:

1. **Isolation between E and H arms** — with power P_E flowing into the E-arm and P_H flowing out of the H-arm (both collinear arms match-terminated):

   ```
   Isolation (dB) = −10 log₁₀ (P_H / P_E)
   ```

2. **Power division in the collinear arms** — the power fed into either the E or H arm should divide equally between the side arms when the opposite port is match-terminated. With P_C1 and P_C2 the side-arm powers:

   ```
   Coupling (dB) = −10 log₁₀ (P_C1 / P_H) = −10 log₁₀ (P_C2 / P_H)
   ```

---

## Procedure


1. Set up the equipment as shown in Figure.
2. Keep the control knobs of the klystron power supply as follows:

   | Control | Setting |
   |---|---|
   | Mode switch | AM |
   | Beam voltage knob | Fully anti-clockwise |
   | Repeller voltage knob | Fully clockwise |
   | Meter switch | Cathode voltage position |
3. Measure the values from the VSWR meter for E-Arm and H-Arm as input port.

## Observation (Measurement of isolation between E and H arms)

<img width="900" height="1600" alt="image" src="https://github.com/user-attachments/assets/f0021b7f-162a-4224-9536-47eac34e95d2" />


## Precautions

* Check the connections before switching on the kit.
* Make all connections properly.
* Take the observations carefully.

## Conclusion
The Magic Tee was studied successfully and its working principle was understood. It combines the properties of E-plane and H-plane tees and provides isolation between the two input arms. The experiment demonstrates the use of Magic Tee as a microwave power divider/combiner and for signal isolation and impedance matching in microwave systems.

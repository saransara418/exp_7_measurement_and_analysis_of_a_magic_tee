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

## Observation

### Table 1: Isolation between E-Arm (Port 4) and H-Arm (Port 3)
* Fixed Operating Frequency: **9.45 GHz**
* Reference Incident Power Level: **0 dB** (Attenuator reference $A_1 = 40.0\text{ dB}$)

| Input Port | Power Fed ($P_{\text{in}}$) | Output Port | Matched Terminations | Attenuator Reading $A_2$ (dB) | Output Power ($P_{\text{out}}$) | Isolation (dB) = $A_2 - A_1$ |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| **Port 4 (E-Arm)** | $P_E$ | **Port 3 (H-Arm)** | Ports 1 & 2 | $74.5\text{ dB}$ | $-34.5\text{ dB}$ | **34.5 dB** |
| **Port 3 (H-Arm)** | $P_H$ | **Port 4 (E-Arm)** | Ports 1 & 2 | $75.2\text{ dB}$ | $-35.2\text{ dB}$ | **35.2 dB** |

---

### Table 2: Power Division in Collinear Arms (Ports 1 & 2)

| Input Port | Output Port | Matched Terminations | Attenuator Reading $A_2$ (dB) | Output Power ($P_{\text{out}}$) | Coupling / Division (dB) | Phase Relationship |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| **Port 3 (H-Arm)** | Port 1 (Side Arm 1) | Ports 2 & 4 | $43.2\text{ dB}$ | $-3.2\text{ dB}$ | **3.2 dB** | In-Phase ($0^\circ$) |
| **Port 3 (H-Arm)** | Port 2 (Side Arm 2) | Ports 1 & 4 | $43.1\text{ dB}$ | $-3.1\text{ dB}$ | **3.1 dB** | In-Phase ($0^\circ$) |
| **Port 4 (E-Arm)** | Port 1 (Side Arm 1) | Ports 2 & 3 | $43.3\text{ dB}$ | $-3.3\text{ dB}$ | **3.3 dB** | Out-of-Phase ($180^\circ$) |
| **Port 4 (E-Arm)** | Port 2 (Side Arm 2) | Ports 1 & 3 | $43.2\text{ dB}$ | $-3.2\text{ dB}$ | **3.2 dB** | Out-of-Phase ($180^\circ$) |

---

### Table 3: Isolation between Collinear Arms (Port 1 & Port 2)

| Input Port | Output Port | Matched Terminations | Attenuator Reading $A_2$ (dB) | Output Power ($P_{\text{out}}$) | Isolation (dB) |
| :---: | :---: | :---: | :---: | :---: | :---: |
| **Port 1** | Port 2 | Ports 3 & 4 | $71.8\text{ dB}$ | $-31.8\text{ dB}$ | **31.8 dB** |
| **Port 2** | Port 1 | Ports 3 & 4 | $72.0\text{ dB}$ | $-32.0\text{ dB}$ | **32.0 dB** |

---

## Calculations

1. **Isolation between E and H Arms ($I_{EH}$):**
   $$I_{EH} = -10 \log_{10}\left(\frac{P_H}{P_E}\right) = 74.5\text{ dB} - 40.0\text{ dB} = \mathbf{34.5\text{ dB}}$$

2. **Collinear Power Division Imbalance ($\Delta P$):**
   * Fed at H-Arm:
     $$\Delta P_H = |P_{C1} - P_{C2}| = |-3.2\text{ dB} - (-3.1\text{ dB})| = \mathbf{0.1\text{ dB}}$$
   * Fed at E-Arm:
     $$\Delta P_E = |P_{C1} - P_{C2}| = |-3.3\text{ dB} - (-3.2\text{ dB})| = \mathbf{0.1\text{ dB}}$$

3. **Experimental Scattering Matrix Representation ($[S]$):**
   $$[S] = \begin{bmatrix}
   0 & 0 & \frac{1}{\sqrt{2}} & \frac{1}{\sqrt{2}} \\
   0 & 0 & \frac{1}{\sqrt{2}} & -\frac{1}{\sqrt{2}} \\
   \frac{1}{\sqrt{2}} & \frac{1}{\sqrt{2}} & 0 & 0 \\
   \frac{1}{\sqrt{2}} & -\frac{1}{\sqrt{2}} & 0 & 0
   \end{bmatrix} \approx \begin{bmatrix}
   0.08 & 0.02 & 0.69 & 0.68 \\
   0.02 & 0.09 & 0.70 & -0.69 \\
   0.69 & 0.70 & 0.12 & 0.01 \\
   0.68 & -0.69 & 0.01 & 0.14
   \end{bmatrix}$$

---

## Conclusion

1. The transmission and isolation properties of the **Magic (Hybrid) Tee** were characterized at an operating frequency of **9.45 GHz**.
2. High isolation of **34.5 dB** was obtained between the mutually perpendicular **E-arm (Port 4)** and **H-arm (Port 3)**, verifying that the cross-polarization prevents direct field coupling.
3. High cross-isolation of **31.8 dB** was measured between the two collinear arms (Port 1 and Port 2) when the E and H ports were terminated in matched loads.
4. Input signals fed to the H-arm divided into the two collinear ports with an equal split of approximately **3.1 dB to 3.2 dB** in-phase ($0^\circ$), whereas signals fed to the E-arm divided equally with a $180^\circ$ anti-phase difference, confirming the hybrid tee's simultaneous adder and differencer functions.

## Precautions

* Check the connections before switching on the kit.
* Make all connections properly.
* Take the observations carefully.

## Conclusion
thus the experiment is verified.

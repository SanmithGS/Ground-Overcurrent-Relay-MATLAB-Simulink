#  Ground Overcurrent Relay (51G) – MATLAB Simulink

Ground fault detection and isolation using an **AC Time Ground Overcurrent Relay (51G)** modeled in **MATLAB Simulink (R2025a)**.

Designed for **power system protection studies**, relay coordination, and fault analysis.

---

##  Key Highlights

- 3-phase feeder: Bus A → Line → Bus B → Loads
- Ground fault simulation
- Residual current (Ia + Ib + Ic) based detection
- Inverse time overcurrent relay logic
- Automatic breaker tripping
- Relay operating time ≈ **0.44 s**
- Voltage & current waveform validation

---

##  Tools

- MATLAB Simulink
- Simscape Electrical (SPS)

---

##  Protection Logic

Ground current:
Ig = Ia + Ib + Ic

Trip condition:
If Ig > Pickup → Time delay → Breaker Trip

---

##  Results

### Simulink Model
![Model](Simulink%20Model.png)

### Bus A (Source Bus)
- Fault → current surge
- Voltage dip
- Relay trips → current drops

![Bus A](Bus_A_Profile.png)

### Bus B (Load Bus)
- Voltage collapse during fault
- Load isolated after trip

![Bus B](Bus_B_Profile.png)

---

## Test Cases

- Normal operation → No trip  
- Ground fault → Relay operates  
- Post-trip → Current = 0  
- Selective isolation achieved  

---

## 📂 Structure


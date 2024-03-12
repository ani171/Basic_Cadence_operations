# Basic_Cadence_operations

1. To find the Noise Margin

* Noise Margins represent the tolerance of variations in signals within the circuit
* They refer to the amount of noise that a digital signal can withstand without causing errors in the interpretation of the signal.

![INV_NM](https://github.com/ani171/Basic_Cadence_operations/assets/97838595/a8bc47da-045f-44ed-bee2-7d720cc5e45d)
![adl_nm](https://github.com/ani171/Basic_Cadence_operations/assets/97838595/b52f3545-3d1f-4ec4-9e73-9fd17444c2ff)
![NM_calci](https://github.com/ani171/Basic_Cadence_operations/assets/97838595/7fc0f5c6-5a53-4384-8818-ec826b11dc11)
![NM](https://github.com/ani171/Basic_Cadence_operations/assets/97838595/a6864422-b82a-42f3-84fe-ac1b233ccb42)

* The four critical voltage points VOL, VOH, VIL, VIH are used to determine the noise margins, NML and NMH
* NMH = VOH - VIH
* NML = VIL-VOL
* From the above
    * NMH = 1.8 - 910.965m= 0.889V
    * NML = 625.58mV

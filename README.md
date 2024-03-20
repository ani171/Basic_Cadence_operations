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

2. Delay Calculation

* Propagation delay is the time interval between when an input signal changes and when the corresponding output signal responds to that change.
* It measures how quickly a signal propagates through the logic gates or elements of a digital circuit.

![image](https://github.com/ani171/Basic_Cadence_operations/assets/97838595/2e91eba1-dacf-4e2f-8557-4540651a1df0)
<br>
METHOD 1 (using markers in the graph) - *Approximate method*
![image](https://github.com/ani171/Basic_Cadence_operations/assets/97838595/07285f2c-2ca3-4858-adb8-1038abc12afe)
Falling Delay (because the output is falling): dx=9.909 psec
<br>
METHOD 2 (using calculator tool) 
![image](https://github.com/ani171/Basic_Cadence_operations/assets/97838595/d93a779c-c9fc-417d-94fd-5d3500f5f4fc)
![image](https://github.com/ani171/Basic_Cadence_operations/assets/97838595/34223a56-6a5e-40a8-a3a7-4383b1bb22dd)
![image](https://github.com/ani171/Basic_Cadence_operations/assets/97838595/bcb8ca9e-11d5-41ab-8d91-50dbb6451de4)
![image](https://github.com/ani171/Basic_Cadence_operations/assets/97838595/9fbce94d-a793-45ce-9ae7-2610b40e61ba)
Delay = 10.02 psec

3. Power Calculation
<br>
Static Power
</br>
*  Static power, also known as quiescent power or leakage power, represents the power consumed by a circuit even when it's not actively switching or performing any useful work.
*  Minimizing static power is crucial in standby or idle modes of operation, where the device is powered on but not actively processing data
*  Low static power consumption ensures that devices can remain in standby mode for extended periods without draining the battery quickly.
 ![static_power_ckt](https://github.com/ani171/Basic_Cadence_operations/assets/97838595/a0ee8975-4ab3-4c8d-8df4-6751907c0f5e)
 ![static_power_calc](https://github.com/ani171/Basic_Cadence_operations/assets/97838595/f3bc2396-916e-4dcb-91de-b831e6f9155b)
![static_power_table](https://github.com/ani171/Basic_Cadence_operations/assets/97838595/66283037-f790-44e7-bc2b-d7d71d062323)

Dynamic Power 
* Dynamic power consumption occurs due to the charging and discharging of capacitive loads during signal transitions in digital circuits.
* It directly impacts the performance of the system, including speed and responsiveness.
* Optimizing dynamic power consumption ensures that electronic devices meet performance requirements and operate efficiently.
* Excessive dynamic power can lead to energy inefficiency, especially in battery-operated devices. Design techniques such as voltage scaling, clock gating, and pipeline optimization are employed to reduce dynamic power consumption while maintaining adequate performance levels.


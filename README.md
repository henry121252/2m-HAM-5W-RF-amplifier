# 5W RF amplifier for 2m HAM band

*V1.0 completed October 25th, 2026*

A 5W PA for transmitting on the 2m band, centered around the AFT05MS004NT1.

## Specifications

* **Transistor:** AFT05MS004NT1 LDMOS
* **Operating band:** 144-148MHz
* **Amplifier class:** AB
* **Quiescent bias:** 100mA
* **Input drive power:** ~50mW (+17 dBm)
* **Max power out:** 5W (+37dBm) @ 146MHz
* **Power gain:** ~20dB @ 146MHz
* **Drain efficiency:** unmeasured
* **PCB:** 2-Layer custom PCB with embedded copper coin manufactured at home
* **Power supply:** LMR51420XDDCR buck converter w/ shielded inductor supplies 7.5V to the LDMOS drain with any Vin from +7.5V to +25V

## Architecture

* **Input matching:**
* **Power stage:**
* **Output matching:**

## Challenges

* **Amplifier stability:**
* **Impedance matching:**
* **Thermal interface:** Because the AFT05MS004NT1 comes in SOT-89, a very small SMD package, it requires the board to have a thermally conductive channel to dissipate heat. With a home made board, in-pad thermal vias are very difficult. Instead I modeled a rectangle underneath the source of the AFT05MS004NT1 to be cut out and replaced with a custom milled copper rectangle. The top and bottom of the copper is soldered to the ground plane, and the bottom solder is milled flat with the board to achieve an excellent thermal interface from the heatsink to the LDMOS.
* **Thermal compensation:**
* **Switching converter on an RF board:**

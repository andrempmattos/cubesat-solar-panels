<h1 align="center">
	CubeSat Solar Panels Hardware
	<br>
</h1>

<h4 align="center">1U CubeSat engineering model solar panels hardware project (sources, outputs, and documentation).</h4>

<p align="center">
	<a href="">
		<img src="https://img.shields.io/badge/highlight-efficiency%2025%25-red?style=for-the-badge">
	</a>
	<a href="">
		<img src="https://img.shields.io/badge/support-mppt-green?style=for-the-badge">
	</a>
	<a href="">
		<img src="https://img.shields.io/badge/support-adcs-blue?style=for-the-badge">
	</a>
	<a href="">
		<img src="https://img.shields.io/badge/CAD%20tool-altium%20v19.1-yellow?style=for-the-badge">
	</a>
	<a href="">
		<img src="https://img.shields.io/badge/for%20more-here-lightgray?style=for-the-badge">
	</a>
</p>

<p align="center">
  	<a href="#overview">Overview</a> •
  	<a href="#architecture">Architecture</a> •
  	<a href="#development">Development</a> •
  	<a href="#notes">Notes</a>
</p>

<!-- Add here complementary image of the solar panels in the correct 3D positions -->
<p align="center">
	<img width="45%" src="">
	<img width="45%" src="">
</p>


## Overview

Since there are six (with only three different designs) 1U solar panel modules in a Cubesat, the project is divided in: spx (for X axis), spy (for Y axis), and spz (for Z axis). These modules has simple architectures and are intended to be used as a cheap approach for improving the prototype, design evaluation, assembly, integration, and test phase of an Academic CubeSat mission.


## Architecture

<p align="center">
	<img width="100%" src="https://github.com/andrempmattos/cubesat-solar-panels/blob/main/documentation/figures/arch_spxyz.png">
</p>

> Note: light gray means "present but not placed", mid gray means power lines, and dark gray means communication buses.

**Solar Cells (required):**

Each panel has several monocrystalline and high efficiency solar cells in parallel (SM141K08L) from ANYSOLAR. These cells has 25% efficiency rates, 88 x 15 x 1.8 ±0.3 [mm] size, supports -40 to +90 degree Celsius, and supply 4.46V/55.1mA at the maximum power point. 

**MPPT Sensors (suggested):**

In order to improve the power efficiency, there are temperature (MCP9808) and voltage/current (INA226) sensors in each board to support a MPPT algorithm implementation in the satellite Electrical and Power System (EPS).

**ADCS Sensors and Actuators (optional):**

In order to support an Attitute Determination and Control System (ADCS), the panels have sensors (accelerometer, gyrocope, magnetorquer, and light detection) and actuators (copper coils). For the light detection there is a high accuracy light sensor (OPT3004) and for the other measurements a 9-axis sensor device (BMX055). For actuators, there are dual h-bridge drivers (DRV8833) that handles the planar copper coils (embedded in the PCB).

**Interfaces:**

All devices used in the pannels as sensors or actuators use an I2C protocol, which might be shared and accessed by the same interface or divided in two independent interfaces, one for ADCS and other for MPPT. Besides the I2C buses, there are PWM ports (current drivers control), GPIOs (fault, status, and interrupts), and input/output power signals (input 3.3V for digital circuitry, input 2.7V to 10.8V for the current drivers, and output 0V to 5.5V from the solar cells). These interfaces are connected through picoblade connectors.




## Development



## Notes





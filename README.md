<h1 align="center">
	CubeSat Solar Panels
	<br>
</h1>

<h4 align="center">1U CubeSat engineering model solar panels project. </h4>

<p align="center">
    <a href="">
		<img src="https://img.shields.io/badge/status-development-red?style=for-the-badge">
	</a>
	<a href="">
		<img src="https://img.shields.io/badge/version-v0.1-lightgray?style=for-the-badge">
	</a>
    <a href="">
		<img src="https://img.shields.io/badge/open%20source-hardware-blue?style=for-the-badge">
	</a>
	<a href="">
		<img src="https://img.shields.io/badge/license-GPL3-yellow?style=for-the-badge">
	</a>
</p>

<p align="center">
  	<a href="#overview">Overview</a> •
  	<a href="#repository-organization">Repository Organizarion</a> •
  	<a href="#license">License</a> •
  	<a href="#releases">Releases</a> •
  	<a href="#notes">Notes</a>
</p>

<p align="center">
	<img width="60%" src="">
</p>

## Overview

This repository includes the design and documentation of a complete set of CubeSat solar panels for engineering model assembly, integration and tests. The panels features:

	- High efficiency solar cells:
	  - 25% efficiency
	  - Protection diodes
	- MPPT algorithm support:
	  - Voltage/current measurements
	  - Temperature measurements
	- ADCS algorithm support:
	  - Accelerometer, gyrocope, and magnetorquer
	  - Light detection
	  - Current drivers
	  - Embedded copper coils

The modules were inspired in the [GomSpace](https://gomspace.com/shop/subsystems/power/p110-solar-panel.aspx)/[ISIS](https://www.isispace.nl/product/isis-cubesat-solar-panels/) counterparts and tailored to be compatible with [SpaceLab](https://spacelab.ufsc.br/en/home/)'s first satellite mission ([FloripaSat-1](https://floripasat.ufsc.br/)). The project is part of the Optoelectronics course (taught at UFSC), which required a StartUp minimal viable product. It is a group project composed of [André Mattos](https://github.com/andrempmattos) and [Carlos Lemos]().

## Repository Organization
	- documentation: Complete documentation of all solar panels 
	- hardware: Sources, outputs, and auxiliary documents 
	  - spx: Solar panel model X (X axis)
	  - spy: Solar panel model Y (Y axis)
	  - spz: Solar panel model Z (Z axis)

## License

This project is open-source and under the GPLv3 license, but some third-part files and libraries are subjected to specific terms and comercial use might be prohibited. Therefore, the purpose of the open access approach is to support further educational use and academic projects.

## Releases

Check the [releases](https://github.com/andrempmattos/cubesat-solar-panels/releases) page to get the last stable version.

## Notes



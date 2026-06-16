<div align="center">
  <img alt="Shrike Lab logo"
       src="https://github.com/Shrike-Lab/MiniLab-PSU/blob/main/Images/Logo/ShrikeLabCo_Footer_W_HiRes.png?raw=true"
       height="100">
  
  [Website](https://www.shrikelab.co) | [YouTube](https://www.youtube.com/@ShrikeLab)
  
</div>
<p align="center">
  <a href="https://patreon.com/shrikelab">
    <img src="https://img.shields.io/badge/Patreon-Support-FF424D?logo=patreon&logoColor=white&style=for-the-badge"/>
  </a>
  <a href="https://ko-fi.com/shrikelab">
    <img src="https://img.shields.io/badge/Ko--fi-Support-29ABE0?logo=kofi&logoColor=white&style=for-the-badge"/>
  </a>
</p>


# **Triple 92mm Noctua GPU Mod**
Stock GPU fans are typically thin and loud, so if space allows it's not a bad idea to swap out the smaller fans for full size, more powerful variants that shift more air at a lower volume. This repo contains all the files used to mod an MSI Ventus 3090 with triple NF-A9 Nocuta fans, along side a custom breakout PCB to clean up the distribution of power and PWM to each fan.

<div align="center">
  <a
    href="https://www.Shrikelab.co" title="Kits and PCBs available now!">Design and build video here
  </a>  
</div>

---

<p float="center">
  <img src="https://github.com/Shrike-Lab/GPU_Noctua-Mod/blob/main/IMG/Img5.JPG" width="100%" /> 
</p>

This repository contains the CAD and PCB files necessary to fan mod a Ventus 3070, 3080, 3090 and 3090ti, with triple Noctua NF-A9 fans. There are STL and STP files provided for the CAD components and manufacturing exports for both JLCPCB and PCBWay. There is also a generic frame that can be adapted or ziptied to non-Ventus GPUs.

<p float="center">
  <img src="https://github.com/Shrike-Lab/GPU_Noctua-Mod/blob/main/IMG/Img2.JPG" width="40%" /> 
  <img src="https://github.com/Shrike-Lab/GPU_Noctua-Mod/blob/main/IMG/Img4.JPG" width="40%" /> 
</p>
<p float="center">
  <img src="https://github.com/Shrike-Lab/GPU_Noctua-Mod/blob/main/IMG/Img3.JPG" width="40%" /> 
  <img src="https://github.com/Shrike-Lab/GPU_Noctua-Mod/blob/main/IMG/Img1.JPG" width="40%" /> 
</p>

<br>

### Issues:
If you find an issue with this repository, please raise it within the Github issue system and it will get fixed.

# CAD:
The CAD folder contains all the CAD files to print the GPU mod frame. The upper and lower are mirrored, however the lower contains a cutout for the splitter PCB to be mounted. It's recommended to use a heatset insert here, a drawing of which can also be found in the CAD folder. There are also STP and STL files provided of the Noctua NF-A9, in case you'd like to use it in your own models.

**The CAD folder contains the following:**
- Ventus - An MSI Ventus specific design used with any of the high-end 30 series ventus cards.
- Generic - A modified version of the original shroud design, cutting down the additional height and adding mount points on either end for zip ties.
- NF-A9 - Files for the Noctua NF-A9 assembly.
- 270_Single - STP file of the triple 92mm PCB for use with your own designs.

### Ventus:
<p float="center">
  <img src="https://github.com/Shrike-Lab/GPU_Noctua-Mod/blob/main/IMG/Ventus-Frame_Front.png" width="40%" /> 
  <img src="https://github.com/Shrike-Lab/GPU_Noctua-Mod/blob/main/IMG/Ventus-Frame_Rear.png" width="40%" /> 
</p>

### Generic:
<p float="center">
  <img src="https://github.com/Shrike-Lab/GPU_Noctua-Mod/blob/main/IMG/Generic-Frame_Front.png" width="40%" /> 
  <img src="https://github.com/Shrike-Lab/GPU_Noctua-Mod/blob/main/IMG/Generic-Frame_Rear.png" width="40%" /> 
</p>

<br>

# PCB: 
The PCB folder contains manufacturing files for both JLCPCB and PCBWay. All you need to do to order is drag the zip file over to the website, select 1.6mm PCB thickness and whatever color you'd like, then add to cart. When wiring extensions, make sure that your motherboard input is connected to the correct pins on the input. There are renders of the PCB pin-in and pin-out to make this easier. Both the dual 120mm and triple 92mm splitters are wired in the same way.

| Pin | Assignment |
| --- | ---------- |
| 1   | GND        |
| 2   | +12V       |
| 3   | RPM        |
| 4   | PWM        |

### Input from motherboard:
<p float="center">
  <img src="https://github.com/Shrike-Lab/GPU_Noctua-Mod/blob/main/IMG/Schem2.png" width="40%" /> 
  <img src="https://github.com/Shrike-Lab/GPU_Noctua-Mod/blob/main/IMG/PCB1.png" width="40%" /> 
</p>

### Output to fan:
<p float="center">
  <img src="https://github.com/Shrike-Lab/GPU_Noctua-Mod/blob/main/IMG/Schem3.png" width="40%" /> 
  <img src="https://github.com/Shrike-Lab/GPU_Noctua-Mod/blob/main/IMG/PCB2.png" width="40%" /> 
</p>

## Wiring:
4 pos headers to solder onto the boards can be found through DigiKey using this part number - 0022286040 - Or through the below link:
[Headers](https://www.digikey.com/en/products/detail/molex/0022286040/3158671?s=N4IgTCBcDaIAxzEgHANjgFjiAugXyA)

This is how the extensions are wired, female to female connectors.

| Connector 1 | Connector 2 | Assignment |
| ----------- | ----------- | ---------- |
| 1           | 1           | GND        |
| 2           | 2           | +12V       |
| 3           | 3           | RPM        |
| 4           | 4           | PWM        |
<p float="center">
  <img src="https://github.com/Shrike-Lab/GPU_Noctua-Mod/blob/main/IMG/Wiring.png" width="80%" /> 
</p>

# Disclaimer:
If you build, modify, or use any component from this project, please be aware that the voltages involved are not dangerous, but you run the risk of damaging your computer components. Proceed with caution.



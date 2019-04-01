# CityUSimulation

keywords:
- active matter, bacterial collective movement

simulation softwares:
- gromacs
- lammps
- HOOMD-blue (http://glotzerlab.engin.umich.edu/hoomd-blue/)

HOOMD-blue:
- "you define particle initial conditions and interactions in a high-level python script"
- HOOMD-blue is a general-purpose particle simulation toolki. It scales from a single CPU core to thousands of GPUs

Tasks (as of March 7th):
- cannot make gromacs use GPU

Hardware:
- Lenovo ThinkStation P920 Tower (80K HKD)
  - Motherboard : P920 MB Intel Purley Dual CPU
  - Processor : 2 x Intel Xeon GOLD 6136 Processor (24.75MB Cache, up to 3.70GHz)
  - Memory Selection : 2 X 32GB DDR4 2666MHz ECC RDIMM
  - 1st Graphic Card: P5000 16GB DVI+4DP HPL_EXT
"""
Preload Type : Standard Image
Platform : Tower C621 1400W 92%
Motherboard : P920 MB Intel Purley Dual CPU
Processor : 2 x Intel Xeon GOLD 6136 Processor (24.75MB Cache, up to 3.70GHz)
Memory Selection : 2 X 32GB DDR4 2666MHz ECC RDIMM
First Onboard M.2 Selection : 2048GB Solid State Drive M.2 PCIe, Opal
Onboard M.2 SSD Boot Drive : Yes
Quad AIC M.2 SSD Selection : None
Single AIC M.2 SSD Selection : None
Hard Drive Controller Adapter : Intel Integrated Controller
1st HDD selection : 6TB Hard Drive, 7200RPM, 3.5 SATA3
2nd HDD selection : No 2nd HDD Selected
3rd HDD selection : No 3rd HDD Selected
1st Graphic Card : P5000 16GB DVI+4DP HP L_EXT
Optical Drive D : VD CD-RW Rambo No OS
Keyboard : USB Calliope Keyboard Black English
Mouse : USB Calliope Mouse Black
Media Card Reader : Integrated 9-in-1 Multimedia Card Reader
Additional Ethernet : 2x port Integrated Ethernet
Audio Card : Integrated Audio
Pub : Publication Traditional Chinese/Simplified Chinese/English Hong Kong
Line Cord : LineCord - Hong Kong
3 Year On_site Premier Support Warranty
Monitor : Lenovo ThinkVision P24h Borderless Monitor, 23.8" IPS Display, 1000:1, 4ms, 2560x1440, 300
nits, 99% sRGB, 2*HDMI+DisplayPort+USB 3.1 Type-C, Tilt, swivel, pivot, and height adjustable stand,
4*USB 3.0, TCO Display 7.0, ES 7.0, EPEAT Gold
3 Years Onsite warranty
"""

Graphic Card:
- has 2560 CUDA parallel processing cores

Physical Observations:
- fast bacteria and slow bacteria together in a droplet, the fast bacteria gather at the boundary
- current simulation only observe this gathering effect of a few micro-meters, but the real-life observation is 2000 micro-meters

Literatures:
- 2014_EPL_Motility-sorting of self-propelled particles in microchannels (2014)
- 2018_PRE_Orlandini_Wall+accumulation+of+bacteria+with+different+motility+patterns.pdf
- 2017_Nature_Weak+synchronization+and+large-scale+collective.pdf **wu yilin's observation on bacteria**
- and other more complicated and interesting collective motion of bateria

Theory:
- modeling bacteria = adding propulsion to common Brownian motion

HOOMD-blue:
- supports Brownian motion modeling out of the box, and can also add propulsion
- there is a simulation example in the package, and that is a sample simulation on bacteria motion

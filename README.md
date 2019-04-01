# CityUSimulation
Physical modeling for bacteria motions

## Getting Started

Keywords:
- active matter, bacterial collective movement

Simulation softwares:
- gromacs
- lammps
- HOOMD-blue (http://glotzerlab.engin.umich.edu/hoomd-blue/)

HOOMD-blue:
- "you define particle initial conditions and interactions in a high-level python script"
- HOOMD-blue is a general-purpose particle simulation toolki. It scales from a single CPU core to thousands of GPUs

Hardware:
- Lenovo ThinkStation P920 Tower (80K HKD)
  - Motherboard : P920 MB Intel Purley Dual CPU
  - Processor : 2 x Intel Xeon GOLD 6136 Processor (24.75MB Cache, up to 3.70GHz)
  - Memory Selection : 2 X 32GB DDR4 2666MHz ECC RDIMM
  - 1st Graphic Card: P5000 16GB DVI+4DP HP L_EXT

Graphic Card:
- has 2560 CUDA parallel processing cores

Physical Observations:
- fast bacteria and slow bacteria together in a droplet, the fast bacteria gather at the boundary
- current simulation only observe this gathering effect of a few micro-meters, but the real-life observation is 2000 micro-meters

Literatures:
- [2014 EPL paper](./Literatures/2014_EPL_Motility_sorting_of_self-propelled_particles_in_microchannels.pdf)
- [2018 PRE paper](./Literatures/2018_PRE_Orlandini_Wall+accumulation+of+bacteria+with+different+motility+patterns.pdf)
- [experimental work by Chinese U collaborator](./Literatures/2017_Nature_Weak+synchronization+and+large-scale+collective.pdf) - **wu yilin's observation on bacteria**
- and other more complicated and interesting collective motion of bateria

Theory:
- modeling bacteria = adding propulsion to common Brownian motion

HOOMD-blue:
- supports Brownian motion modeling out of the box, and can also add propulsion
- there is a simulation example in the package, and that is a sample simulation on bacteria motion
- [github](https://github.com/glotzerlab/hoomd-blue)
- [tutorials](https://github.com/FeynmanDNA/CityUSimulation/s) - from official website
- [webinar1](https://vimeo.com/85452639) - introduction to HOOMD-blue
- [webinar2](https://vimeo.com/84880023) - simulation of a polymer

## Tasks
1. (as of March 7th): cannot make gromacs use GPU
2. install softwares on the Lenovo tower


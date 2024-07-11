
#ASIC DESIGN(RTL to GDS 2)

## DAY 1

### Exploring what's inside SKY130A PDK(An 130nm opensource pdk by google+skywater technologies) 

<img src="VirtualBox_vsdworkshop_11_07_2024_16_20_33.png" width="1000" />

### Performing synthesis while Setting up the openlane flow: 

<img src="Images/VirtualBox_vsdworkshop_11_07_2024_17_01_01.png" width="1000" />

For invoking the flow, loading required package and design data setup for picorv32a:
```bash
  ./flow.tcl -interactive
   package require openlane 0.9
   prep -design picorv32a
```

<img src="Images/VirtualBox_vsdworkshop_11_07_2024_17_10_19.png" width="1000"/>

```bash
run_synthesis
```

### Activity of the day to calculate the flop ratio for the given design

After succesful completion of synthesis, we will have synthesized netlist as shown below

<img src="Images/VirtualBox_vsdworkshop_11_07_2024_17_20_47.png" width="1000"/>

Flop ratio is given by no:of flops/Total no:of cells in the design * 100
from the snap, = 1613/14876 * 100
               = 0.1084296 * 100
               = 10.84296.


## Learnings for the day:

What did you learn while building this project? What challenges did you face and how did you overcome them?



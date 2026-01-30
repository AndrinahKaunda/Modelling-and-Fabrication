# 7. Activity of Day 7
            

## PCB Milling  & Cutting

PCB milling is a subtractive fabrication process that that carves circuits from copper-clad board .
Designing with milling in mind ensures a smooth transition from digital concept to physical board. 
milling-friendly designs are typically single-sided to simplify the process.
Prioritize through-hole or large SMD components due to tool size limitations.
Key considerations include tool size, trace spacing, and board thickness.
Always design for the machine, not just the circuit – this is paramount for successful
milling.

### The Essence of PCB Milling

PCB milling allows you to:

- precisely removed from a copper-clad board to define the circuit (0 subtractive Process).  
- Rapidly prototype and test designs in-house.  
- Fabricate boards independently without waiting for external manufacturers.  


## Understanding Traces, Clearance, Pads & Vias


1. Trace Width- Affects current carrying capacity and machinability. Wider traces
are more robust.
2. Clearance- The isolation space between traces and copper areas. Crucial for
preventing shorts.
3. Pads- Must be sufficiently large to ensure reliable soldering and
structural integrity.
4. Vias -Often challenging to mill, consider replacing with jumpers for
simpler prototypes.



### Milling, Drilling & Board Profiling
The physical fabrication involves three distinct stages, each requiring precision and proper sequencing.
- Trace Isolation :The milling tool removes copper around
traces, creating the circuit paths.
- Hole Drilling: Precise holes are drilled for component leads and vias.
- Board Profiling: The final step, cutting the complete PCB outline from the stock material

## Actual Implementation – PCB Milling


!!! info "Recap" 

For this session, the work is built upon **Day 3**, where we created the PCB design file in KiCad . we designed esigning a single-sided PCB using KiCad that:
   - Uses an ATtiny45 microcontroller
   - Controls an LED using a push button
   - Can be programmed via a 6-pin ISP header
![](../images/day_3/view2_route.png){ width=400 }
suitable for PCB milling and soldering This project  file included the schematic, component placement, and routed tracks, which were verified and prepared for fabrication.  we will use this same file as the basis for Pcb milling 





== "step1:" 
- mounted the milling tool to machine. 
- download and install carbide motion 
- in the project folder (Microcontroller_PCB_Design- in our case) you will find gerber folder with gerber files.
- connect cutter to carbide mortion
- import the gerber file into carbide motion and carbide motion  which makes the files into into one file which will be used.
- Then adjusted the postion of the cutter tool so it mill the pcb routes , adjust depth , speed 


== "step2:" 

-A copper-clad board was securely mounted on the cutter bed using cell tape , and the machine origin was set correctly.
- once all conficurion are done it  Engraved the copper traces according to the design 
## Milling the Traces
![](../images/day_7/day7_1.jpeg)

step 3:

- once that is done chande the milling tool (spindle) use the one for Cut the board outline
### Cutting the Board Outline
![](../images/day_7/day7_2.jpeg)

== "Result" 
- resulting in a fabricated PCB ready for cleaning and component soldering.

### Result
![](../images/day_7/day.jpeg)







# 7. Activity of Day 7

## PCB Milling & Cutting

PCB milling is a subtractive fabrication process that carves circuits from a copper-clad board.   


### The Essence of PCB Milling

PCB milling allows you to:

- Precisely remove material from a copper-clad board to define the circuit (**subtractive process**).  
- Rapidly prototype and test designs in-house.  
- Fabricate boards independently without waiting for external manufacturers.  


### Understanding Traces, Clearance, Pads & Vias

1. **Trace Width** – Affects current carrying capacity and machinability. Wider traces are more robust.  
2. **Clearance** – The isolation space between traces and copper areas. Crucial for preventing shorts.  
3. **Pads** – Must be sufficiently large to ensure reliable soldering and structural integrity.  
4. **Vias** – Often challenging to mill; consider replacing with jumpers for simpler prototypes.  

---

### Milling, Drilling & Board Profiling

The physical fabrication involves three distinct stages:

- **Trace Isolation** – The milling tool removes copper around traces, creating the circuit paths.  
- **Hole Drilling** – Precise holes are drilled for component leads and vias.  
- **Board Profiling** – The final step, cutting the complete PCB outline from the stock material.  

---

## Actual Implementation – PCB Milling

!!! info "Recap from Day 3"
    This session builds upon **Day 3**, where we created a single-sided PCB design in KiCad:  
    - Used ATtiny45 microcontroller  
    - LED controlled by a push button  
    - 6-pin ISP header for programming  
    ![](../images/day_3/view2_route.png){ width=400 }  
The schematic, component placement, and routed tracks were verified and prepared for fabrication.  
We will use this same file as the basis for PCB milling.



== "Step 1: Preparation"

- Mount the milling tool.  
- Secure the copper-clad board on the cutter bed using cell tape.  
- Download and install **Carbide Motion**.  
- In the project folder (`Microcontroller_PCB_Design`), locate the `gerber` folder with Gerber files.  
- Connect the cutter to Carbide Motion.  
- Import the Gerber files into Carbide Motion; it combines them into one file for milling.  
- Adjust the **cutter tool position**, depth, and speed configuration.  



== "Step 2: Milling the Traces"

- Set the machine origin correctly.  
- Once all configuration is done, engrave the copper traces according to the design.  
![Milling](../images/day_7/day7_1.jpeg)


== "Step 3: Cutting the Board Outline"
- Change the milling tool (spindle) to the one used for cutting the board outline.
- adjust adjust the cutter tool again (e.g position)

![Cutting](../images/day_7/day7_2.jpeg)


== "Result"

- The final PCB is ready for **cleaning and component soldering**.  

### Result
![](../images/day_7/day.jpeg)

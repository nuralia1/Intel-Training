# **Intel-CKT-Training 2023** 
## Table of contents
+ **[ Day 1 - Fundamentals of VLSI Design and overview of Sand-to-Silicon ](https://github.com/nuralia1/Intel-Training#day-1)**
+ **[ Day 2 - Analog VLSI Design Flow and CMOS Fabrication Process ](https://github.com/nuralia1/Intel-Training#day-2)**
+ **[ Day 3 - CMOS Fabrication Process in DeepSubmicron (DSM) and Ultra DeepSubmicron (UDSM) Technology ](https://github.com/nuralia1/Intel-Training#day-3)**
+ **[ Day 4 - Metal-Oxide-Semiconductor Structure ](https://github.com/nuralia1/Intel-Training#day-4)**





## **Day 1 - Fundamentals of VLSI Design and overview of Sand-to-Silicon**

<details><summary> Theory </summary>

### **Theory- Fundamentals of VLSI Design and overview of Sand-to-Silicon**



   <details><summary> Overview of VLSI Design </summary> 
   
   #### **Overview of VLSI Design**
   
* **Packaged Chip:**
    * Different types of packaging are available (SIP, DIP, QFN, BGA etc)
    * The central part of the chip is call die
    * Integrated circuits are put into protective packages to allow easy handling and assembly onto printed circuit boards and to protect the devices from damage
    * Integrated circuit packaging is the last assembly process before testing and shipping devices to customers.
    
    ![image](https://user-images.githubusercontent.com/121996204/212537263-52a2a056-f4a6-46c0-ac93-f4b922622324.png)


* **Die and Wafer:**
    * A die, in the context of integrated circuits, is a small block of semiconducting material on which a given functional circuit is fabricated
    * Generally the die size is 1mm X 1mm or 1mm X 2mm.
    * All the components fabricated on the die
    * Wafer is the round slice of silicon that the individual die (chips) are printed on. Before processing, it’s shiny and clear.
    * The wafer is cut (diced) into many pieces, each containing one copy of the circuit. Each of these pieces is called a die.
    * The wafer diameter is around 12 inch ~ 300 mm.
    * A Single wafer contains 10’s of thousands die
    
 ![image](https://user-images.githubusercontent.com/121996204/212537288-38681759-6e9c-471e-9b1b-531e57a10c10.png)


* **Inside the Die**

![image](https://user-images.githubusercontent.com/121996204/212538880-ddad0242-ec2d-4f1f-be24-5a85fd6afdd2.png)

   </details>



   <details><summary> VLSI </summary> 
      
   #### **VLSI**
      
   ##### **What is VLSI technology?**
* **Very-large-scale integration (VLSI)** is the process of creating an integrated circuit (IC) by combining millions or billions of transistors into a single chip
* VLSI is a successor to large-scale integration (LSI), medium-scale integration (MSI) and small-scale integration (SSI) technologies   

      
##### **What is VLSI mainly used for?** 
* VLSI is mainly used to design electronic components like microprocessors and memory chips
   
   </details>



   <details><summary> Moore's Law </summary>
      
#### **Moore's Law**
      
* **Moore's Law**- states that the number of transistors on a microchip doubles every two years. We can expect the speed and capability of our computers to increase       every two years because of this, yet we will pay less for them.  
      
*  In 1965, Gordon Moore predicted that transistors would continue to shrink.
   * Doubled transistor density every 2 year
   * Doubled performance density every 2 year
      
   </details>

   
   
   <details><summary> VLSI Design Methodology </summary>

#### **These are different VLSI Design styles:**

* Field programming gate array (FPGA) design
* ASIC
    * Standard cell based design (semi custom design)
    * Full custom design

      
     
#### **FPGA VS ASIC**
* **FPGA** - is a multipurpose microchip you can reprogram for multiple applications
* **ASIC** - is designed for a specific application 


|                   |     FPGA      |   ASIC      |
|  -------------    | ------------- | ----------- |
|  Time to Market   |     Fast      |    Slow     |
|    Design Flow    |    Simple     |  Complex    |
|    Unit Cost      |     High      |    Low      |
|    Performance    |     Low       |    High     |
| Power Consumption |     High      |    Low      |
|     Unit Size     |    Medium     |    Low      |
  

#### **Full custom design vs Semi custom design**
* **Full custom design** - All design and manufacturing process cycles are circuit specific
* **Semi custom design** - Some design and manufacturing cycles are predefined  

|                Full custom design                    |                                      Semi custom design                                     |
|  ------------------------------------------------    | ------------------------------------------------------------------------------------------- |
| All mask layers are customised in full custom design | It uses pre-designed logic cell (AND gates, OR gate, multiplexers) known as standard cells  |
|         Design time and complexity is higher         |                             Design time and complexity is lower                             |
|                 higher performance                   |                                       low performance                                       |
|                      high cost                       |                                          low cost                                           | 
|       less dependency on existing technology         |                       complete dependency on existing technology                            | 
|   entire design is made without use of any library   |                  design is completed with the use of multiple library                       | 

   </details>



   <details><summary> VLSI Design Quality </summary>

#### **These are the criteria to be important to measure the design quality:**
* Testability
* Yield and Manufacturability
* Reliability
* Technology Upgradability


1. **Testability:**
     * Generation of good test vector
     * Availability of good test fixture at speed
     * Design of testable chip
     
2. **Yield and Manufacturability:**
     * Yield: No. of tested ok chips/Total no. of Chips
     * Functional Yield: Checks at lower speed
     * Parametric Yield: Checks at required speed
     
3. **Reliability:**
     * ESD and EOS
     * Electromigration
     * Oxide breakdown
     * Power and ground bouncing
     * On-chip noise and cross-talk
     
4. **Technology Upgradability**
     * Rapid development of process technology results, the life span of a given technology generation has remain constant even for sub-micron technologies. 
       * This Causes:
         * Design of complex chip in a shorter time
         * Technology updated to new design rules.
         * Updating the mask to new design rules
	 
     * Design style should be chosen such that the technology update of the chip of functional module for design reuse can be achieved quickly with minimal cost.
     * Designers can develop and use advanced CAD tools that automatically generates the physical layout
   </details>
   
   
   
   <details><summary> Types of Package </summary>

#### **Types of Package**
##### **These are classified by the method used to solder the package on the PCB:**

1. **Pin-through-hole (PTH):**
     * Pin-Through-hole is a method for mounting components on a printed circuit board (PCB) in which pins on the component are inserted into holes in the board and          soldered in place.
     * This process is also known as conventional assembly.
     * not cost effective but soldering process in not inexpensive.
     
     ![image](https://user-images.githubusercontent.com/121996204/212539977-3c253941-a7d5-4c62-900f-a82109ac596a.png)
.

* **These are package types for Pin-through-hole:**

  * Dual-in-Line Package (DIPs)
  * Pin Grid Array (PGA) Packages
  * Single in-line Pin Package (SIP or SIPP)
     
     
2. **Surface Mount Technology (SMT):** 
     * Surface-mount technology, originally called planar mounting 
     * Surface-mount technology (SMT) is a method in which the electrical components are mounted directly onto the surface of a printed circuit board. An electrical          component mounted in this manner is referred to as a surface-mount device.
     * The components are attached and connected on the surface of the board using batch solder-reflow processes
     * cost and space effective but expensive equipment's are needed for soldering
     * Smaller size and reduced weight are the two main advantages to SMT
     
     ![image](https://user-images.githubusercontent.com/121996204/212540643-73dcf5b2-fbfc-4017-a5bc-9f083a09e426.png)


* **These are package types for surface mount integrated circuits:**

  * Small outline integrated circuit (SOIC)
  * Small outline package (SOP)
  * Quad flat pack (QFP)
  * Plastic leaded chip carrier (PLCC)
  * Ball grid array (BGA)
  * Chip Carrier Packages (CCP)


* **Comparison between Pin-through-hole (PTH) and Surface Mount Technology (SMT)**   

![image](https://user-images.githubusercontent.com/121996204/212540127-d8387078-15ee-49b8-8f66-5a96ff7558eb.png)


3. **Plastic:** 
     * Dominant for many years but it has the disadvantage of being permeable to environmental moisture.
     * Plastic packaging can absorb moisture in condensing atmospheres and ramped to >100C


4. **Ceramic:** 
     * In the beginning, every BGA/PGA package was based on a ceramic substrate but today laminate is a primary source for both low cost and high end applications. 
     * Power consumption, performance and environmental requirements
     * Ceramic packages are used for high temperature
     * Ceramic packages with a hollow cavity can have particle contamination from the environment or the sealing process. 


   </details>



   <details><summary> CAD Tools </summary>

#### **CAD Tools**  

The CAD technology for VLSI chip design can be categorized into the following areas:
   * High-level synthesis
   * Logic synthesis
   * Circuit optimization
   * Layout
   * Placement and routing
   * Simulation
   * Design rules and checking
   
   </details>
   </details>





<details><summary> Lab </summary>

### **Lab**
   
   <details><summary> Pre-Lab </summary>
      
   #### **Pre-Lab - How to setup**
[Pre-lab training day 1_nuraliah alwani rosli.pdf](https://github.com/nuralia1/Intel-Training/files/10379658/Pre-lab.training.day.1_nuraliah.alwani.rosli.pdf)

   </details>
   </details>
   
   
   
   
   
<details><summary> Assignment - Semiconductor Devices </summary>
 
   #### **Assignment - Semiconductor Devices**
      
**1. What is the difference between conductor, semi-conductor and insulator?**
      
|          conductor                                             |     insulator                                                |   semiconductor                     |
|  ------------------------------------------------------------- | ------------------------------------------------------------ | ----------------------------------- |
|The conductivity of conductor is high          |     The conductivity of insulator is very low   |   The conductivity of semiconductor is moderate      |
|Low resistivity                                               |Very high resistivity                                                  |    moderate resistivity     |
|It has no forbidden gap                                       |It has large forbidden gap                  |    	It has small forbidden gap     |
|Conductor has positive temperature coefficient of resistance  |insulator has negative temperature coefficient of resistance           |semiconductor has negative temperature coefficient of resistance     |
|Effect of resistance and temperature are increase             |Effect of resistance is decrease and effect of temperature is increase |Effect of resistance is decrease and effect of temperature is increase     |
|There is a large number of electrons available for conduction |There is a small number of electrons available for conduction          |There is a moderate number of electrons available for conduction     |
|Example: Metal, aluminium, copper                             |Paper, Mica glass                                                      |Silicon, Germanium     |
	



**2. Which semiconductor material used mostly for IC design and why?**
      
* Silicon is the most widely used semiconductor material as it is more efficient in producing high-speed integrated circuits. It can be used as either an insulator (doesn't allow electricity to flow) or a semiconductor (allows a little flow of electricity). This is important for making chips and very cheap. Silicon elements are able to bind atoms tightly and in complex arrangements. The abundance of silicon makes it inexpensive and easy to acquire. 




**3. What is the difference between Silicon and Germanium?**
      
|         Silicon          |     Germanium      |
|  -------------    | ------------- |
|  Silicon is the chemical element present in periodic table with atomic number 14 and represented as Si  |     Germanium is the chemical element present in the periodic table with atomic number 32 and represented as Ge      |
|       The atomic radius is smaller compared with Germanium because of smaller atomic number    |     The atomic radius is larger compared with Silicon      | 
|  Silicons are less conductive than Germanium    | Germanium is more conductive in nature |
|  Silicons are used as semiconductors as they can withstand up to higher temperature ranges.   |  Germanium cannot be used as semiconductors as they have a certain limit to temperatures  |




**5. What is doping? What are the different types of trivalent and pentavalent impurity materials?**

* **Doping**
   * **Doping** is the process of adding impurities to intrinsic semiconductors to alter their properties. 
   * The conductivity of metal is increased by adding an appropriate amount of suitable impurity. This process is known as doping. 
   * It can be performed with an impurity that is electron-rich or electron-deficient than the intrinsic semiconductor silicon or germanium.


* **Pentavalent impurities**
   * **Pentavalent impurities** are the atoms with five valence electrons used for the doping of semiconductors. 
   * For example: Arsenic (As), Phosphorous (Pi), Antimony (Sb)

* **Trivalent impurities** 
   * **Trivalent impurities** are called Acceptor impurities. Since the trivalent atoms, an element whose each atom has 3 valence electrons is called Trivalent impurity. 
   * For example: Indium ,Gallium,Aluminium,Boron
   
   


**7. What is PN junction? How it behaves without any external bias voltage?**

* A P-N junction is an interface or a boundary between two semiconductor material types, namely the p-type and the n-type, inside a semiconductor. In a semiconductor,   the P-N junction is created by the method of doping.

* Zero Bias – No external voltage potential is applied to the PN junction diode.
  * When a diode is Zero Biased no external energy source is applied and a natural Potential Barrier is developed across a depletion layer which is approximately 0.5       to 0.7v for silicon diodes and approximately 0.3 of a volt for germanium diodes.
  
  * in zero bias or thermal equilibrium state junction potential provides higher potential energy to the holes on the P-side than the N-side. If the terminals of           junction diode are shorted, few majority charge carriers (holes) in the P side with sufficient energy to surmount the potential barrier travel across the depletion     region
  
  * Therefore, with the help of holes, current starts to flow in the diode and it is referred to as forward current. In the similar manner, holes in the N side move       across the depletion region in reverse direction and the current generated in this fashion is referred to as reverse current.
  
  * The potential barrier that now exists discourages the diffusion of any more majority carriers across the junction. However, the potential barrier helps minority       carriers (few free electrons in the P-region and few holes in the N-region) to drift across the junction.
  
  * Then an “Equilibrium” or balance will be established when the majority carriers are equal and both moving in opposite directions, so that the net result is zero       current flowing in the circuit. When this occurs the junction is said to be in a state of “Dynamic Equilibrium“.
  
  * The minority carriers are constantly generated due to thermal energy so this state of equilibrium can be broken by raising the temperature of the PN junction           causing an increase in the generation of minority carriers, thereby resulting in an increase in leakage current but an electric current cannot flow since no           circuit has been connected to the PN junction
  
![image](https://user-images.githubusercontent.com/121996204/211701809-3a15381c-7622-4fc6-8624-78f0d3f9f929.png)




**8. What is built-in potential of a P-N junction?**

* The built-in potential of a P N junction diode is 0.7 V at room temperature




**13. What is BJT and how it is different from the diode?**

|                   |     diode      |   BJT      |
|  -------------    | ------------- | ----------- |
|  Definition   |     A semiconductor device in which current flows only in one direction      |    A semiconductor device which transfers the weak signal from low resistance circuit to high resistance circuit.     |
|    Symbol    |   ![image](https://user-images.githubusercontent.com/121996204/211700559-e684d5f6-bd10-489e-8d08-cb711abb5d8f.png)     |  ![image](https://user-images.githubusercontent.com/121996204/211700573-cde340a2-78e2-4e02-9c28-89ebc0a9f8d4.png)    |
|    Uses      |     The diode is used for converting the AC to DC or Rectification      |    Regulator, Amplification and Rectification      |
|    Terminal    |     Two (Anode and Cathode)       |    Three (Emitter, Base and Collector)     |
|    Switch      |     Uncontrolled      |    Controlled      |
|    Region    |     P-region and N-region: The hole is the majority charge carrier of the P-region and electrons is the majority charge carrier of the N – region of the diode    |    Emitter, Collector and Base: the base is the smallest region, and the collector is the largest region     |




**14. What is the difference between NPN and PNP BJT?**

|         NPN          |     PNP      |  
|  -------------    |  -------------    |
|  The current flows from collector terminal to emitter terminal.   |     The current flows from emitter to collector terminal.    |
|    One P-type semiconductor is sandwiched between the two N-type semiconductors    |    It is made of up two P-type material layers with N-type sandwiched between them   |
|   The current flow from the collector is generated by keeping a +ve voltage there.      |   The current flow from the emitter to collector is generated at emitter terminal by keeping a +ve voltage there      |
|    The transistor switches ON with the increase in current in the base terminal    |  The transistors switch ON when there is no current flow at the base terminal  |
| When the current is reduced in the base, the transistor doesn’t function across the collector terminal and switches OFF |     When a current is present at the base of a PNP transistor, then the transistor switches OFF.    |

![image](https://user-images.githubusercontent.com/121996204/211699607-c4f93aa1-f061-4448-9523-f69478076d73.png) 
![image](https://user-images.githubusercontent.com/121996204/211699631-37b54da6-1271-4ac9-851e-6ea81b3816cb.png)
![image](https://user-images.githubusercontent.com/121996204/211699641-b10706b0-e9d5-4b53-88cd-fe5a809d9691.png)
![image](https://user-images.githubusercontent.com/121996204/211699664-c4b858ee-445f-4377-8c75-d0be999b404d.png)




**18. What are the different types of MOSFET?**

* **MOSFETs has two classes:**
   * Enhancement mode
   * Depletion mode
   
* Each class is available as n-channel or p-channel, hence overall they tally up to four types of MOSFETs.
   * n-channel Depletion Mode
   * p-channel Depletion Mode
   * n-channel Enhancement Mode
   * p-channel Enhancement Mode

* **Depletion Mode**
When there is no voltage across the gate terminal, the channel shows maximum conductance. When the voltage across the gate terminal is either positive or negative, then the channel conductivity decreases.

* **Enhancement Mode**
When there is no voltage across the gate terminal, then the device does not conduct. When there is the maximum voltage across the gate terminal, then the device shows enhanced conductivity.

![image](https://user-images.githubusercontent.com/121996204/211695131-96d392cf-6757-4631-afaf-20aa97029517.png)




**20. What is the difference between P-channel and N-channel MOSFET?**

|         N-channel MOSFET          |     P-channel MOSFET      |
|  -------------    | ------------- |
|         N-channel MOSFET use electron flow as the charge carrier          |     P-channel MOSFET use hole flow as the charge carrier      |
|  Higher mobility    | has less mobility than electron flow |
|         Lower resistance          |     higher resistance      |
|  higher efficient    | less efficient |
|         Less heat generation          |     higher heat generation      |
|  N-channel MOSFET occupies a lesser area    | P-channel MOSFET occupies a larger area |
|         High switching device (mobility of electrons is high)          |     Low switching speed (mobility of holes is low)      |
|         Smaller in size for same complexity          |     Size will be bigger      |

![image](https://user-images.githubusercontent.com/121996204/211698278-5d31256f-503c-48ec-aeca-b089754a2e1f.png)
	


   </details>
   </details>








## **Day 2 - Analog VLSI Design Flow and CMOS Fabrication Process**

<details><summary> Theory </summary>

### **Theory- Analog VLSI Design Flow and CMOS Fabrication Process**



   <details><summary> Analog IC Design Process </summary>
	   
   #### **Analog IC Design Process**
   
![image](https://user-images.githubusercontent.com/121996204/211686158-037b81c6-6f76-42fd-b73a-23cc28e3025c.png)



|         Electrical Design          |     Physical Design      |   Test Design      |
|  -------------    | ------------- | ----------- |
| Electrical design is the process of going from the specification to a circuit solution   |     Physical design is the process of representing the electrical design in a layout consisting of many distinct geometrical rectangle at various levels      |    Test design is the process of coordinating, planning and implementing the measurement of the analog integrated circuit performance     |
| The electrical design requires active and passive device electrical models for creating the design, verifying the design and determining the robustness of the design |     The physical design needs: Entering various geometries, Follow DRC, Check LVS, Extract Parasitic     |    Types of test: Functional, Parametric, Static, Dynamic     |

   </details>




   <details><summary> Analog IC Design Process and its Relation with CAD and PDK </summary>
	   
#### **Analog IC Design Process and its Relation with CAD and PDK**
   
![image](https://user-images.githubusercontent.com/121996204/211687093-efd7621d-1be1-41fc-9022-05b951f80088.png)
   
   </details>




   <details><summary> CMOS Technology </summary>
	   
#### **CMOS Technology**
	   
|         Comparison Feature          |     BJT      |   MOSFET      |
|  -------------    | ------------- | ----------- |
| Cut-off Frequency (FT)   |     High      |    Less     |
|   Noise (at same thermal noise)    |    Less 1/f     |  More 1/f    |
|    DC Range of Operation      |     9 decades of exponential current versus VBE      |    2-3 decades of square law behaviour     |
|    Transconductance (Same Current)    |     Larger by 10X       |    Smaller by 10X     |
| Small Signal Output Resistance |     Slightly larger      |    Smaller for short channel      |
|     Switch Implementation     |    Poor    |    Good      |	
|    Capacitor    |    Voltage dependent    |    More option      |
|     Performance/Power Ratio     |    High    |    Low      |	
|     Technology Improvement     |    Slower    |    Faster      |
	  
   </details>




   <details><summary> CMOS Fabrication Process Step </summary>

   #### **CMOS Fabrication Process Step**
   
   * ##### **Process Steps:**
   1. wafer formation (sand-to-silicon)
   
   <details><summary> wafer formation (sand-to-silicon) </summary>
   
  * The basic raw material used in CMOS fabs is a wafer or disk of silicon, roughly 75 mm to 300 mm (12 inch) in diameter and less than 1 mm thick
  * Pure silicon is melted in a pot at 1400º C. 
  * A small seed containing the desired crystal orientation is inserted into molten silicon and slowly (1mm/minute) pulled out. 
  * The silicon crystal is manufactured as a cylindrical ingot. 
  * This cylinder is sawed into discs or wafers. Polishing and crystal orientation takes place later on.
   
   </details>
   
   
   
   2. Photolithography
   
   <details><summary> Photolithography </summary>
   
  * The wafer is coated with the photoresist and subjected to selective illumination through the photomask 
  * A photomask is constructed with chromium (chrome) covered quartz glass. A UV light source is used to expose the photoresist
  * It uses ultraviolet light and photomask to transfer the image from the photomask to the layer
  * Photoresist that is sensitive to light allows the pattern underneath to be selectively exposed or selectively protected
  * A developer solvent is then used to dissolve the soluble unexposed photoresist, leaving islands of insoluble exposed photoresist
  
   </details>
   
   
   
   3. Well and Channel Formation
   
   <details><summary> Well and Channel Formation </summary>
   
  * There are 4 CMOS technology processes
     * N-well process
     * P-well process
     * Twin-well process
     * Triple-well process
     
     ![image](https://user-images.githubusercontent.com/121996204/212575252-edc54c67-b9e5-4078-8c07-4cd014e5dd3d.png)
  
   </details>
   
   
   
   4. Silicon Dioxide 
   
   <details><summary> Silicon Dioxide </summary>
   
  * **Wet Oxidation**: when the oxidizing atmosphere contains water vapor.
    * for thick oxide (field oxide)
    * Fast growth rate (140 - 250 A/h)
    * The temperature is usually between 900 °C and 1000 °C
    * use for masking oxide and the LOCOS oxide
    * Higher defect
    
  * **Dry Oxidation**: when the oxidizing atmosphere is pure oxygen
    * best for thin oxide (less than 1000 A)
    * Slow growth rate (140 - 250 A/h)
    * Temperatures are in the region of 1200 °C to achieve an acceptable growth rate
    * use for MOS transistor and dielectric components (use for dielectric layer)
    * low surface state charges (low defect) and thus make ideal dielectrics for MOS transistors
  
   </details>
   
   
   
   5. Isolation 
   
   <details><summary> Isolation </summary>
   
   * CMOS process need to be isolated from one another so that they do not have unexpected interactions.
   * The transistor gate consists of a thin gate oxide layer.
   * The thick oxide used to be formed by a process called Local Oxidation of Silicon (LOCOS).
   * A problem with LOCOS-based processes is the transition between thick and thin oxide, which extended some distance laterally to form a so-called bird’s beak.
   * Starting around the 0.35 µm node, shallow trench isolation (STI) was introduced to avoid the problems with LOCOS.
   * STI forms insulating trenches of SiO2 surrounding the transistors (everywhere except the active area)
    
   </details>   
   
   
   
   6. Gate Oxide Creation 
   
   <details><summary> Gate Oxide </summary>
   
   * The next step is to form the gate oxide for the transistors. As mentioned, this is most commonly in the form of silicon dioxide (SiO2).The transistor gate             consists of a thin gate oxide layer
   * Relatively slowgrowth rates must be used to grow thin oxide films of precise thickness
   * use lower temperature at atm pressure (800 to 900 degree) or use lower than 10 atm pressure or using composite oxide films

   </details>   



   7. Gate and Source/Drain Formations
   
   <details><summary> Gate and Source/Drain Formations </summary>   
   
   * Grow gate oxide wherever transistors are required (area = source + drain + gate)
   * Deposit polysilicon on chip
   * Pattern polysilicon (both gates and interconnect)
   * Etch exposed gate oxide—i.e., the area of gate oxide where transistors are required that was not covered by polysilicon
   * Implant pMOS and nMOS source/drain regions
   
   </details> 
   
   
   
   8. Contacts and Metallization 
   
   <details><summary> Contacts and Metallization </summary>   
      
   * Contact cuts are made to source, drain, and gate according to the contact mask. 
   * Etch oxide where contact cuts are needed. These are holes etched in the dielectric after the source/drain formation.
   * Older processes commonly use aluminum (Al) for wires, although newer ones offer copper (Cu) for lower resistance.
   * Tungsten (W) can be used as a plug to fill the contact holes (to alleviate problems of aluminum not conforming to small contacts).,
   * Sputter on aluminium metal over whole wafer
   * pattern to remove excess metal, leaving wires
   
   </details> 
   
   
   
   9. Passivation
   
   <details><summary> Passivation </summary>    
   
   * The final processing step is to add a protective glass layer called passivation or over glass that prevents the ingress of contaminants.
   * Openings in the passivation layer, called overglass cuts, allow connection to I/O pads and test probe points if needed.

   </details> 
   
   
   
   10. Metrology
   
   <details><summary> Metrology </summary>    
   
   * Metrology is the science of measuring. Everything that is built in a semiconductor process has to be measured to give feedback to the manufacturing process.

   </details> 
   </details>    
   
   
   
   
   
   <details><summary> CMOS Fabrication Process </summary>  
    
* ##### **Fabrication Process**
   
   * **Step 1:** 
     * For N- well, a P-type silicon substrate is selected as a base for fabrication.
       
      ![image](https://user-images.githubusercontent.com/121996204/211259019-24347079-e183-41b3-9321-443baed27672.png)

	   
   * **Step 2 – Thermal Oxidation:** 
     * The selective diffusion of n-type impurities is accomplished using SiO2 as a barrier which protects portions of the wafer against contamination of the                substrate. SiO2 is laid out by oxidation process done exposing the substrate to high-quality oxygen and hydrogen in an oxidation chamber at approximately              10000c
     
      ![image](https://user-images.githubusercontent.com/121996204/211259036-30841c51-ed5e-41b9-bd5d-4ce916382263.png)
    
	   
   * **Step 3 – Growing of Photoresist:**
      * At this stage to permit the selective etching, the SiO2 layer is subjected to the photolithography process. In this process, the wafer is coated with a               uniform film of a photosensitive emulsion.
      
      ![image](https://user-images.githubusercontent.com/121996204/211259048-8b65aa6c-ab71-44f9-bbb7-7ca912fcf179.png)
      
	   
   * **Step 4 – Masking:** 
      * This step is the continuation of the photolithography process. In this step, a desired pattern of openness is made using a stencil. This stencil is used as a         mask over the photoresist. The substrate is now exposed to UV rays the photoresist present under the exposed regions of mask gets polymerized.
      
      ![image](https://user-images.githubusercontent.com/121996204/211259056-d54aab98-1a8d-4c1f-8f72-62b1c210b1ec.png)
      
	   
   * **Step 5 – Removal of Unexposed Photoresist:** 
      * The mask is removed and the unexposed region of photoresist is dissolved by developing wafer using a chemical such as Trichloroethylene
      
      ![image](https://user-images.githubusercontent.com/121996204/211259067-1a8d0d83-65cf-4cf1-bf6d-66ff3d926ca8.png)
      
	   
   * **Step 6 – Etching:** 
      * The wafer is immersed in an etching solution of hydrofluoric acid, which removes the oxide from the areas through which dopants are to be diffused
      
      ![image](https://user-images.githubusercontent.com/121996204/211259077-ed2fee4b-88c4-4f73-90fe-3a1780fac83d.png)
      
	   
   * **Step 7 – Removal of Whole Photoresist Layer:** 
      * During the etching process, those portions of SiO2 which are protected by the photoresist layer are not affected. The photoresist mask is now stripped off wit         chemical solvent (hot H2SO4)
      
      ![image](https://user-images.githubusercontent.com/121996204/211259089-58d5dcdb-b4e0-407d-aa0b-1a6e4b71f720.png)
      
	   
   * **Step 8 – Formation of N-well:** 
      * The n-type impurities are diffused into the p-type substrate through the exposed region thus forming an N- well
      
      ![image](https://user-images.githubusercontent.com/121996204/211259104-a1cd568b-a55d-4454-9331-f48b54cf4f8c.png)
      
	   
   * **Step 9 – Removal of SiO2:** 
      * The layer of SiO2 is now removed by using hydrofluoric acid
      
      ![image](https://user-images.githubusercontent.com/121996204/211259112-80d6c5b9-a3cd-4f32-81b7-f7d53add9c30.png)
      
	   
   * **Step 10 – Deposition of Polysilicon:** 
      * The misalignment of the gate of a CMOS transistor would lead to the unwanted capacitance which could harm circuit. So to prevent this “Self-aligned gate               process” is preferred where gate regions are formed before the formation of source and drain using ion implantation.

      ![image](https://user-images.githubusercontent.com/121996204/211259136-a4c16229-cdba-460d-9e1a-51a6d6b62b06.png)
       
      * Polysilicon is used for formation of the gate because it can withstand the high temperature greater than 80000c when a wafer is subjected to annealing methods 
      for formation of source and drain. Polysilicon is deposited by using Chemical Deposition Process over a thin layer of gate oxide. This thin gate oxide under the 
      Polysilicon layer prevents further doping under the gate region.

	   
   * **Step 11 – Formation of Gate Region:** 
      * Except the two regions required for formation of the gate for NMOS and PMOS transistors the remaining portion of Polysilicon is stripped off.

      ![image](https://user-images.githubusercontent.com/121996204/211259481-b832190e-f9bf-41d4-8923-09fa4ec0077e.png)
      
	   
   * **Step 12 – Oxidation Process:** 
      * An oxidation layer is deposited over the wafer which acts as a shield for further diffusion and metallization processes.

      ![image](https://user-images.githubusercontent.com/121996204/211259493-d71bca98-498a-4202-9bf2-eac899ce408d.png)
      
	   
   * **Step 13 – Masking and Diffusion:** 
      * For making regions for diffusion of n-type impurities using masking process small gaps are made

      ![image](https://user-images.githubusercontent.com/121996204/211259503-631422cc-b356-46f4-aa17-ec016aa77bbd.png)
      
      * Using diffusion process three n+ regions are developed for the formation of terminals of NMOS.

      ![image](https://user-images.githubusercontent.com/121996204/211259522-50d20292-dad1-4594-b6d8-9949bf06ff6c.png)
      
	   
   * **Step 14 – Removal of Oxide:** 
      The oxide layer is stripped off

      ![image](https://user-images.githubusercontent.com/121996204/211259537-24780a99-1c86-4bbb-a64d-196ef2f06f74.png)
      
	   
   * **Step 15 – P-type Diffusion:** 
      Similar to the n-type diffusion for forming the terminals of PMOS p-type diffusion are carried out

      ![image](https://user-images.githubusercontent.com/121996204/211259544-f5384f77-efb8-4661-98da-28e4589e769e.png)
      
	   
   * **Step 16 – Laying of Thick Field oxide:** 
      Before forming the metal terminals a thick field oxide is laid out to form a protective layer for the regions of the wafer where no terminals are required

      ![image](https://user-images.githubusercontent.com/121996204/211259549-03adfb06-85c8-44c0-bafe-345404245dbc.png)
      
	   
   * **Step 17 – Metallization:** 
      This step is used for the formation of metal terminals which can provide interconnections. Aluminum is spread on the whole wafer

      ![image](https://user-images.githubusercontent.com/121996204/211259559-c300ea4b-61fb-42f1-bf9b-e77436dd4e3f.png)
      
	   
   * **Step 18 – Removal of Excess Metal:** 
      The excess metal is removed from the wafer.

	   
   * **Step 19 – Formation of Terminals:** 
      In the gaps formed after removal of excess metal terminals are formed for the interconnections.

      ![image](https://user-images.githubusercontent.com/121996204/211259579-41a7b31e-1cc4-4555-ad1d-c6a659547ab4.png)

   </details>
   </details>




<details><summary> Assignment </summary>

### **Assignment**
   
   <details><summary> Assignment - Fabrication Process and Layout </summary>
      
   #### **Assignment - Fabrication Process and Layout**
   
[Fabrication-Process-and-Layout-Assignment_Nuraliah Alwani Rosli.pdf](https://github.com/nuralia1/Intel-Training/files/10391204/Fabrication-Process-and-Layout-Assignment_Nuraliah.Alwani.Rosli.pdf)

   </details>
   </details>







## **Day 3 - CMOS Fabrication Process in DeepSubmicron (DSM) and Ultra DeepSubmicron (UDSM) Technology**

<details><summary> Theory </summary>

### **Theory- CMOS Fabrication Process in DeepSubmicron (DSM) and Ultra DeepSubmicron (UDSM) Technology**



   <details><summary> Deep Submicron CMOS Process </summary> 
	   
   1. #### **Deep Submicron CMOS Process**
	   
   * DSM technology typically has a minimum channel length between 0.35µm and 0.1µm
   * DSM technology addresses the problem of excessive depletion region widths in junction isolation techniques by using shallow trench isolation
   * DSM technology may have from 4 to 8 levels of metal
   * Lightly doped drains and sources are a key aspect of DSM technology
	   
	  
	   
   2. #### **Disadvantage of the Deep Submicron CMOS Process**
   
   * Isolation of the Transistors:

     * The use of reverse bias pn junctions to isolate transistors becomes impractical as the transistor sizes decrease


	   
   3. #### **Illustration of a Deep Submicron (DSM) CMOS Technology**
	   
   * In addition to the NMOS and PMOS transistor, the DSM technology provides
	   
     * Different types of resistors in Deep Submicron (DSM) CMOS Technology:
	   
       * Diffused and/or implanted resistors
       * Well resistors
       * Poly resistors
       * Metal Resistors
	   
     ![image](https://user-images.githubusercontent.com/121996204/212593837-c4388ff6-6e95-48f6-9c4d-25393cac95d2.png)

     * Different types of capacitor in Deep Submicron (DSM) CMOS Technology:
	   
       * Metal-Insulator-Metal (MIM) Capacitor
       * Polysilicon-Polysilicon Capacitor	
	   
      ![image](https://user-images.githubusercontent.com/121996204/212594820-c14d7cd5-bec1-410a-aa2e-c5d6bfc07fb1.png)
	   
	   
   </details>     
   
   
   
   
   <details><summary> Local Oxidation of Silicon (LOCOS) </summary> 
   
   <details><summary> Local Oxidation of Silicon (LOCOS) Isolation Process </summary>   
   
#### **Local Oxidation of Silicon (LOCOS) Isolation Process**
   
* **Local Oxidation of Silicon (LOCOS)** is the traditional isolation technique used in submicron processes.


    1. A very thin layer silicon dioxide is grown on the wafer, called as pad oxide. Then a layer of silicon nitride is deposited which is used as an oxide barrier.
    2. Then photolithography is done to pattern and etch the nitride and pad oxide where the thick oxide will be grown
    3. Then by thermal oxidation process thick oxide is grown in the exposed area.
    4. The last step is the removal of the silicon nitride layer.

    ![image](https://user-images.githubusercontent.com/121996204/212211919-68cb4a83-8415-4f58-bc69-9eff855c76a5.png)

   </details>   
   
   
	   
   <details><summary> Limitation and Advantages of Local Oxidation of Silicon (LOCOS) </summary>   
   
#### **Limitation and Advantages of Local Oxidation of Silicon (LOCOS)**
   
|      **Limitation**     |     **Advantages**      | 
|  ---------------    | ------------------- | 
|  the bird’s beak effect and the surface area which is lost to this encroachment  | simple process flow and high oxide quality because the whole LOCOS structure is thermally grown  |
|  the restricted bird’s beak leads to undesirable stress effects in the transistor.    |    | 
	   
   </details>
   </details>





   <details><summary> Shallow trench isolation (STI) </summary> 
   
   <details><summary> Shallow trench isolation (STI) process </summary>    
   
   #### **Shallow trench isolation (STI)**   

* **Sallow Trench Isolation (STI)** isolation process is the preferred isolation process for deep-submicron process because it allows closer spacing of transistors by eliminating the depletion region at the surface and it completely avoids Bird’s beak shape characteristics due to LOCOS process.


   0. The STI process starts in the same way as the LOCOS process
   1. Cover the wafer with pad oxide and silicon nitride.
   2. First etch nitride and pad oxide. Next, an anisotropic etch is made in the silicon to a depth of 0.4 to 0.5 microns.
   3. Grow a thin thermal oxide layer on the trench walls the so-called as liner oxide.But unlike with LOCOS, the thermal oxidation process is stopped after the             formation of a thin oxide layer.
   4. A CVD dielectric film is used to fill the trench.
   5. A chemical mechanical polishing (CMP) step is used to polish back the dielectric layer until the nitride is reached. The nitride acts like a CMP stop layer.
   6. Densify the dielectric material at 900°C and strip the nitride and pad oxide

![image](https://user-images.githubusercontent.com/121996204/212214645-d55bee6d-7da3-483a-99d9-3540a1612b16.png)
   
   
   </details>
   
   
   <details><summary> Disadvantage and Advantages of Shallow trench isolation (STI) </summary>   
   
#### **Disadvantage and Advantages of Shallow trench isolation (STI)**
   
|      **Disadvantage**     |     **Advantages**      | 
|  ---------------    | ------------------- | 
|  larger number of process steps  | With its zero oxide field encroachment STI is more suitable for the increased density requirements in a small area because it allows forming smaller isolation regions  |
|      | advantage of STI is that it minimizes the heat cycle needed for n+ or p+ isolation compared to LOCOS | 


   </details>
   </details>



   <details><summary> Deep Submicron (DSM) CMOS Fabrication Process </summary>   
   
#### **Deep Submicron (DSM) CMOS Fabrication Process**

* **Fabrication Steps for a DSM CMOS Process**

   <details><summary> 0. Starting Material </summary>

   * The substrate should be highly doped to act like a good conductor

   ![image](https://user-images.githubusercontent.com/121996204/212584524-f9af3ffb-2f0c-4e23-adbb-904d2e1b3069.png)

   </details>
   
   
   
   <details><summary> 1. p and n wells creation </summary>

   * These are the areas where the transistors will be fabricated - NMOS in the p-well and PMOS in the n-well.
   * Done by implantation followed by a deep diffusion

   ![image](https://user-images.githubusercontent.com/121996204/212584592-f638490d-6429-47ab-93cc-612315525151.png)

   </details>
   
   

   <details><summary> 2. Shallow trench isolation </summary>

   * The shallow trench isolation (STI) electrically isolates one region/transistor from another

   ![image](https://user-images.githubusercontent.com/121996204/212584797-2c864cd9-795f-4e6b-96e1-2ddc1e0fd30f.png)

   </details>
   


   <details><summary> 3. Threshold shift and anti-punch through implants </summary>
 
   * The natural thresholds of the NMOS is about 0V and of the PMOS is about –1.2V. An p-implant is used to make the NMOS harder to invert and the PMOS easier              resulting in threshold voltages balanced around zero volts.

   * Also an implant can be applied to create a higher-doped region beneath the channels to prevent punch-through from the drain depletion region extending to source      depletion region.

   ![image](https://user-images.githubusercontent.com/121996204/212585006-2f37f404-2946-4f3e-ab62-6b45f9133d4e.png)

   </details>
   
   

   <details><summary> 4. Thin oxide and gate polysilicon </summary>

   * A thin oxide is deposited followed by polysilicon. These layers are removed where they are not wanted.

   ![image](https://user-images.githubusercontent.com/121996204/212585493-12cbb704-ccf3-406c-b04a-0299c68caecb.png)

   </details>
   


   <details><summary> 5. Lightly doped drains and sources </summary>
   
   * A lightly-doped implant is used to create a lightly-doped source and drain next to the channel of the MOSFETs.

   ![image](https://user-images.githubusercontent.com/121996204/212585745-4b5f73b7-0ba2-4d8c-92e7-1f29db2a6975.png)

   </details>
   
   

   <details><summary> 6. Sidewall spacer </summary>
   
   * A layer of dielectric is deposited on the surface and removed in such a way as to leave “sidewall spacers” next to the thin-oxide-polysilicon-polycide sandwich. 
   * These sidewall spacers will prevent the part of the source and drain next to the channel from becoming heavily doped

   ![image](https://user-images.githubusercontent.com/121996204/212585966-62662724-f93b-48ab-8f31-40aff991b143.png)

   </details>   
   
   

   <details><summary> 7. Implantation of the Heavily Doped Sources and Drains </summary>
   
   * Note that not only does this step provide the completed sources and drains but allows for ohmic contact into the wells and substrate.

   ![image](https://user-images.githubusercontent.com/121996204/212586151-51016054-994e-4d57-80dc-9487592c8678.png)

   </details>   
   
   

   <details><summary> 8. Siliciding (Salicide and Polycide) </summary>
   
   * This step reduces the resistance of the bulk diffusions and polysilicon and forms an ohmic contact with material on which it is deposited.
   * Salicide = Self-aligned silicide

   ![image](https://user-images.githubusercontent.com/121996204/212586341-d0bb3af8-7876-4db9-aad0-e31fedea4278.png)

   </details>   
   
   

   <details><summary> 9. Intermediate Oxide Layer </summary>
   
   * An oxide layer is used to cover the transistors and to planarize the surface. 

   ![image](https://user-images.githubusercontent.com/121996204/212586553-c0f0217d-3129-4c96-a089-fd99372ca013.png)

   </details>   
   
   

   <details><summary> 10. Higher level metals, tungsten plugs/vias, and oxide </summary>
   
   * Tungsten plugs are built through the lower intermediate oxide layer to provide contact between the devices, wells and substrate to the first-level metal.

   ![image](https://user-images.githubusercontent.com/121996204/212586740-cdef5755-fbd5-46f2-9eeb-7a3b56ac361f.png)

   </details>   
   
   

   <details><summary> 11. Top level metal, vias and protective oxide </summary>
   
   * The previous step is repeated for the second-level metal.
   * After multiple levels of metal are applied, the fabrication is completed with a thicker top level metal and a protective layer to hermetically seal the circuit        from the environment.
   * metal is used for the upper level metal vias. The chip is electrically connected by removing the protective layer over large bonding pads

   ![image](https://user-images.githubusercontent.com/121996204/212586959-18bc6be8-9c63-4e09-9da6-2eac55a2b938.png)

   </details>
	  
	  
   </details>
	



	
   <details><summary> Ultra Deep Submicron (UDSM) CMOS Technology </summary>
	   
   <details><summary> Ultra Deep Submicron (UDSM) CMOS Technology Features </summary>	   
	   
#### **Ultra Deep Submicron (UDSM) CMOS Technology Features**
	   
* Increased transconductance and frequency capability
* Low power supply voltages
* Reduced parasitics
* Gate leakage causes challenges for analog applications of UDSM technology
	   
   * Can no longer use the MOSFET for capacitance
   * Conflict between matching and gate leakage
	   
* Other issues
	   
   * Noise
   * Zero temperature coefficient behavior
	   
* UDSM technology typically has a minimum channel length less than 0.1µm
* UDSM transistors utilize enhanced channel strains to increase drive capability and reduce off currents
	   
	   
   </details>
	   
	   
	   
   <details><summary> Disadvantage and Advantages of Ultra Deep Submicron (UDSM) CMOS Technology </summary>   
   
   #### **Disadvantage and Advantages of Ultra Deep Submicron (UDSM) CMOS Technology**
   
|      **Disadvantage**     |     **Advantages**      | 
|  ---------------    | ------------------- | 
|      Reduction in power supply resulting in reduced headroom     |     Improved Ion/Ioff | 
|      Reduced small signal intrinsic gain    |     Reduced gate capacitance     | 
|      Increased nonlinearity     |     Higher drive current capability      | 
|      Increased noise and poorer matching     |     Reduced interconnect density      |
|      Gate leakage currents     |     Reduction of active power      | 
|           |     More levels of metal      | 
|           |     Higher cutoff frequency      | 
|           |     Higher capacitance density      | 
|           |     Reduced junction capacitance per transconductance      | 
|           |     More speed     | 

	   
	   
   #### **What is the Gate Leakage Problem**
	   
* Gate current occurs in thin oxide devices due to direct tunneling through the thin oxide


   </details>
   </details>
   </details>	
	

	
	
<details><summary> Assignment </summary>

### **Assignment**
   
   <details><summary> Assignment - DSM and UDSM Fabrication Process </summary>
      
   #### **Assignment - DSM and UDSM Fabrication Process**
   

   </details>
   </details>	
	


## **Day 4 - Metal-Oxide-Semiconductor Structure**
<details><summary> Notes </summary>

### **Notes- Fundamentals of VLSI Design and overview of Sand-to-Silicon**
   
   <details><summary>  </summary> 
	   
   </details>
   </details>
	

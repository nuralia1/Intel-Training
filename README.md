# **Intel-CKT-Training 2023** 
## Table of contents
+ **[ Day 1 - Fundamentals of VLSI Design and overview of Sand-to-Silicon ](https://github.com/nuralia1/Intel-Training#day-1---fundamentals-of-vlsi-design-and-overview-of-sand-to-silicon)**
+ **[ Day 2 - Analog VLSI Design Flow and CMOS Fabrication Process ](https://github.com/nuralia1/Intel-Training#day-2---analog-vlsi-design-flow-and-cmos-fabrication-process)**
+ **[ Day 3 - CMOS Fabrication Process in DeepSubmicron (DSM) and Ultra DeepSubmicron (UDSM) Technology ](https://github.com/nuralia1/Intel-Training#day-3---cmos-fabrication-process-in-deepsubmicron-dsm-and-ultra-deepsubmicron-udsm-technology)**
+ **[ Day 4 - Metal-Oxide-Semiconductor Structure ](https://github.com/nuralia1/Intel-Training#day-4---metal-oxide-semiconductor-structure)**

+ **[ Day 5 - Metal-Oxide-Semiconductor Field Effect Transistor ](https://github.com/nuralia1/Intel-Training#day-5---metal-oxide-semiconductor---field-effect-transistor)**




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
   
[Day3-Assignment-DSM-and-UDSM-Fabrication-Process_nuraliah alwani rosli.pdf](https://github.com/nuralia1/Intel-Training/files/10430115/Day3-Assignment-DSM-and-UDSM-Fabrication-Process_nuraliah.alwani.rosli.pdf)

   </details>
   </details>	









## **Day 4 - Metal-Oxide-Semiconductor Structure**

<details><summary> Theory </summary>

### **Theory- Metal-Oxide-Semiconductor Structure**



   <details><summary>  MOS Capacitor </summary> 
	   
* **Metal-Oxide-Semiconductor (MOS) Junction**

1. MOS junction simply a capacitor
	   
2. No current-voltage relationship, only capacitor-voltage relationship 
  
3. Also call as MOSCAP   
   * M - O - S  = Metal - Oxide - Semiconductor
   * CAP = because the oxide which is insulator is sandwich between a conductor and semiconductor which will act as capacitor
	   
| Metal  |used polysilicon that is used as a gate| 	   
|  ---------------    | ------------------- | 	   
|  **Insulator**  | **that is used is silicon dioxide (SiO2) which we call as Oxide** | 
|  **Semiconductor**  | **that is used is silicon** | 
	   
![image](https://user-images.githubusercontent.com/121996204/214475556-06dd6bcd-672f-4139-beeb-c95558ba1065.png)
	   
![image](https://user-images.githubusercontent.com/121996204/216503309-8b4b3b6d-ab6e-40b5-9280-015231022fcb.png)
   
   </details>

	
	
	
	
   <details><summary> Ideal MOS Capacitor </summary> 
	   
   #### **Ideal MOS Junction or Capacitor**	
	   
|      **Ideal**     | 
|  ---------------    | 
|  the work function of metal and semiconductor are the same = 0  |  
|  Oxide has no charges inside or the oxide is free of charges  |  
|  the substrate is uniformly doped  |  
|  Oxide has infinite resisitivity which mean there cannot be current flowing through the oxide when we do the operation  |  

![image](https://user-images.githubusercontent.com/121996204/216503465-a74f53a2-d26b-46e4-867b-d073ba3b24dc.png)

	   
* **Energy band diagram of Ideal MOS Junction or Capacitor**
	   
![image](https://user-images.githubusercontent.com/121996204/216505127-eaa58c38-f782-4267-864a-9dd73b8ebb4e.png)
	   
   </details>

	
	
	
	
	
	
   <details><summary> Principle of operation </summary> 
	   
* The four modes of operation of an MOS structure:
1. Case1: (V < 0) = Accumulation
		 
   <details><summary> Accumulation </summary> 
	   
   **Accumulation Mode (V < 0):**
	
   * below the flatband voltage, VFB is called as Accumulation mode of operation			 
   * Pile of majority carrier at the interface
   * Charge at the surface directly proportional to voltage	
   * Accumulation occurs typically for -ve voltages where the -ve charge on the gate attracts holes from the substrate to the oxide-semiconductor interface.
		 				 
   ![image](https://user-images.githubusercontent.com/121996204/216512360-9a2be14a-11c3-4381-b954-a654736e486e.png)
				 
   ![tempsnip](https://user-images.githubusercontent.com/121996204/217410452-350aaa69-0409-4250-81f4-8e6c56f099aa.png)

				 				 
   </details>
	   
	   
	   
2. Case2: (V > 0) = Depletion and weak inversion
	   
   <details><summary> Depletion </summary> 

   **Depletion Mode (V > 0):**
				 
   * between the flatband voltage and the threshold voltage, VT is called as Depletion mode of operation 
   * Depletion occurs for positive voltages.
   * The +ve charge on the gate pushes the mobile holes into the substrate.
   * Therefore, the semiconductor is depleted of mobile carriers at the interface and a -ve charge, due to the ionized acceptor ions, is left in the space charge          region
   * The voltage at which the surface carrier concentration is exactly equal to bulk carrier concentration, is called weak inversion voltage and from this point the        weak inversion started.
   * Charge at the surface directly proportional to voltage
   * The voltage at which the surface concentration exactly equal to the bulk concentration, that is called threshold voltage

   ![image](https://user-images.githubusercontent.com/121996204/217412009-e2fb7ed3-238b-419c-ba7b-e4102af35dec.png)

   ![image](https://user-images.githubusercontent.com/121996204/217412079-b84d098e-458c-4cb5-b996-33401410be57.png)

   </details>	   
	   
	   
	   
3. Case3: (V ≥ VT) = Strong inversion

   <details><summary> Inversion </summary> 
   
   **Inversion Mode (V ≥ VT):**
	   
   * larger than the threshold voltage is called as Inversion mode of operation   
   * At threshold voltage a channel form at the surface of the semiconductor due to inversion charges.
   * Before threshold voltage the charge comes from negatively charged ionized acceptors.
   * After threshold voltage, the more charge comes from the electrons rather than depleting the holes.
   * Inversion occurs at voltages beyond the threshold voltage.	 
   * In inversion, there exists a negatively charged inversion layer at the oxide semiconductor interface in addition to the depletion-layer.
   * This inversion layer is due to minority carriers, which are attracted to the interface by the positive gate voltage  
	    
   ![image](https://user-images.githubusercontent.com/121996204/217424851-abe04d89-a01b-4a7a-9b4a-48aa97e03a0f.png)
  
   ![image](https://user-images.githubusercontent.com/121996204/217424739-c8e1a40d-2a44-4d97-bbfd-a1078ac539f0.png)
	   
	   
   </details>

	   
	   
4. Flat-band and Threshold voltage	   

   <details><summary> Threshold voltage and Flat-band </summary> 

   **Flat-band:**
 
   * Flatband conditions exist when no charge is present in the semiconductor so that the Si energy band is flat	 
   * Flat band means flatness of conduction and valence band edges at semiconductor surface  
   * The voltage separating the accumulation and depletion regime is referred to as the flatband voltage, VFB.
   * The flatband voltage is obtained when the applied gate voltage equals the workfunction difference between the gate metal and the semiconductor.
   * If there is a fixed charge in the oxide and/or at the oxide-silicon interface, the expression for the flatband voltage must be modified accordingly.
	      
   ![image](https://user-images.githubusercontent.com/121996204/217428109-7155ecf7-bc14-46e6-9e92-d10f937d727e.png)
	
	   
   </details>
   </details>


	  

	   
   <details><summary> C-V Characteristic </summary> 

    * This frequency dependence occurs primarily in inversion since a certain time is needed to generate the minority carriers in the inversion layer.
    * Thermal equilibrium is therefore not immediately obtained.
    * Capacitance depends on frequency of applied signal.
    * If speed of variation is slow enough so that electrons can be generated by thermal generation fast enough to be created in phase with applied signal, then Cs is       very large
    * A very low frequency, the recombination-generation kinetics of electrons can vary in response to the vltage variations, therefore capacitance resembles thatof         the parallel plate capacitor


   ![image](https://user-images.githubusercontent.com/121996204/217453095-e1d1118c-2162-4f82-b1bb-932a6a4c6638.png)	   
	   
   </details>
	   
	
	
	
	
	
   <details><summary> Non-Ideal MOS Capacitor </summary> 

   #### **Non-Ideal MOS Junction or Capacitor**	   
	   
   1. Effect of fixed charge Qf
      * To cerate a zero charge on silicon a negative voltage is required to give at gate terminal.
      * By applying a negative volute at gate the surface charge at silicon will be zero.
      * Zero charge in the semiconductor corresponds to flat-band condition of a MOS junction.	   

	   
   2. Effect of work metal-semiconductor work function difference ϕms
      * Electrons are always moves from higher energy level to lower energy level.
      * Electrons are transferred through wire.
      * To remove the electrons from semiconductor surface we have to provide a –ve voltage to the gate.
	   
   </details>
   </details>

	   
	   
	   
	   
	   
	   
<details><summary> Assignment </summary>

### **Assignment**
   
   <details><summary> Assignment - Metal-Oxide-Semiconductor Structure </summary>
      
   #### **Assignment - Metal-Oxide-Semiconductor Structure**
   
[Day4-Assignment-Metal-Oxide-Semiconductor-Structure_nuraliah alwani rosli.pdf](https://github.com/nuralia1/Intel-Training/files/10680792/Day4-Assignment-Metal-Oxide-Semiconductor-Structure_nuraliah.alwani.rosli.pdf)


   </details>
   </details>








## **Day 5 - Metal-Oxide-Semiconductor - FIELD EFFECT TRANSISTOR**

<details><summary> Theory </summary>

### **Theory- Metal-Oxide-Semiconductor - FIELD EFFECT TRANSISTOR**

   <details><summary> MOSFET </summary> 
	   
   * **MOSFET**

      * Metal Oxide Semiconductor Field Effect Transistors commonly known as MOSFET
      * MOSFET is a semiconductor device that is widely used for switching purposes and for the amplification of electronic signals in electronic devices. 
      * It is a voltage controlled device and is constructed by four terminal which are: source(S), gate (G), drain (D) and body (B) terminals
      * In general, The body of the MOSFET is in connection with the source terminal thus forming a three-terminal device such as a field-effect transistor

	   
![image](https://user-images.githubusercontent.com/121996204/217461966-77ebe569-8e70-4f0c-852b-584313996072.png)

![image](https://user-images.githubusercontent.com/121996204/217476909-8c7e786b-9ef6-4ffb-a108-6f7e2d7f95a4.png)	   
	   
   </details>	   	   
	  
	   
	 
	   

   <details><summary> MOSFET Types </summary> 
	   
* **MOSFET Types**	
	   
    * MOSFETs are of two classes: Enhancement mode and depletion mode. 
	   
   <details><summary> 1. Depletion Mode </summary> 	   
	   
   * **Depletion Mode**
	   
     * When there is no voltage across the gate terminal, the channel shows its maximum conductance. Whereas when the voltage across the gate terminal is either             positive or negative, then the channel conductivity decreases. 

   </details>	   
	
	   
	   
   <details><summary> 2. Enhancement Mode </summary> 	  
	   
   * **Enhancement Mode**
	   
     * When there is no voltage across the gate terminal, then the device does not conduct. When there is the maximum voltage across the gate terminal, then the              device shows enhanced conductivity

   </details>	  
	   
	   
    * Each class is available as n-channel or p-channel, hence overall they tally up to four types of MOSFETs
    * Now with respect to the working principle, MOSFET is classified as follows:

      * P-Channel Depletion MOSFET
      * P-Channel Enhancement MOSFET
      * N-Channel Depletion MOSFET
      * N-Channel Enhancement MOSFET   
	   
![image](https://user-images.githubusercontent.com/121996204/217478342-be9a56ba-f98c-45c6-b001-d370291622fa.png)
	   
   </details>		   
      
	   
   <details><summary>  MOSFET Operation (N-Channel and P-Channel) </summary> 
	   
* **MOSFET Operation (N-Channel and P-Channel)**
	   
   <details><summary> 1. MOSFET Operation (N-Channel) </summary> 
	   
   * **MOSFET Operation (N-Channel)**

      * The drain and source are heavily doped N+ region and the substrate is p-type. The current flows due to the flow of negatively charged electrons and that’s why         known as n-channel MOSFET. 

      * When we apply the positive gate voltage, the holes present beneath the oxide layer experience repulsive force, and the holes are pushed downwards into the             bound negative charges which are associated with the acceptor atoms. 

      * The positive gate voltage also attracts electrons from the N+ source and drain region into the channel thus an electron reach channel is formed.
	   
   ![image](https://user-images.githubusercontent.com/121996204/217480456-7c26afd8-8526-46f9-aace-c29fbbd77f7e.png)

   ![image](https://user-images.githubusercontent.com/121996204/217484987-9abaef3d-5e36-4efb-a412-a70b2c462ef8.png)
	   
   </details>		   
	 
	   
	   
   <details><summary> 2. MOSFET Operation (P-Channel) </summary> 
	   
   * **MOSFET Operation (P-Channel)**
	   
      * The drain and source are heavily doped p+ region and the substrate is in n-type. The current flows due to the flow of positively charged holes, and that’s why         known as p-channel MOSFET. 

      * When we apply negative gate voltage, the electrons present beneath the oxide layer experience repulsive force and are pushed downward into the substrate, the         depletion region is populated by the bound positive charges which are associated with the donor atoms. 

      * The negative gate voltage also attracts holes from the P+ source and drain region into the channel region.
	   
   ![image](https://user-images.githubusercontent.com/121996204/217480349-53eb46b4-a023-4462-a53d-329c279f7fec.png)

   ![image](https://user-images.githubusercontent.com/121996204/217484332-a715f9e4-d74a-4cf6-8318-53de51a8326f.png)
	   

   </details>	
 
	   
   ![image](https://user-images.githubusercontent.com/121996204/217471255-58f3d85b-eaa0-49a5-95f0-fb2e0237ad95.png)
	   
   </details>		  
	   	
  
	   
 

	   
	   
	
	   
	   
	   
	   
   <details><summary>  MOSFET Regions of Operation </summary> 	   
	   
   * **MOSFET Regions of Operation**	   
	   
   <details><summary> 1. MOSFET in cutoff mode of operation </summary> 

  1. MOSFET in cutoff mode of operation
	
      * It is the region where the device will be in the OFF condition and there zero amount of current flow through it. 
      * Here, the device functions as a basic/open switch and is so employed as when they are necessary to operate as electrical switches	   
	   
   ![image](https://user-images.githubusercontent.com/121996204/217459119-844b0eab-ce11-43f1-a6aa-d6e075c54f53.png)

   ![image](https://user-images.githubusercontent.com/121996204/217486340-a48af3d8-9efd-48c5-8cf8-d2d6a9168f6e.png)
	   
   </details>
	
	   
	   
   <details><summary> 2. MOSFET in linear or triode mode of operation </summary> 

   2. MOSFET in linear or triode mode of operation

      * It is the region where the current across the drain to source terminal enhances with the increment in the voltage across the drain to source path. 
      * When the MOSFET devices function in this linear region, they perform amplifier functionality.
	
   ![image](https://user-images.githubusercontent.com/121996204/217459184-d18a3e54-7830-48fa-971d-26224eb30f52.png)	

   ![image](https://user-images.githubusercontent.com/121996204/217486376-686400f7-3419-4415-8b98-7ade12b3bfaf.png)
	   
   </details>
	   
	   
	   
   <details><summary> 3. MOSFET in saturation mode of operation </summary> 

   3. MOSFET in saturation mode of operation
	
      * In this region, the devices will have their drain to source current value as constant without considering the enhancement in the voltage across the drain to           source. 
      * This happens only once when the voltage across the drain to source terminal increases more than the pinch-off voltage value. 
      * In this scenario, the device functions as a closed switch where a saturated level of current across the drain to source terminals flows. 
      * Due to this, the saturation region is selected when the devices are supposed to perform switching.	
	
   ![image](https://user-images.githubusercontent.com/121996204/217459249-674efd9b-88c4-4015-b698-9bff7276aed5.png)

   ![image](https://user-images.githubusercontent.com/121996204/217486420-1a06c3c6-7eec-4c10-88d1-dcfbcb495855.png)

   </details>
   </details>	   
   </details>
	
	
	
	
	
	
	
	
	
	
	
	
	
## **Day 6 - MOSFET Intrinsic Capacitances**

<details><summary> Theory </summary>

### **Theory- MOSFET Intrinsic Capacitances**

	
	
	
   <details><summary> MOSFET Intrinsic Capacitance: Cutoff Region </summary> 
	   
   * **MOSFET Intrinsic Capacitance: Cutoff Region**

       * Cutoff:
         * no channel capacitance
         * Only gate-to-bulk capacitance (High value)
	   
![image](https://user-images.githubusercontent.com/121996204/217684829-45b9b160-23a0-4cea-aafb-ab3262225f3e.png)
	   
	   
   </details>	  
	
	
   <details><summary> MOSFET Intrinsic Capacitance: Linear Region </summary> 
	   
   * **MOSFET Intrinsic Capacitance: Linear Region**

       * Linear:
         * Cgsch, Cgdch : Gate-to-channel at source side and gate-to-channel at drain side
         * Voltage dependent
         * ![image](https://user-images.githubusercontent.com/121996204/217688440-ee824edb-86cb-439e-8bbe-d3f299c8a99c.png)

	   
![image](https://user-images.githubusercontent.com/121996204/217684886-47c9c833-199d-4ed3-b43f-ee0b72227003.png)
	   
	   
	   
   </details>	
	
	

	
   <details><summary> MOSFET Intrinsic Capacitance: Saturation Region </summary> 
	   
   * **MOSFET Intrinsic Capacitance: Saturation Region**

       * Saturation:
         * Cgsch : Gate-to-channel at source side
         * No drain side capacitance because of pinch-off
         * ![image](https://user-images.githubusercontent.com/121996204/217689196-1614ed3e-73b4-4c76-804c-d1838e730911.png)

	   
![image](https://user-images.githubusercontent.com/121996204/217689254-6692effc-96bb-4475-8d69-17f8b3fba3b4.png)

	   
	   
   </details>	
	

	
	
	
	
	
   <details><summary> Schematic Design, Circuit Simulation, Layout Design and Postlayout Simulation </summary> 
	   
   * **Schematic Design, Circuit Simulation, Layout Design and Postlayout Simulation**

      * **Custom IC Design Process**
	   
![image](https://user-images.githubusercontent.com/121996204/217685349-5a915b5f-0d70-41f1-bc7a-1241a1d5d236.png)

	   
	   
	   
	   
   * **Custom IC Design Flow using Tools**	
	   
|      **Schematic Drawing Phase**     | 
|  ---------------    | 
|  Step-1: Schematic entry |  
|  Step-2: Symbol creation |  	   
|  Step-3: Create testbench for simulation |  	   

|      **Circuit Simulation Phase**     | 
|  ---------------    | 
|  Step-4: Launch ADE-L |  
|  Step-5: Select simulation type:DC operating point sim, DC sweep simulation, Transient Simulation and AC simulation|  	   
|  Step-6: Plot waveforms and use calculators to plot for some predefined functions (rise time, fall time, delay, derivative, gain margin, phase margin etc) |  
|  Step-7: Do parametric simulation (vary two variable at a time) |  
	   
	   
|      **Layout Design and Verification Phase**     | 
|  ---------------    | 
|  Step-8: Generate layout from schematic |  
|  Step-9: Place the components |  	   
|  Step-10: Routing between the components, supply and ground. |  
|  Step-11: Verify the layout with the design rule (DRC). |  	   
|  Step-12: Verify the layout with schematic (LVS) |  
|  Step-13: Extract the parasitic and create a schematic view of the that extracted netlist |  	   
	   
|      **Post Layout Simulation Phase**     | 
|  ---------------    | 
|  Step-14: Create config view |  
|  Step-15: Do the simulation for both views and compare the result. Follow same process as you have done pre-layout simulation. Only difference is instead of schematic netlist you will use parasitic extracted netlist.   |  	   
   
   </details>	

	

	
  <details><summary> Custom IC Design Flow </summary> 	
	  
  <details><summary> Custom IC Design Flow: Schematic Phase </summary> 
	   
   * **Custom IC Design Flow: Schematic Phase**

![image](https://user-images.githubusercontent.com/121996204/217701961-5f8891c3-60bf-4ca3-aa77-bbc64f67e194.png)
	  
   </details>		

	

  <details><summary> Custom IC Design Flow: Simulation Phase </summary> 
	   
   * **Custom IC Design Flow: Schematic Phase**

![image](https://user-images.githubusercontent.com/121996204/217702390-7d331a06-70cb-4df3-ab27-12130640bdc1.png)

	  
   </details>		

	  
	  
  <details><summary> Custom IC Design Flow: Simulation Phase (AC and Transient) </summary> 
	   
   * **Custom IC Design Flow: Simulation Phase (AC and Transient)**

![image](https://user-images.githubusercontent.com/121996204/217702657-52d5351e-d045-4979-bab2-902da6b939fe.png)

	  
   </details>		
	
	
	  
  <details><summary> Custom IC Design Flow: Layout Phase (Generate from Source) </summary> 
	   
   * **Custom IC Design Flow: Layout Phase (Generate from Source)**

![image](https://user-images.githubusercontent.com/121996204/217702737-ee957eea-6cf7-4563-b19c-f07d59a260f2.png)


	  
   </details>	
   </details>	
   </details>		  
	  
	  
	  
	  




	  
	  
	
## **Day 7 - CMOS Inverter**

<details><summary> Theory </summary>

### **Theory- CMOS Inverter**

	
	
	
   <details><summary> CMOS Inverter </summary> 
	   
   * **CMOS Inverter**

      * Complementary Metal oxide semiconductor inverter consists of an n-MOS transistor and p-MOS transistor as a load 
      * the gates of the two transistors are shorted at the input  
      * the drains of the two transistors are also shorted where the output is obtained
      * the source n-MOS and p-MOS transistors of the CMOS Inverter are connected to the ground and supply respectively

   * this gate with respect to different design matrices such as:
	   
      * Cost: Expressed by the complexity and area  
      * Integrity and robustness: Expressed by the static (steady-state) behavior.
      * Performance: Determined by the dynamic (or transient) response.
      * Energy Efficiency: Set by the energy and power consumption

	   
![image](https://user-images.githubusercontent.com/121996204/217683651-38ba1daf-f8dc-4f8d-9673-b701a4324ab4.png)

   </details>	
	
	

	
	
   <details><summary> CMOS Inverter: Static Characteristics </summary> 
	   
   * **CMOS Inverter: Static Characteristics**

      * When Vin is high and equal to VDD, the n-MOS transistor is ON while P-MOS is off.
      * On the other hand, when the input voltage is 0V, n-MOS and p-MOS transistors are OFF and ON respectively.
      * Here High and low levels refer to VDD and grounds respectively. 
      * It means the voltage swing (Rail-to-rail swing) is the same as the voltage supply. This leads to a high noise margin.	 
      * In steady state there is always exist a path with a fine resistance between the output and either VDD or Ground. This results low output impedance and less           sensitive to noise.
      * Input impedance of the CMOS inverter is extremely high. Theoretically, a single inverter can drive infinite number of gates.
      * No direct path exit between supply and ground. Static power almost zero.
   
![image](https://user-images.githubusercontent.com/121996204/217706823-c7e3534c-f704-4925-b7b1-74a31202fe17.png)

![image](https://user-images.githubusercontent.com/121996204/217706544-3abbcf6d-4215-4f3d-ae65-84e4e22c9df4.png)

   </details>
	
	
	
	
	
	
   <details><summary> CMOS Inverter: MOSFET Strength Variation </summary> 
	   
   * **CMOS Inverter: MOSFET Strength Variation**
	   
        * ![image](https://user-images.githubusercontent.com/121996204/217711721-4e2d8caf-1138-48b5-a4fb-cd14b22bf33d.png)
	   
|         NMOS          |     PMOS      |   TRANSITION      |
|  -------------    | ------------- | ----------- |
|  weak   |     weak      |    less slope     |
|    strong    |    strong     |  more slope    |
|    weak      |     strong      |    right shift      |
|    strong    |     weak       |    left shift     |
  

   </details>	 
	
	
	
	
   <details><summary> CMOS Inverter: Noise Margin </summary> 
	   
   * **CMOS Inverter: Noise Margin**
	   
       * The characteristics of an inverter define the allowable noise voltage on the input of the gate so that output will not be affected.
	   
         * Transition Region: 𝑉𝐼𝐻−𝑉𝐼𝐿
	   
         * 𝑉𝐼𝐻−𝑉𝐼𝐿=((𝑉0𝐿−𝑉𝑂𝐻)/𝐺𝐴𝐼𝑁)=−𝑉𝐷𝐷/𝐺𝐴𝐼𝑁
	   
         * 𝑉𝐼𝐻=𝑉𝑀+((0−𝑉𝑀)/𝐺𝐴𝐼𝑁)
	   
         * 𝑉𝐼𝐿=𝑉𝑀−((𝑉𝑀−𝑉𝐷𝐷)/𝐺𝐴𝐼𝑁)
	   
         * Noise Margin High: 𝑁𝑀𝐻=𝑉𝐷𝐷−𝑉𝐼𝐻
	   
         * Noise Margin Low: 𝑁𝑀𝐿= 𝑉𝐼𝐿
	   
         * ![image](https://user-images.githubusercontent.com/121996204/217710343-7a6ec536-b3ca-4dcc-98aa-defe8a9cae76.png)



   </details>		
	

	
	
   <details><summary> CMOS Inverter: Dynamic Characteristics </summary> 
	   
   * **CMOS Inverter: Dynamic Characteristics**

      * ![image](https://user-images.githubusercontent.com/121996204/217716366-da2aeaa1-9281-40c4-b170-c108004100a2.png)



   </details>	
	
	
	
	
	
	
   <details><summary> CMOS Inverter: Dynamic Characteristics </summary> 
	   
   * **CMOS Inverter: Dynamic Characteristics**

      * ![image](https://user-images.githubusercontent.com/121996204/217716366-da2aeaa1-9281-40c4-b170-c108004100a2.png)



   </details>	
	
	
	
	
	
	
   <details><summary> CMOS Inverter: Dynamic Characteristics </summary> 
	   
   * **CMOS Inverter: Dynamic Characteristics**

      * ![image](https://user-images.githubusercontent.com/121996204/217716366-da2aeaa1-9281-40c4-b170-c108004100a2.png)



   </details>	

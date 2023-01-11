# **Intel-CKT-Training 2023** 
## Table of contents
+ **[ Day 1 - Fundamentals of VLSI Design and overview of Sand-to-Silicon ](https://github.com/nuralia1/Intel-Training#day-1)**
+ **[ Day 2 - Analog VLSI Design Flow and CMOS Fabrication Process ](https://github.com/nuralia1/Intel-Training#day-2)**

## **Day 1**
<details><summary> Notes </summary>

### **Notes- Fundamentals of VLSI Design and overview of Sand-to-Silicon**
   
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


   </details>

<details><summary> Lab </summary>

### **Lab**
   
   <details><summary> Pre-Lab </summary>
      
   #### **Pre-Lab - How to setup**
[Pre-lab training day 1_nuraliah alwani rosli.pdf](https://github.com/nuralia1/Intel-Training/files/10379658/Pre-lab.training.day.1_nuraliah.alwani.rosli.pdf)

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


## **Day 2**
<details><summary> Notes </summary>

### **Notes- Analog VLSI Design Flow and CMOS Fabrication Process**
	
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
	
   <details><summary> CMOS Fabrication Process </summary>

   #### **CMOS Fabrication Process**
   
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
  
   </details>
   
   4. Silicon Dioxide 
   
   <details><summary> Silicon Dioxide </summary>
   
  * Wet Oxidation : when the oxidizing atmosphere contains water vapor.
    * for thick oxide (field oxide)
    * Fast growth rate (140 - 250 A/h)
    * The temperature is usually between 900 °C and 1000 °C
    * use for masking oxide and the LOCOS oxide
    * Higher defect
    
  * Dry Oxidation: when the oxidizing atmosphere is pure oxygen
    * best for thin oxide (less than 1000 A)
    * Slow growth rate (140 - 250 A/h)
    * Temperatures are in the region of 1200 °C to achieve an acceptable growth rate
    * use for MOS transistor and dielectric components (use for dielectric layer)
    * low surface state charges (low defect) and thus make ideal dielectrics for MOS transistors
  
   </details>
   
   5. Isolation 
   6. Gate Oxide Creation 
   7. Gate and Source/Drain Formations
   8. Contacts and Metallization 
   9. Passivation
   10. Metrology
   
   
   * ##### **Fabrication Process**
   
   * **Step 1:** 
     * For N- well, a P-type silicon substrate is selected as a base for fabrication.
       
      ![image](https://user-images.githubusercontent.com/121996204/211259019-24347079-e183-41b3-9321-443baed27672.png)
   
   * **Step 2 – Thermal Oxidation:** 
     * The selective diffusion of n-type impurities is accomplished using SiO2 as a barrier which protects portions of the wafer against contamination of the                  substrate. SiO2 is laid out by oxidation process done exposing the substrate to high-quality oxygen and hydrogen in an oxidation chamber at approximately 10000c
     
      ![image](https://user-images.githubusercontent.com/121996204/211259036-30841c51-ed5e-41b9-bd5d-4ce916382263.png)
       
   * **Step 3 – Growing of Photoresist:**
      * At this stage to permit the selective etching, the SiO2 layer is subjected to the photolithography process. In this process, the wafer is coated with a uniform         film of a photosensitive emulsion.
      
      ![image](https://user-images.githubusercontent.com/121996204/211259048-8b65aa6c-ab71-44f9-bbb7-7ca912fcf179.png)
      
   * **Step 4 – Masking:** 
      * This step is the continuation of the photolithography process. In this step, a desired pattern of openness is made using a stencil. This stencil is used as a           mask over the photoresist. The substrate is now exposed to UV rays the photoresist present under the exposed regions of mask gets polymerized.
      
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
   
<details><summary> Lab </summary>

### **Lab**
   
   <details><summary> Assignment - Fabrication Process and Layout </summary>
      
   #### **Assignment - Fabrication Process and Layout**
   
[Fabrication-Process-and-Layout-Assignment_Nuraliah Alwani Rosli.pdf](https://github.com/nuralia1/Intel-Training/files/10391204/Fabrication-Process-and-Layout-Assignment_Nuraliah.Alwani.Rosli.pdf)

   </details>
   </details>

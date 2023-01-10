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
      
      

   </details>
   </details>


## **Day 2**
<details><summary> Notes </summary>

### **Notes- Analog VLSI Design Flow and CMOS Fabrication Process**
	
   <details><summary> Analog IC Design Process </summary>
	   
   #### **Analog IC Design Process**
|         Electrical Design          |     Physical Design      |   Test Design      |
|  -------------    | ------------- | ----------- |
| Electrical design is the process of going from the specification to a circuit solution   |     Physical design is the process of representing the electrical design in a layout consisting of many distinct geometrical rectangle at various levels      |    Test design is the process of coordinating, planning and implementing the measurement of the analog integrated circuit performance     |
| The electrical design requires active and passive device electrical models for creating the design, verifying the design and determining the robustness of the design |     The physical design needs: Entering various geometries, Follow DRC, Check LVS, Extract Parasitic     |    Types of test: Functional, Parametric, Static, Dynamic     |

Test Design:
• Test design is the process of
coordinating, planning and
implementing the
measurement of the analog
integrated circuit
performance
• Types of test:
• Functional
• Parametric
• Static
• Dynamic

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
   2. Photolithography
   3. Well and Channel Formation
   4. Silicon Dioxide 
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

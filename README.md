# VLSI-LAB-EXP-6

# AIM:

  To create,simulate the  design of CMOS inverter,NAND,NOR from schematic  using cadence. 

# APPARATUS REQUIRED:

   cadence

# PROCEDURE:
~~~
## Commands to get into Cadence

1.	Right Click and open the terminal window
2.	Type the following commands as follows and press enter.
          i)	tcsh
          ii)	source /home/install/cshrc
          iii)	virtuoso 
## Procedure for Schematic simulation using Cadence
1.	Now two windows must open i)virtuoso/command interpreter window ii)”Whats New…”
2.	Close the 2nd window
3.	Use 1st window i.e virtuoso window(CIW) for further processing.
          i)	Create a New Library
          ii)	Create Schematic Cell view.
          iii)	Create the Symbol for schematic Cell view.
          iv)	Create the test Cell view.
          v)	Analog simulation by spectre
## Procedure for Creating New Library.
a)	File –New – Library
b)	Name : Give name for ur library Ex: VLSILAB , Enable Attach to an existing technology library, Click OK
c)	Attach the library to the technology library gpdk045.Click OK
## Create Schematic Cell view.
a)	Go to 1st window i.e virtuoso(CIW)
b)	File-New-Cell view
c)	Setup the new file form, Library: Select the one you a created. Cell : Give the experiment name Ex: Inverter View: Schematic
d)	Type: Schematic press OK
e)	Add the required components from the libraries and make the connections.
f)	Go to instance fixed menu or use shortcut key “I” from keypad to go instances Click on browse. This opens the library browser ow select the appropriate library for components like Gpdk045,nmos, pmos
g)	Analog library	Vdd, Gnd, Vcc, Vpulse, Vsin
h)	Make the connections by using fixed narrow wire key
i)	Click Check and Save button


## Creating the Symbol for schematic Cell view
a.	In the schematic window, execute
          Crate – Cell view – From Cell view
          The cell view from cell view window appears
          Check Lib Name, Cell Name, From View name must be schematic Press ok
b.	Now Symbol generation form appears. Click Ok If No changes required
c.	A new window with with default symbol is created.
d.	Edit the symbol if you want to give actual symbol shape else continue.
          i.	Execute Create-Cell view-from cell view
          ii.	Library Name and Cell Name must be same which you have used for schematic. Press OK
          iii.	Check for the position of pin side.Prss OK
          iv.	Edit for the shape by Create-Shape-Choose required options to edit.
## Creating the new test cell view

a)	Go to CIW window, Execute File-New-Cell view
b)	Setup the new file form
Library: Select the one you a created.
          Cell: Cell name must be different from the name used in schematic cell view. Ex: Inverter_test
          View: Schematic
          Type: Schematic  press OK
## Analog simulation by SPECTRE.
a.	In test cell view window
i.	Launch – ADE L(Analog Design Environment)
b.	Execute Setup—Simulation/directory/Host A new window opens
c.	Set the simulation window to spectre and click ok
d.	Execute Setup-Model Library. Anew window opens, Check of gpdk.scs as lib and section type as stat then press OK.
e.	Execute Analysis – Choose. A window opens.
f.	Select the type and set the specifications and press OK
g.	Execute Output s—to be plotted – Select on Schematic
h.	Then Select the INPUT WIRE(Vin ) and OUTPUT WIRE(Vout) from your test Schematic using mouse
i.	Execute Simulation -- Net list and Run
~~~
# INVERTER SCHEMATIC:

![image](https://github.com/teja2134/VLSI-LAB-EXP-6/assets/161149578/7fcfd07b-3fe6-42b7-819f-d8292014f988)

![image](https://github.com/teja2134/VLSI-LAB-EXP-6/assets/161149578/057132c7-47aa-4bc2-9326-4a7f5a48959d)

# Specifications:  
## Vpulse 	
        V1 = 0	       
        V2 = 1
        td = 0,tr=tf=1 n, ton= 100n ,T=200n

## Vdc	= 1
# Simulation Settings

## Setup for transient analysis:
1.	Stop time =400n

## Setup for D.C analysis
1.	Component to be selected in schematic is	for d.c analysis
2.	Start = -1 Stop = 1 resp.

# Expected Waveform: 

## Transient Analysis:

![inverter](https://github.com/teja2134/VLSI-LAB-EXP-6/assets/161149578/69343dae-2d49-410c-97ca-d07d9b90a425)

## DC Analysis:

<img width="1280" alt="dc " src="https://github.com/teja2134/VLSI-LAB-EXP-6/assets/161149578/6f7a36e2-34a2-46cf-80a6-26b69fcdbd23">

# NAND SCHEMATIC :

<img width="509" alt="nand sch" src="https://github.com/teja2134/VLSI-LAB-EXP-6/assets/161149578/8ff2ba05-e9da-4ff2-823d-cf63c9e25437">

<img width="542" alt="nand diagram" src="https://github.com/teja2134/VLSI-LAB-EXP-6/assets/161149578/f1c140b4-bc4f-406e-9a55-9a2d634ce783">

# Specifications:  

## Vpulse 
Va1 = 0	
Va2 = 1
tr=tf=50ps, period=20ns
pulse width = 10ns

Vb1 = 0	
Vb2 = 1
tr=tf=50ps, period=40ns
pulse width = 20ns

## Vdc	= 1

# Expected Waveform: 

## Transient Analysis:

![nand2](https://github.com/teja2134/VLSI-LAB-EXP-6/assets/161149578/09fe35b1-0049-45b6-8a33-e74254d0430b)

# NOR SCHEMATIC:

<img width="529" alt="nor sch" src="https://github.com/teja2134/VLSI-LAB-EXP-6/assets/161149578/d76f5962-6ade-4852-add2-87eaf541060f">

<img width="494" alt="nor diagram" src="https://github.com/teja2134/VLSI-LAB-EXP-6/assets/161149578/63dd4469-aebc-48fa-b5b0-cf7d05414810">

# Specifications:  

## Vpulse 
Va1 = 0	
Va2 = 1
tr=tf=50ps, period=20ns
pulse width = 10ns

Vb1 = 0	
Vb2 = 1
tr=tf=50ps, period=40ns
pulse width = 20ns

## Vdc	= 1

# Expected Waveform: 

## Transient Analysis:

<img width="743" alt="nor (2)" src="https://github.com/teja2134/VLSI-LAB-EXP-6/assets/161149578/81f08171-c332-4268-9e7d-f817f9ec1315">

# RESULT:

   Thus, the design,simulation and verification of the  CMOS inverter,NAND,NOR from schematic  using cadence was successfully completed. 





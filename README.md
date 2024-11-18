## Ex No: 06 Design-Implementation-of-2-Bit-Multiplier-using-Cadence-Tools 

### Aim:
To design and implement a 2-bit multiplier circuit using Cadence EDA tools, simulate its functionality, and to understand its application in digital arithmetic operations.

### Tools Required:
- Personal Computer
- Cadence Virtuoso Software
  
### Circuit Diagram:

![WhatsApp Image 2024-11-13 at 16 25 39_c1439924](https://github.com/user-attachments/assets/d9cd3034-570c-4b86-8847-b608ccb1c2b5)

### SCHEMATIC SIMULATION:
PROCEDURE FOR CREATING THE SCHEMATIC SIMULATION
Commands to get into Cadence:

1. Right-click and open the terminal window.
2. Type the following commands and press enter:
   
   • csh&emsp;• source /cadence/install/cshrc&emsp;• virtuoso


#### Procedure for Schematic simulation using Cadence
1.	Now two windows must open
    i) virtuoso/command interpreter window
  	ii)”Whats New…”
2.	Close the 2nd window
3.	Use 1st window i.e virtuoso window (CIW) for further processing.
   -	Create a New Library
   - Create Schematic Cell view.
   - Create the Symbol for schematic Cell view.
   - Create the test Cell view.
   - Analog simulation by spectre

### Steps for Schematic Simulation using Cadence:
#### i)	Procedure for Creating New Library.
-	File –New – Library
-	Name: Give name for ur library Ex: VLSILAB_EXP_1
-	Enable Attach to an existing technology library, Click OK
-	Attach the library to the technology library gpdk045.Click OK

### ii)	Create Schematic Cell view.
-	Go to 1st window i.e virtuoso (CIW)
-	File-New-Cell view
-	Setup the new file form
    + Library: Select the one you created.
    + Cell: Give the experiment name Ex: Inverter ViewSchematic
    + Type: Schematic press OK
-	Add the required components from the libraries and make the connections.
    + Go to instance fixed menu or use shortcut key “I” from keypad to go instances
    + Click on browse. This opens the library browser
    +	Now select the appropriate library for components like 
    +	Gpdk45 ------------------------nmos1v, pmos1v
    +	Create Input and Output pins
    +	Make the connections by using fixed narrow wire key
    +	Click Check and Save button

![exp6_schematic](https://github.com/user-attachments/assets/d182d566-f735-4600-8a24-70d1f1ca23b5)

 
### iii)	Creating the Symbol for schematic Cell view

-	In the schematic window, execute 
    +	Create – Cell view – From Cell view
    +	The cell view from cell view window appears
    +	Check Lib Name, Cell Name, From View name must be schematic Press ok
-	Now Symbol generation form appears. Click Ok If No changes required
-	A new window with with default symbol is created.
- Edit the symbol if you want to give actual symbol shape else continue.
- Execute Create-Cell view-from cell view
- Library Name and Cell Name must be same which you have used for schematic. Press OK
- Check for the position of pin side.Prss OK
- Edit for the shape by Create-Shape-Choose required options to edit.

![exp6_symbol](https://github.com/user-attachments/assets/80ac81ba-ef14-48cc-8a34-0e116ae1b78e)

### iv)	Creating the new test cell view

-	Go to CIW window, Execute File-New-Cell view
    +	Setup the new file form
    +	Library: Select the one you created.
    +	Cell: Cell name must be different from the name used in schematic cell view. Ex: Inverter_test
    +	View: Schematic
    +	Type: Schematic press OK
-	Follow the step 3(ii) d to make the required connections

![exp6_sim](https://github.com/user-attachments/assets/73be9b91-b6e0-44cf-b698-b67ba34cf1dc)

 
### Analog simulation by SPECTRE.
-	In test cell view window
-	Launch – ADE L(Analog Design Environment)
    +	Execute Setup—Simulation/directory/Host A new window opens
    +	Set the simulation window to spectre and click ok
    +	Execute Analysis – Choose. A window opens.
    +	Select the type and set the specifications and press OK
    +	Execute Output s—to be plotted – Select on Schematic
    +	Then Select the INPUT WIRE(Vin ) and OUTPUT WIRE(Vout) from your test Schematic using mouse
-	Execute Simulation -- Net list and Run

![exp6_trans1](https://github.com/user-attachments/assets/f5edd5d1-fdb9-49bc-823d-31822655fa28)


##  For Transient Analysis:
  - In the simulation setup, choose transient analysis.
  - Specify the time range for the analysis (start and stop time).
  - Run the simulation and observe the output waveforms


![exp6_trans](https://github.com/user-attachments/assets/1ad15662-a8b7-4031-802f-d600d5082a85)

![exp6_out](https://github.com/user-attachments/assets/08a97ce1-2a2b-4332-8db5-544a83831897)

## Results:
The design and implementation of the 2-bit multiplier using Cadence EDA tools were successfully carried out. The simulation results confirmed the correct operation of the multiplier for all input combinations. 

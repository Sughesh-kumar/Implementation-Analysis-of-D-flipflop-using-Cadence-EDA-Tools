# Implementation-Analysis-of-D-flipflop-using-Cadence-EDA-Tools
Ex No: 03     Implementation & Analysis of D-flipflop using Cadence EDA Tools   

### Aim:
To design and implement a D flip-flop circuit using Cadence EDA tools, analyze its functionality and performance, and understand the principles of digital logic design, including schematic creation, layout design, and simulation.

### Tools Required:

- Personal Computer
- Cadence Virtuoso Software

### Circuit Diagram:
![WhatsApp Image 2024-11-13 at 16 26 07_7924f9ac](https://github.com/user-attachments/assets/d693de5b-08c0-4b6b-a788-10a463e87720)



### SCHEMATIC SIMULATION:
PROCEDURE FOR CREATING THE SCHEMATIC SIMULATION
Commands to get into Cadence

1.	Right Click and open the terminal window
2.	Type the following commands as follows and press enter.
	- csh
	- source /cadence/install/cshrc
	- virtuoso

Procedure for Schematic simulation using Cadence

1.	Now two windows must open i)virtuoso/command interpreter window ii)”Whats New…”

2.	Close the 2nd window
3.	Use 1st window i.e virtuoso window(CIW) for further processing.
	
  - Create a New Library
  - Create Schematic Cell view.
  - Create the Symbol for schematic Cell view.
  - Create the test Cell view.
  - Analog simulation by spectre



i)	Procedure for Creating New Library.

- File –New – Library
- Name : Give name for ur library Ex: VLSILAB_EXP_2
- Enable Attach to an existing technology library, Click OK
- Attach the library to the technology library gpdk045.Click OK

ii)	Create Schematic Cell view.

- Go to 1st window i.e virtuoso(CIW)
- File-New-Cell view
- Setup the new file form
	 + Library: Select the one you a created.
	 + Cell : Give the experiment name Ex: Inverter View_Schematic
	 + Type: Schematic press OK
    
- Add the required components from the libraries and make the connections.
	 + Go to instance fixed menu or use shortcut key “I” from keypad to go instances
	+ Click on browse. This opens the library browser
	+ Now select the appropriate library for components like 
	+ Gpdk45 ------------------------nmos1v,  pmos1v
	+ Create Input and Output pins
	+ Make the connections by using fixed narrow wire key
	+ Click Check and Save button
![Screenshot 2024-10-22 182428](https://github.com/user-attachments/assets/1f0c0e24-06fb-436a-82b8-1ba3065cb9a3)





iii)	Creating the Symbol for schematic Cell view

- In the schematic window, execute 
	+	Create – Cell view – From Cell view
	+	The cell view from cell view window appears
	+	Check Lib Name, Cell Name, From View name must be schematic Press ok
- Now Symbol generation form appears. Click Ok If No changes required
- A new window with with default symbol is created.
- Edit the symbol if you want to give actual symbol shape else continue.
- Execute Create-Cell view-from cell view
- Library Name and Cell Name must be same which you have used for schematic. Press OK
- Check for the position of pin side.Prss OK
- Edit for the shape by Create-Shape-Choose required options to edit.

![Screenshot 2024-10-22 183009](https://github.com/user-attachments/assets/48861d1e-5bb0-44c1-8bb8-d0130e78c9bf)


 
iv)	Creating the new test cell view

- Go to CIW window, Execute File-New-Cell view
	+ Setup the new file form
	+ Library: Select the one you created.
	+ Cell: Cell name must be different from the name used in schematic cell view. Ex: Inverter_test
	+ View: Schematic
	+ Type: Schematic press OK
- Follow the step 3(ii) d to make the required connections
![Screenshot 2024-10-22 182459](https://github.com/user-attachments/assets/4d556d51-d23d-4b23-a3c9-b9e31f792402)







### Analog simulation by SPECTRE.

- In test cell view window
- Launch – ADE L(Analog Design Environment)
	+ Execute Setup—Simulation/directory/Host A new window opens
	+ Set the simulation window to spectre and click ok
	+ Execute Analysis – Choose. A window opens.
	+ Select the type and set the specifications and press OK
	+ Execute Output s—to be plotted – Select on Schematic
	+ Then Select the INPUT WIRE(Vin ) and OUTPUT WIRE(Vout) from your test Schematic using mouse
- Execute Simulation -- Net list and Run
![Screenshot 2024-10-22 182548](https://github.com/user-attachments/assets/a4f3d1f7-b9e3-4a41-b2c4-d31e35631a4b)




### For Transient Analysis :
 In the simulation setup, choose transient analysis.
 Specify the time range for the analysis (start and stop time).
 Run the simulation and observe the output waveforms for the D and Q signals

 ![Screenshot 2024-10-22 182521](https://github.com/user-attachments/assets/9e5f2144-3ea2-4d44-914a-479af1af7be5)


![Screenshot 2024-10-22 182637](https://github.com/user-attachments/assets/e219c6df-2818-4b73-bd1e-f2970463b202)



### Results:
The design and implementation of the D-flip-flop using Cadence EDA tools were successfully completed. The simulated results confirmed the correct operation of the flip-flop, with proper synchronization of the input data with the clock signal. Key performance parameters such as propagation delay, power consumption, and area utilization were evaluated, aligning with expected theoretical values.












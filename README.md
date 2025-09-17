## Exp-No: 02 - Write and simulate seven segment display using Verilog HDL and verify with testbench

# Aim:
To design and simulate a Seven Segment using Verilog HDL and verify its functionality through a testbench using the Vivado 2023.1 simulation environment.

# Apparatus Required:
Vivado 2023.1

# Procedure:
Launch Vivado Open Vivado 2023.1 by double-clicking the Vivado icon or searching for it in the Start menu.

Create a New Project Click on "Create Project" from the Vivado Quick Start window.

In the New Project Wizard: Project Name: Enter a name for the project (e.g., Mux4_to_1).

Project Location: Select the folder where the project will be saved. 

Click Next.

Project Type: Select RTL Project, then click Next.

Add Sources: Click on "Add Files" to add the Verilog files (e.g., mux4_to_1_gate.v, mux4_to_1_dataflow.v, etc.). 

Make sure to check the box "Copy sources into project" to avoid any external file dependencies. 

Click Next.

Add Constraints: Skip this step by clicking Next (since no constraints are needed for simulation). 

Default Part Selection: You can choose a part based on the FPGA board you are using (if any).

If no board is used, you can choose any part, for example, xc7a35ticsg324-1L (Artix-7).

Click Next, then Finish.
Add Verilog Source Files In the "Sources" window, right-click on "Design Sources" and select Add Sources if you didn't add all files earlier. 

Add the Verilog files (mux4_to_1_gate.v, mux4_to_1_dataflow.v, etc.) and the testbench (mux4_to_1_tb.v).

Check Syntax Expand the "Flow Navigator" on the left side of the Vivado interface. 

Under "Synthesis", click "Run Synthesis". 

Vivado will check your design for syntax errors. 

If any errors or warnings appear, correct them in the respective Verilog files and re-run the synthesis.

Simulate the Design In the Flow Navigator, under "Simulation", click on "Run Simulation" → "Run Behavioral Simulation". Vivado will open the Simulations Window, and the waveform window will show the signals defined in the testbench.

View and Analyze Simulation Results.

Adjust Simulation Time To run a longer simulation or adjust timing, go to the Simulation Settings by clicking "Simulation" → "Simulation Settings". 

Under "Simulation", modify the Run Time (e.g., set to 1000ns).

Generate Simulation Report Once the simulation is complete, you can generate a simulation report by right-clicking on the simulation results window and selecting "Export Simulation Results". 

Save the report for reference in your lab records.

Save and Document Results Save your project by clicking File → Save Project.

Take screenshots of the waveform window and include them in your lab report to document your results. 

You can include the timing diagram from the simulation window showing the correct functionality of the Seven Segment across different select inputs and data inputs.

Close the Simulation Once done, by going to Simulation → "Close Simulation

# Input/Output Signal Diagram:
<img width="603" height="736" alt="image" src="https://github.com/user-attachments/assets/cac7cd37-6d01-4ef0-8134-2733ecb5908c" />
<img width="811" height="306" alt="image" src="https://github.com/user-attachments/assets/259e994e-aecf-4dcb-8d3e-d7015d158f50" />
<img width="800" height="602" alt="image" src="https://github.com/user-attachments/assets/04529e6b-6017-4a92-a613-893f241f0f7c" />



# RTL Code:

<img width="1920" height="1080" alt="bcd_7_seg_verilog_code" src="https://github.com/user-attachments/assets/73be6d05-a9cf-4fb3-a1ad-aa2676ecee53" />

# TestBench:

<img width="1920" height="1080" alt="bcd_7_seg_verilog_tb_code" src="https://github.com/user-attachments/assets/c5eaf690-a494-44b4-8204-cf1a66a79819" />

# Output waveform:

<img width="1920" height="1080" alt="bcd_7_seg_verilog_output" src="https://github.com/user-attachments/assets/7ba5269e-56dc-4435-9fbe-144b76e31a2b" />
<img width="1920" height="1080" alt="bcd_7_seg_verilog_tb_output" src="https://github.com/user-attachments/assets/a6ad295a-814d-4e73-8d64-f4decffdc527" />



# Conclusion:
In this experiment, a seven-segment display decoder was designed and simulated using Vivado 2024.1. The Verilog code was implemented to convert binary-coded decimal(BCD) inputs into appropriate segment control signals. The behavioral simulationverified that each digit (0–9) was correctly displayed by activating the corresponding segments (a–g).
Thus, the experiment successfully demonstrated the design and working of a seven segment display using Verilog HDL and provided practical experience with synthesis
and simulation in Vivado.

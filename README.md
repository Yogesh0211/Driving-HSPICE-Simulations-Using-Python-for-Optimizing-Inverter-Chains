# **Project: Driving an HSPICE Tool from Python**

### **Description**  
This project demonstrates how to drive circuit simulation tools (HSPICE) using Python for optimizing delay in an inverter chain. The primary goal is to minimize the delay between the rising edge of the first inverter and the falling edge of a capacitive load, with the following constraints:  
- Each inverter in the chain is an integer multiple (referred to as "fan") larger than its preceding inverter.  
- The capacitive load is fixed at **30 pF**.  
- You will determine the optimal **fan** (scaling factor) and the number of inverters (**N**) to achieve the minimum delay.

---

### **Key Steps**  
1. **Simulation Setup**:  
   - Start with the provided **InvChain.sp** module.
   - Update it for a capacitive load of **30 pF**.
   - Modify the `.tran` statement as needed for longer delay simulations.

2. **Python Automation**:  
   - Use Python to drive HSPICE simulations by iterating through combinations of fan and N.  
   - For each combination, simulate the inverter chain and extract the delay.  

3. **Optimization**:  
   - Evaluate delays for all combinations of **fan** and **N**.  
   - Identify the optimal values of fan and N that minimize the delay.  
   - Print the delay for each combination, followed by the optimal configuration and its corresponding time delay.

---

### **Deliverables**  
1. **Python Script (`project4.py`)**:  
   - Drives the HSPICE simulations.  
   - Prints delays for all combinations of fan and N.  
   - Outputs the optimal fan, N, and the corresponding minimum delay.  

2. **Additional Files**:  
   - Any files required for the Python script to run (e.g., modified SPICE files).  
   - Do **not** include the CMOS library file.  

3. **Output**:  
   - Console logs showing delay calculations and the optimal results.  

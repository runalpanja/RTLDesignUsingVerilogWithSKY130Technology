# RTL design using Verilog with SKY130 Technology 
![Verilog-flyer](https://user-images.githubusercontent.com/100710081/165515835-c9e707e7-cc42-4439-8f95-81b94bb8a397.png)

## Brief Description of the Workshop

*Workshop intends to teach the verilog coding guidelines that results in predictable logic in Silicon. It is important to note that every verilog code is not synthesizable and even if it is , it may result in different logic depending on the coding styles used. The course details all these aspects of the Verilog HDL with theory and backed with lot of practical examples. Workshop introduces to the digital logic design using Verilog HDL . Validating the functionality of the design using Functional Simulation. Writing Test Benches to validate the functionality of the RTL design . Logic synthesis of the Functional RTL Code. Gate Level Simulation of the Synthesized Netlist.*
# *Index*
- [RTL design using Verilog with SKY130 Technology](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#rtl-design-using-verilog-with-sky130-technology)
  - [Day 1: Introduction to Verilog RTL Design and Synthesis](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#day-1-introduction-to-verilog-rtl-design-and-synthesis)
    - [Part 1: Introduction to Open-Source simulator iverilog](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#part-1-introduction-to-open-source-simulator-iverilog)
    - [Part 2: Labs using iverilog and gtkwave](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#part-2-labs-using-iverilog-and-gtkwave)
    - [Part 3: Introduction to Yosys and Logic Synthesis](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#part-3-introduction-to-yosys-and-logic-synthesis)
    - [Part 4: Lab using Yosys and SKY130 PDKs](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#part-4-lab-using-yosys-and-sky130-pdks)











# Day 1: Introduction to Verilog RTL Design and Synthesis
On the first day of the workshop, we learnt about the flow of RTL design to GDSII. We learnt how to use the simulator iVerilog and also learnt about the synthesizer tool Yosys. Synthesizer tool converts an RTL design to netlist.
## Part 1: Introduction to Open-Source simulator iverilog
### Sub-Part 1: Introduction to iVerilog Simulator
-  What is a Simulator?
    -   Simulator is a tool used for simulating the design
    -   RTL design is checked for adherence to the spec by simulating the design
- What is a Design?
    -   Design is the actual Verilog code or set of codes which has the intended functionalityn to meet with the required specifications
- What is a Testbench? 
    -   TestBench is the set up to apply stimulus(test_vectors) to the design to check its functionality
    -   ![Screenshot 2022-04-28 at 10 27 40 AM](https://user-images.githubusercontent.com/100710081/165680015-a6474780-d33d-42f9-be1e-eae923873e52.png)

- How simulator works?
    - Simulator looks for changes in the input signals
    - Upon change to the input, the output is evaluated.If no change in the input, there will be no change in the output    
    - Simulator is looking for change in the values of the input
    - ![Screenshot 2022-04-28 at 10 28 06 AM](https://user-images.githubusercontent.com/100710081/165680028-5f937eb0-57be-4b35-91c4-039f2ab441fc.png)



    
## Part 2: Labs using iverilog and gtkwave

## Part 3: Introduction to Yosys and Logic Synthesis

## Part 4: Lab using Yosys and SKY130 PDKs




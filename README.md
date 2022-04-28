# RTL design using Verilog with SKY130 Technology 
![Verilog-flyer](https://user-images.githubusercontent.com/100710081/165515835-c9e707e7-cc42-4439-8f95-81b94bb8a397.png)

## Brief Description of the Workshop

*Workshop intends to teach the verilog coding guidelines that results in predictable logic in Silicon. It is important to note that every verilog code is not synthesizable and even if it is , it may result in different logic depending on the coding styles used. The course details all these aspects of the Verilog HDL with theory and backed with lot of practical examples. Workshop introduces to the digital logic design using Verilog HDL . Validating the functionality of the design using Functional Simulation. Writing Test Benches to validate the functionality of the RTL design . Logic synthesis of the Functional RTL Code. Gate Level Simulation of the Synthesized Netlist.*
# *Index*
- [RTL design using Verilog with SKY130 Technology](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#rtl-design-using-verilog-with-sky130-technology)
  - [Day 1: Introduction to Verilog RTL Design and Synthesis](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#day-1-introduction-to-verilog-rtl-design-and-synthesis)
    - [Part 1: Introduction to Open-Source simulator iverilog](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#part-1-introduction-to-open-source-simulator-iverilog)
      - [Sub-Part 1: Introduction to iVerilog Simulator](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#sub-part-1-introduction-to-iverilog-simulator)  
    - [Part 2: Labs using iverilog and gtkwave](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#part-2-labs-using-iverilog-and-gtkwave)
      - [Sub-Part 1: Introduction to the lab](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#sub-part-1-introduction-to-the-lab) 
      - [Sub-Part 2: Introduction iverilog gtkwave part 1](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#sub-part-2-introduction-iverilog-gtkwave-part-1)
      - [Sub-Part 3: Introduction iverilog gtkwave part 2](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#sub-part-3-introduction-iverilog-gtkwave-part-2)
    - [Part 3: Introduction to Yosys and Logic Synthesis](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#part-3-introduction-to-yosys-and-logic-synthesis)
    
      - [Sub-Part 1: Introduction to Yosys](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#sub-part-1-introduction-to-yosys)
      - [Sub-Part 2: Introduction to Logic Synthesis Part 1](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#sub-part-2-introduction-to-logic-synthesis-part-1)
      - [Sub-Part 3: Introduction to Logic Synthesis Part 2](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#sub-part-3-introduction-to-logic-synthesis-part-2)
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

### Sub-Part 1: Introduction to the lab
In this lab, envrionment set up has been done.A new directory 'VLSI' has been created. 'vsdflow' and 'sky130RTLDesignAndSynthesisWorkshop' have been cloned to the directory from github using the ' git clone' command.
![Screenshot 2022-04-28 at 11 14 19 AM](https://user-images.githubusercontent.com/100710081/165684973-8a243571-bbd9-43f3-8396-1460cbaaa9f7.png)

Let us walk through the directory.
my_lib contains all our library files. It contains two folder 'lib' and 'verilog_model'. 'lib' contains SKY130 standard cell library which we will be using for synthesis and 'verilog_model' contains all the standard cell verilog models

![Screenshot 2022-04-28 at 11 23 43 AM](https://user-images.githubusercontent.com/100710081/165686193-ab6babbb-4919-437b-8489-a6cf0ece81ea.png)

### List of Verilog Models



### List of Verilog Files 
It contains both design and corresponding testbench files.

![Screenshot 2022-04-28 at 3 38 26 PM](https://user-images.githubusercontent.com/100710081/165730279-08176a04-2650-45ea-8a2e-fcbfc83f2d1a.png)


### Sub-Part 2: Introduction iverilog gtkwave part 1

Generarting waveform by creating .vcd files.

![image](https://user-images.githubusercontent.com/100710081/165738527-5063cb6e-831b-4816-ad00-382949878f83.png)
![image](https://user-images.githubusercontent.com/100710081/165738834-aa3bb9bb-d583-4e98-a4f6-3ccd0506187e.png)
![image](https://user-images.githubusercontent.com/100710081/165739005-0ad07504-541e-428a-9994-b8586e0ee225.png)
![image](https://user-images.githubusercontent.com/100710081/165740590-4347f545-139c-41ca-949a-25bc97cddedb.png)
Using gtkwave , we can show for the " good_mux.v " design how the output toggles between i0 and i1 respectively as select line 'sel' toggles between 0 & 1.
So, this is how we will load the design and check its functionality.

### Sub-Part 3: Introduction iverilog gtkwave part 2

![image](https://user-images.githubusercontent.com/100710081/165743595-bf5fd003-cb78-4867-bd41-d72f43d23c2b.png)
![image](https://user-images.githubusercontent.com/100710081/165744353-eb4bd0ba-adc1-4962-b820-23a049d26786.png)

In the above testbench, we can see instantiation of good_mux.v e.g Instantiate the Unit Under Test (UUT).It is also called Design Under Test (DUT).

It may kindly be noted that the testbench neither have primary inputs nor primary outputs.

Now we will start dumping the VCD file.

Running the simulator for 300ns and finish with the command $finish.
In order to run it for ,say 500ns , we will write ' #500 $finish; ' Just like that!

In every 75 ns, sel = - sel which means 'sel' line toggles in every 75ns.


The below piece of code is said to be the STIMULUS GENERATOR.

![image](https://user-images.githubusercontent.com/100710081/165748608-8320065b-a9fd-4400-947c-7126576f09d3.png)

In this TestBench, we are not having any STIMULUS OBSERVER. We are directly dumping out the VCD file while observing the output in the gtkwave.


## Part 3: Introduction to Yosys and Logic Synthesis

### Sub-Part 1: Introduction to Yosys

-  What is a Synthesizer?
   -  It is the tool used for converting the RTL to netlist.
   -  Yosys is the synthesizer used in this workshop.
  
-  Yosys setup
   -![image](https://user-images.githubusercontent.com/100710081/165752064-3984e59e-096a-4a1b-86a5-62678ad788d4.png)
- NOTE : 
   - The set of primary inputs/primary outputs will remain same between the RTL design and the synthesized output -> same testbench can be used.

  

### Sub-Part 2: Introduction to Logic Synthesis Part 1 

-  What is RTL?

     ![image](https://user-images.githubusercontent.com/100710081/165756584-2ec44a03-ad4e-442c-98c2-813d2b43690c.png)

-  How to map RTL code with Digital Logic Design?

     ![image](https://user-images.githubusercontent.com/100710081/165756069-52d91575-fd28-4446-b473-a853d19f46d2.png)
     
-  What is Synthesis?

     ![image](https://user-images.githubusercontent.com/100710081/165757365-36a7e5e2-8bb4-48e3-98b7-6b6ee952c534.png)


-  What is .lib ?
     
     ![image](https://user-images.githubusercontent.com/100710081/165757991-56648c41-2c0f-4c11-9fbe-4176dccac2c0.png)
     
-  Why different flavours of gate?

     ![image](https://user-images.githubusercontent.com/100710081/165759243-a0cd46c7-0618-40d5-9cbc-56685bc7e844.png)
     
    -  Tcq_a = propagation delay of flop A
    -  In order to make fclk -> 'max' , Tclk -> 'min'
    -  Tclk -> 'min' when Tcombi -> 'min'
    
     


### Sub-Part 3: Introduction to Logic Synthesis Part 2 

-  Why do we need slow cells?

     ![image](https://user-images.githubusercontent.com/100710081/165760465-94dbf4ff-13c6-442f-bfa9-74374483900f.png)
     
-  Faster cells vs. Slower cells

     ![image](https://user-images.githubusercontent.com/100710081/165766112-e059648f-2b02-49a6-ab55-50df0284eadc.png)

-  Selection of cells

     ![image](https://user-images.githubusercontent.com/100710081/165766973-02a7e899-a8aa-43e8-bbd4-f768955bac31.png)
     
-  Synthesis (Illustration)
     
     
     ![image](https://user-images.githubusercontent.com/100710081/165767679-b281404f-ccb3-4a73-b4a2-24a160a549e2.png)























## Part 4: Lab using Yosys and SKY130 PDKs




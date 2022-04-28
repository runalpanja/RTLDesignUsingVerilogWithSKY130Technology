# RTL design using Verilog with SKY130 Technology 

<p>
<img src="https://user-images.githubusercontent.com/100710081/165515835-c9e707e7-cc42-4439-8f95-81b94bb8a397.png" />
</p>
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
<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/165680015-a6474780-d33d-42f9-be1e-eae923873e52.png" />
</p>

- How simulator works?
    - Simulator looks for changes in the input signals
    - Upon change to the input, the output is evaluated.If no change in the input, there will be no change in the output    
    - Simulator is looking for change in the values of the input
    
<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/165680028-5f937eb0-57be-4b35-91c4-039f2ab441fc.png" />
</p>
    



    
## Part 2: Labs using iverilog and gtkwave

### Sub-Part 1: Introduction to the lab
In this lab, envrionment set up has been done.A new directory 'VLSI' has been created. 'vsdflow' and 'sky130RTLDesignAndSynthesisWorkshop' have been cloned to the directory from github using the ' git clone' command.

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/165684973-8a243571-bbd9-43f3-8396-1460cbaaa9f7.png" />
</p>

Let us walk through the directory.
my_lib contains all our library files. It contains two folder 'lib' and 'verilog_model'. 'lib' contains SKY130 standard cell library which we will be using for synthesis and 'verilog_model' contains all the standard cell verilog models.

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/165686193-ab6babbb-4919-437b-8489-a6cf0ece81ea.png" />
</p>  

### List of Verilog Models



### List of Verilog Files 
It contains both design and corresponding testbench files.

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/165730279-08176a04-2650-45ea-8a2e-fcbfc83f2d1a.png" />
</p>


### Sub-Part 2: Introduction iverilog gtkwave part 1

Generarting waveform by creating .vcd files.

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/165738527-5063cb6e-831b-4816-ad00-382949878f83.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/165738834-aa3bb9bb-d583-4e98-a4f6-3ccd0506187e.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/165739005-0ad07504-541e-428a-9994-b8586e0ee225.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/165740590-4347f545-139c-41ca-949a-25bc97cddedb.png" />
</p>

Using gtkwave , we can show for the " good_mux.v " design how the output toggles between i0 and i1 respectively as select line 'sel' toggles between 0 & 1.
So, this is how we will load the design and check its functionality.

### Sub-Part 3: Introduction iverilog gtkwave part 2

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/165743595-bf5fd003-cb78-4867-bd41-d72f43d23c2b.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/165744353-eb4bd0ba-adc1-4962-b820-23a049d26786.png" />
</p>  

In the above testbench, we can see instantiation of good_mux.v e.g Instantiate the Unit Under Test (UUT).It is also called Design Under Test (DUT).

It may kindly be noted that the testbench neither have primary inputs nor primary outputs.

Now we will start dumping the VCD file.

Running the simulator for 300ns and finish with the command $finish.
In order to run it for ,say 500ns , we will write ' #500 $finish; ' Just like that!

In every 75 ns, sel = - sel which means 'sel' line toggles in every 75ns.


The below piece of code is said to be the STIMULUS GENERATOR.

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/165748608-8320065b-a9fd-4400-947c-7126576f09d3.png" />
</p>

In this TestBench, we are not having any STIMULUS OBSERVER. We are directly dumping out the VCD file while observing the output in the gtkwave.


## Part 3: Introduction to Yosys and Logic Synthesis

### Sub-Part 1: Introduction to Yosys

-  What is a Synthesizer?
   -  It is the tool used for converting the RTL to netlist.
   -  Yosys is the synthesizer used in this workshop.
  
-  Yosys setup
<p align="center">
 <img src="https://user-images.githubusercontent.com/100710081/165752064-3984e59e-096a-4a1b-86a5-62678ad788d4.png" />
</p>

- NOTE : 
   - The set of primary inputs/primary outputs will remain same between the RTL design and the synthesized output -> same testbench can be used.

  

### Sub-Part 2: Introduction to Logic Synthesis Part 1 

-  What is RTL?
<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/165756584-2ec44a03-ad4e-442c-98c2-813d2b43690c.png" />
</p>

-  How to map RTL code with Digital Logic Design?
<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/165756069-52d91575-fd28-4446-b473-a853d19f46d2.png" />
</p>
     
-  What is Synthesis? 
<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/165757365-36a7e5e2-8bb4-48e3-98b7-6b6ee952c534.png" />
</p>


-  What is .lib ?
-  
<p align="center"> 
<img src="https://user-images.githubusercontent.com/100710081/165757991-56648c41-2c0f-4c11-9fbe-4176dccac2c0.png" />
</p>
     
-  Why different flavours of gate? 

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/165759243-a0cd46c7-0618-40d5-9cbc-56685bc7e844.png" />
</p>
     
    -  Tcq_a = propagation delay of flop A
    -  In order to make fclk -> 'max' , Tclk -> 'min'
    -  Tclk -> 'min' when Tcombi -> 'min'
    
     


### Sub-Part 3: Introduction to Logic Synthesis Part 2 

-  Why do we need slow cells?

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/165760465-94dbf4ff-13c6-442f-bfa9-74374483900f.png" />
</p>
     
-  Faster cells vs. Slower cells
  
<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/165766112-e059648f-2b02-49a6-ab55-50df0284eadc.png" />
</p>

-  Selection of cells

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/165766973-02a7e899-a8aa-43e8-bbd4-f768955bac31.png" />
</p>
     
-  Synthesis (Illustration)

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/165767679-b281404f-ccb3-4a73-b4a2-24a160a549e2.png" />
</p>
     





## Part 4: Lab using Yosys and SKY130 PDKs
### Sub-Part 1: Yosys 1 good mux Part1
In this lab, we will have an introduction to synthesizer Yosys. We will learn how to invoke Yosys and how to synthesize our design.



Invoke Yosys.

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/165773780-5fa5038e-932a-4fca-b3c7-3adcffc49c06.png" />
</p>

When we installed 'vsdflow' , Yosys automatically got installed. We are in the Yosys prompt now!!!!

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/165797118-9681daf4-7e50-42c2-a5ab-81007b627fda.png" />
</p>
<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/165798646-c62a7e19-a682-4a31-a15e-6c840a80783f.png" />
</p>

To synthesize a particular module, we use the 'synth - top' command as follows....

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/165799518-0b81027c-1b57-4d6e-8b71-705ca37aaa27.png" />
</p>
<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/165800418-0a5f8c3c-6096-4b36-b222-25b0992a8456.png" />
</p>
<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/165801455-8845e4e6-d161-488f-b9db-7ce5197f9f8a.png" />
</p>
<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/165801722-6e5319ce-b31a-450c-9506-141a1e33365a.png" />
</p>
<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/165801999-7782c05c-193c-44b2-b4ca-4b74842572d3.png" />
</p>
<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/165802131-3b63a8bf-7442-4ab7-a42d-83b30347628f.png" />
</p>
<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/165802462-26a08b73-3ee3-47ee-89e6-4d47d036e2fd.png" />
</p>
<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/165802845-efd41b76-f4c3-419e-8569-76f87777894d.png" />
</p>
<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/165803125-ed9b6bc6-10ad-433a-bde1-260ede63eb42.png" />
</p>
<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/165803402-cdaa1ab1-6172-4abe-a6b0-dde129499e98.png" />
</p>
<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/165803598-af98df44-ad24-4968-be61-8bd57bbc2ac8.png" />
</p>
<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/165803807-a0b8fdab-d51a-4653-afaf-b60c852a95c4.png" />
</p>
<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/165804015-b208a502-2f76-4310-b1d2-e8f96e180d48.png" />
</p>
<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/165804307-b24ffd0b-b52e-4958-b094-8d0eeb85f6cb.png" />
</p>
<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/165804489-f4d5a2e6-d9e3-442f-8eb4-4042bb7630e1.png" />
</p>












































### Sub-Part 2: Yosys 1 good mux Part2



### Sub-Part 3: Yosys 1 good mux Part3






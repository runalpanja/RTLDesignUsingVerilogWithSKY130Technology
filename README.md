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
       - [Sub-Part 1: Yosys 1 good mux Part1](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology#sub-part-1-yosys-1-good-mux-part1)
       - [Sub-Part 2: Yosys 1 good mux Part2](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#sub-part-2-yosys-1-good-mux-part2)



  -  [Day 2: Timing libs,hierarchical vs flat synthesis and efficient flat coding styles](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology//blob/main/README.md#day-2-timing-libshierarchical-vs-flat-synthesis-and-efficient-flat-coding-styles)
      - [Part 1: Introduction to Timing .libs](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#part-1-introduction-to-timing-libs)
         - [Sub-Part 1: Introduction to dot Lib part1](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#sub-part-1-introduction-to-dot-lib-part1)
         - [Sub-Part 2: Introduction to dot Lib part2](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#sub-part-2-introduction-to-dot-lib-part2)
         - [Sub-Part 3: Introduction to dot Lib part3](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#sub-part-3-introduction-to-dot-lib-part3)


      - [Part 2: Hierarchical vs. Flat synthesis](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#part-2-hierarchical-vs-flat-synthesis)
         - [Sub-Part 1: Hier synthesis flat synthesis part1](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#sub-part-1-hier-synthesis-flat-synthesis-part1)
         - [Sub-Part 2: Hier synthesis flat synthesis part2](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#sub-part-2-hier-synthesis-flat-synthesis-part2)
         
    
      - [Part 3: Various flop coding styles and optimization](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#part-3-various-flop-coding-styles-and-optimization)
        
         - [Sub-Part 1: Lab flop synthesis simulations part1](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#sub-part-1-lab-flop-synthesis-simulations-part1)
         - [Sub-Part 2: Lab flop synthesis simulations part2](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#sub-part-2-lab-flop-synthesis-simulations-part2)
         - [Sub-Part 3: Interesting optimisations part1](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#sub-part-1-interesting-optimisations-part1)
         - [Sub-Part 4: Interesting optimisations part2](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#sub-part-2-interesting-optimisations-part2)


      
    -  [Day 3: Combinational and Sequential optimizations](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#day-3-combinational-and-sequential-optimizations)
       - [Part 1: Introduction to optimizations](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#part-1-introduction-to-optimizations)
         - [Sub-Part 1: Introduction to optimizations Part 1](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#sub-part-1-introduction-to-optimizations-part-1)
         - [Sub-Part 2: Introduction to optimizations Part 2](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#sub-part-2-introduction-to-optimizations-part-2)
        


       - [Part 2: Combinational Logic Optimisations](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#part-2-combinational-logic-optimisations)
         - [Sub-Part 1: Combinational Logic Optimisations part1](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#sub-part-1-combinational-logic-optimisations-part1)
         - [Sub-Part 2: Combinational Logic Optimisations part2](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#sub-part-2-combinational-logic-optimisations-part2)
         
       - [Part 3: Sequential Logic Optimisations](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#part-3-sequential-logic-optimisations)
         - [Sub-Part 1: Sequential Logic Optimisations part1](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#sub-part-1-sequential-logic-optimisations-part1)




       - [Part 4: Sequential Logic Optimisations for unused outputs](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#part-4-sequential-logic-optimisations-for-unused-outputs)
         - [Sub-Part 1: Sequential Logic Optimisations part1](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#sub-part-1-sequential-logic-optimisations-part1-1)
         - [Sub-Part 2: Sequential Logic Optimisations part2](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#sub-part-2-sequential-logic-optimisations-part2)


     -  [Day 4: GLS, BLOCKING VS NON-BLOCKING and Synthesis Simulation Mismatch](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#day-4-gls-blocking-vs-non-blocking-and-synthesis-simulation-mismatch)
        - [Part 1: GLS Synthesis Simulation mismatch and Blocking -Nonblocking statements](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#part-1-gls-synthesis-simulation-mismatch-and-blocking--nonblocking-statements)
          - [Sub-Part 1: GLS Concepts And Flow Using Iverilog](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#sub-part-1-gls-concepts-and-flow-using-iverilog)
          - [Sub-Part 2: Synthesis Simulation Mismatch](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#sub-part-2-synthesis-simulation-mismatch)
          - [Sub-Part 3: Blocking And Non-Blocking Statements In Verilog](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#sub-part-3-blocking-and-non-blocking-statements-in-verilog)
        - [Part 2: Lab on GLS Synthesis and Simulation mismatch](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#part-2-lab-on-gls-synthesis-and-simulation-mismatch)
          - [Sub-Part 1: Lab GLS Synth Sim Mismatch part1](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#sub-part-1-lab-gls-synth-sim-mismatch-part1)
          - [Sub-Part 2: Lab GLS Synth Sim Mismatch part2](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#sub-part-2-lab-gls-synth-sim-mismatch-part2)


        - [Part 3: Lab on Synth Sim mismatch and blocking statement](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#part-3-lab-on-synth-sim-mismatch-and-blocking-statement)
          - [Sub-Part 1: Lab Synth sim mismatch blocking statement part1](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#sub-part-1-lab-synth-sim-mismatch-blocking-statement-part1)
          - [Sub-Part 2: Lab Synth sim mismatch blocking statement part2](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#sub-part-2-lab-synth-sim-mismatch-blocking-statement-part2)





     -  [Day 5: If,Case,For loop and For generate](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#day-5-ifcasefor-loop-and-for-generate)
        - [Part 1: Lab on 'Incomplete IF Case'](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#part-1-lab-on-incomplete-if-case)
          - [Sub-Part 1: Lab Incomplete IF part1](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#sub-part-1-lab-incomplete-if-part1)
          - [Sub-Part 2: Lab Incomplete IF part2](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#sub-part-2-lab-incomplete-if-part2)
        - [Part 2: Lab incomplete overlapping](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#part-2-lab-incomplete-overlapping)
          
          - [Sub-Part 1: Lab incomplete overlapping Case part1](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#sub-part-1-lab-incomplete-overlapping-case-part1)
          - [Sub-Part 2: Lab incomplete overlapping Case part2](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#sub-part-2-lab-incomplete-overlapping-case-part2)  
          - [Sub-Part 3: Lab incomplete overlapping Case part3](https://github.com/runalpanja/RTLDesignUsingVerilogWithSKY130Technology/blob/main/README.md#sub-part-3-lab-incomplete-overlapping-case-part3)
          -      
          
     









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


-   In order to generate the netlist, we will use 'abc -liberty' command.... this will convert our RTL into gate and which gate it will be linked to that will be specified in our library.... 
-   The logic of *good_mux.v* will be realized in terms of the standard cells available in *" ../my_lib/lib/sky130_fd_sc_hd__tt_025C_1v80.lib "*

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/165811932-adf3a84b-9f34-4731-956d-e63a633c2ba2.png" />
</p>


Comparing the outcome with *good_mux.v* file....

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/165814516-70ead114-0d51-49a1-a067-854fe6eab555.png" />
</p>

Now,  by using 'show' command we get the graphical version of the logic it has realized....

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/165816345-71c6b5e9-9930-4b94-9a52-046c2bc2495e.png" />
</p>

Graphical view....
<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/165816841-926430c8-fe53-4a28-be22-d548014eabcd.png" />
</p>

### Sub-Part 2: Yosys 1 good mux Part2

How to write the netlist?
-  By using *write_verilog* command, we get....

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/165827136-477cb004-691f-48e7-aaae-379223f54b97.png" />
</p>


<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/165826198-929ef1b7-4577-4984-8727-0f12ed8bd20f.png" />
</p>
<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/165826394-2ef39822-dcf6-4b74-ba3b-44415258b91a.png" />
</p>


<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/165828038-afa8ac29-843c-4197-8ee5-cf75fd487493.png" />
</p>



# Day 2: Timing libs,hierarchical vs flat synthesis and efficient flat coding styles
## Part 1: Introduction to Timing .libs 
### Sub-Part 1: Introduction to dot Lib part1

What is .lib?
  - collection of standard cells e.g slow or fast cells

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166093272-3ac71677-96f6-4b9f-be09-684e08fcc585.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166093406-26c6f288-ba89-4a0f-99d6-4be69d8c1800.png" />
</p>

First lines tells it is 130nm technology library.

tt-> typical library

025C -> temperature

1V80 -> voltage

When you look into the library, 3 letters come into picture : *P V T*

P -> PROCESS (variation due to fabrication) 

V -> VOLTAGE

T -> TEMPERATURE 


Our libraries will be characterized to process these variations.





### Sub-Part 2: Introduction to dot Lib part2

It talks about technology, delay_model,time_unit, voltage_unit, leakage_power_unit,current_unit, pulling_resistance_unit,capacitive_load_unit etc ....

It talks about the operating condition.

The keyword 'cell' marks the beginning of cell definition....

There are lot of different types of cells....

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166094406-3a2eb809-186f-454c-9c71-65f1efde01ed.png" />
</p>


### Sub-Part 3: Introduction to dot Lib part3

Wider cells consume MORE power.... and provides LESS delay....

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166094941-0496eb37-f366-4d67-b388-9a0e953a2366.png" />
</p>



## Part 2: Hierarchical vs. Flat synthesis
### Sub-Part 1: Hier synthesis flat synthesis part1

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166096457-a1474f76-a08f-492e-8dcf-e7443cbc6d20.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166096505-eb5e9b20-c9a8-42b1-bb2f-6fd99adf0c4b.png" />
</p>

As we can see above, it has 2 modules.

submodule 1 -> AND GATE which is instantiated as u1

submodule 2 -> OR GATE  which is instantiated as u2

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166096801-4af226da-39fb-4c9b-ac15-8576d8fb5e59.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166097075-363f4ccd-54a2-45ac-b064-6e18b1521050.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166097107-f2874511-93b6-48f4-adbe-b73e2af30e6d.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166097151-4e66c3e8-d80d-4b11-a98b-9c15d22cc3fb.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166097185-fdfa8d0e-db90-4f85-8416-265732b33f9e.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166097312-5fb38cac-2afb-4cdc-b990-1d7f4cf22bbf.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166097351-d1d66bbc-7f46-4ab2-8de3-111fc259ecaa.png" />
</p>
<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166097538-1005fcb1-e360-4573-9210-fa975db7b317.png" />
</p>


<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166097408-b41ac551-eb9b-4f82-9f30-d692f89d8a01.png" />
</p>


Here, we can NOT see AND or OR gate but the instances u1 and u2 only.....

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166097570-e9c8f775-e94a-4921-98d7-9f133f19f90c.png" />
</p>
<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166098227-8256b291-a0c8-4225-9106-efef233992f9.png" />
</p>







<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166098096-c4d53a66-1a9f-4bf8-baa7-861825437ca1.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166098132-20389bad-281b-4880-94ce-5ac199434b33.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166098332-edc819c2-95f3-4441-9bce-9b82e96b5ea9.png" />
</p>
<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166098832-60fbd6a2-224f-4c93-b627-6948cbf6ba25.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166098935-4e71a3f2-2d72-41f8-93c7-b52deff7c488.png" />
</p>



As we can above, the hierarchies are flattened out....




### Sub-Part 2: Hier synthesis flat synthesis part2

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166099444-bf7309bf-3a65-4fd7-9c55-3bbaaf4bf2b6.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166099701-dee5deb8-5acc-46f3-855f-bb6bbeb96ca7.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166099801-b34fbb44-0d05-4e93-a5bc-8a1ab9ba966b.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166099827-6e627fa4-43c3-4b9b-a533-b4b4bc670608.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166099890-fe13e018-f5c5-44f5-8774-1af6f281e0bc.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166099973-625b7951-851d-40ee-9721-cf188d4b38ab.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166100016-d2bee0e1-1b15-405a-b84b-7b0ba8f08462.png" />
</p>

- Why sub-module level synthesis?
    - when we have multiple instances of same module....
    - when the design is MASSIVE, DIVIDE and CONQUER is used.... 


  
## Part 3: Various flop coding styles and optimization
### Sub-Part 1: Lab flop synthesis simulations part1

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166116533-fc7dd665-24bd-45ab-ae5f-1d13f773a831.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166116644-6d866f2b-0958-49c8-b425-0117f0a2417e.png" />
</p>
<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166116868-690f96df-c889-4142-8795-415bb4fdf530.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166116922-17b2527a-56f8-4275-8012-fa0e266e4048.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166117058-95cc166a-4f29-4433-95d0-1a405f4cd173.png" />
</p>

### Sub-Part 2: Lab flop synthesis simulations part2

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166117200-3c7bc7bd-4325-4ce3-851d-b77376843640.png" />
</p>
<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166117392-1e07f722-a5d8-47cd-b405-edae195532d1.png" />
</p>
<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166117478-63970178-e510-4e57-bd39-bfdfbbcd1ca9.png" />
</p>
<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166117523-091720d3-59d2-4e1f-81f8-5f9b90f06c66.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166117551-2dbbd0aa-f582-4550-bf6a-33b76594a9c9.png" />
</p>
<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166117696-8ff6cc98-ef8a-40fa-9c70-f1f2e28dc43b.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166117960-96fefb3f-49cd-41d6-92fe-12bb89f08852.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166118003-a8c1318b-21b3-4c69-a5be-e552edcf616f.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166118030-cf0ce6d8-f6c9-42f9-9655-1533c926acd9.png" />
</p>


<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166118093-fee8e144-9e5f-4907-b64a-1172137ee71f.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166118229-c4272a5c-cfa9-4e42-847d-5256549b08d7.png" />
</p>
<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166118304-0e4542df-b51e-4bbd-9227-f5c97618f0d6.png" />
</p>
<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166118358-4e183371-3764-423c-8f6e-1ce96fa4d0df.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166118398-f473240f-f081-4abc-bfd7-f73cc87390d8.png" />
</p>
<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166118419-70ac4287-d058-48e6-a30e-f9b2f6073955.png" />
</p>


### Sub-Part 3: Interesting optimisations part1

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166118577-be583107-192b-435f-a9f6-7fdc5146a561.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166118612-f5f9e60b-79a2-46e5-bad5-19aa86396967.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166118842-360b3eb7-770b-497e-bce8-8ba1e649b3b8.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166118906-b65daa88-2ef9-4886-9410-654d7ea3a030.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166118951-55aba26a-ed56-4454-a194-7de9446ec66c.png" />
</p>
<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166118976-68de4a8f-d2eb-445e-bf5d-7bac1e6157d3.png" />
</p>

### Sub-Part 4: Interesting optimisations part2

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166119087-1dd081cc-328e-48d7-a5c9-8c16fc208fba.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166119179-11bdd58b-e83c-4105-80db-6e7f8769257f.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166120413-f721a9c1-9a9d-4f4d-89ba-f3786977c2f8.png" />
</p>
<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166120447-f2c5e348-ab12-46f2-a428-a53b728f63c4.png" />
</p>
<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166120499-43e856d9-08b4-4743-bf45-fb1e98a16e74.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166120524-0419b045-463c-4d90-9d6a-cae796c6a4ce.png" />
</p>
<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166120586-ecd9577d-4e13-4871-9201-b87398880b75.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166120617-86abf00f-2fd8-4737-9f1d-4c513d396442.png" />
</p>

















# Day 3: Combinational and Sequential optimizations
## Part 1: Introduction to optimizations
### Sub-Part 1: Introduction to optimizations Part 1


<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166157929-6650fc69-e326-43c2-ac25-18b5e743da31.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166158060-48b5a052-959a-45ae-84ab-a7269017e5f7.png" />
</p>


### Sub-Part 2: Introduction to optimizations Part 2

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166158155-fdd8ef77-5e9a-4d09-8508-3fc63ed6a1b3.png" />
</p>








## Part 2: Combinational Logic Optimisations
### Sub-Part 1: Combinational Logic Optimisations part1


<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166182992-8560ad25-ad58-48c5-bacd-d016bc574641.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166198845-82da96d4-57fe-4254-a5db-6ea45789a82f.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166206547-1df1fc36-e4d7-451c-a2e9-2d97e41d16b2.png" />
</p>


<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166206791-64b8ca6a-0c42-41a8-8ac3-c5b72777486f.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166206982-07529b93-c56e-47d7-99b4-1f01c9846695.png" />
</p>


<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166207511-7c63bb57-9d8b-4924-9681-5c59818b9187.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166207671-22927a26-09c0-4e3f-8c64-688953bca376.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166208203-07a1ade2-3be1-48a1-815c-d3b63276a81f.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166210024-c9ac3173-646b-4ece-8406-557e806231e6.png" />
</p>


<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166210669-c394eee1-5ca1-4e19-8a82-28dcb0fea98c.png" />
</p>



### Sub-Part 2: Combinational Logic Optimisations part2

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166215883-785a6c21-901d-4468-ade8-c9e77c308e93.png" />
</p>


<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166216138-22d149bc-fa57-4eb6-b4d2-26ec3b539834.png" />
</p>


<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166216282-e6d1acb3-8b29-4a4d-8749-60ea183ccc4d.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166216394-92f549cf-526d-4f73-9495-25d85ff1d517.png" />
</p>

## Part 3: Sequential Logic Optimisations
### Sub-Part 1: Sequential Logic Optimisations part1


<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166227329-6013d726-9d1e-447e-86e1-7899e2f05cdc.png" />
</p>


<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166225007-7eb12e4c-e377-4ff7-aa76-5ec938768829.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166227606-5b257c33-3763-451e-9c3f-1bd2eb2c9387.png" />
</p>


<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166228690-c8fac4aa-8c5d-491c-b32a-4c4b2d5628ba.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166228775-714aff05-88b0-486c-ac69-b619004e2c6e.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166229030-429737dd-4112-4b73-8d41-6a1c3a426ce0.png" />
</p>


<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166230193-259841b7-bdf8-4f7f-b55e-3f791cc6fdf7.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166230780-9840f89f-d706-4cc6-82fb-6c6452f01d85.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166230997-dd06341e-9651-4ed2-9f69-17f1b8c93cc2.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166231367-f3d6ae93-4d09-4882-96c8-6c05fe4efc68.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166231455-558931a2-b143-4d81-a1f0-0ad2e0cbc436.png" />
</p>





## Part 4: Sequential Logic Optimisations for unused outputs
### Sub-Part 1: Sequential Logic Optimisations part1




<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166238256-688b5011-933b-4ad0-863c-afd608dd2add.png" />
</p>




<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166237309-3f65d272-2f96-47b9-a1e5-86ad5a70cef1.png" />
</p>


<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166238772-10355be6-11ff-4b3b-a890-b6e7b7ae268a.png" />
</p>


<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166244958-95566975-c603-47f4-814e-8b894bff4e07.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166245156-cab76e1e-23d7-4d2b-a6d2-1d1de7c09ce4.png" />
</p>
<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166245287-2250f852-c1c7-4d15-8042-d12a3bd0ab3c.png" />
</p>



### Sub-Part 2: Sequential Logic Optimisations part2
<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166246835-06606c7f-979d-43bc-affc-43869913b4c2.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166247255-2e64d09f-ca9a-475f-9f19-d8e4ed72866e.png" />
</p>
<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166247397-49dbb1c0-ff4e-440a-8407-4ae27d3a1742.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166248104-515d79f9-ddd1-4c82-ac07-c0d10efdb132.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166248473-8c1e0905-acf9-4b21-aba2-bdfee0d9b9f7.png" />
</p>
<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166248895-9a6a93bd-3fc1-4c56-bc77-20d32160d968.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166249450-897866b8-79ff-448e-b515-77c85583ed0e.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166249668-a0700033-d5d5-4c93-820e-adb5cd87319e.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166249814-15b4ff6d-163a-485a-8cbb-61e2db5fca4d.png" />
</p>





# Day 4: GLS, BLOCKING VS NON-BLOCKING and Synthesis Simulation Mismatch
## Part 1: GLS Synthesis Simulation mismatch and Blocking -Nonblocking statements
### Sub-Part 1: GLS Concepts And Flow Using Iverilog

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166251593-c1f6723f-5e26-4b44-a11b-2129fd737ac1.png" />
</p>


<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166251786-a0d68fc4-de89-41a6-8c03-5019ea7a29ba.png" />
</p>

### Sub-Part 2: Synthesis Simulation Mismatch
<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166252320-d2829193-5aef-42b8-af12-df9df7d3b07a.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166252503-5a365f5e-522c-4529-a9f4-547397983276.png" />
</p>

### Sub-Part 3: Blocking And Non-Blocking Statements In Verilog
 
 -    Inside always block 
 
     -   = -> Blocking 
        -    Executes the statement in the order it is written
        -    So the first statement is evaluated before the second statement

     -  <=   Non-blocking 
        - executes all the RHS when always BLOCK is entered and assigns to LHS
        - parallel evaluation
        
   
<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166256119-6cb337c4-04bf-4554-a621-5fd83305b6df.png" />
</p>   

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166256515-57dec325-74ad-45a3-a358-dab734d13248.png" />
</p> 

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166256938-1827d1b0-dc80-44f4-bbc6-5b971f374ff7.png" />
</p> 

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166257278-3acbb01c-3279-4f6f-8250-8745c75dcf86.png" />
</p> 




## Part 2: Lab on GLS Synthesis and Simulation mismatch
### Sub-Part 1: Lab GLS Synth Sim Mismatch part1

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166258642-50e62068-8c4c-4019-9482-c9ff6220789b.png" />
</p> 

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166258803-8d748ca3-33af-46a7-9bff-682cd704813b.png" />
</p> 

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166259413-bad03f3f-086b-464a-b3da-a35f1c23239b.png" />
</p> 

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166259912-81f573a8-0a5d-46af-8c64-38e16082806e.png" />
</p> 

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166262611-ddd7459c-a601-4a1f-a21f-553e0ccf7190.png" />
</p> 
<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166263203-37911240-c79c-4192-beeb-76b0889ccdbd.png" />
</p> 


<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166263431-1370f2f6-47c4-42e8-b14d-d4c13129949b.png" />
</p> 
<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166263754-1259008d-c8c1-4e24-b5de-f95addb10342.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166264003-ce8ba5a3-ca47-473e-a4f2-258861c957c3.png" />
</p>


<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166264161-f50c0dce-b6a8-4abd-93e9-04b3d8d32ceb.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166265036-e0017633-9d60-432e-9df0-46fd5c66e683.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166265454-6a1e0cb8-df92-45a8-9f8c-55aeebd94953.png" />
</p>


<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166266557-43c8d9ac-9ce8-44d6-9786-394b0c6231c1.png" />
</p>

### Sub-Part 2: Lab GLS Synth Sim Mismatch part2

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166267448-20615494-ec29-4c2e-884d-33458d846ef1.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166267690-784d05fb-9440-42ab-b371-7519defbb855.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166269901-4ad74997-ee33-4574-af2f-55fde7d23a1e.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166270213-46f5ffae-a491-4bd7-9f99-a0675e73eb38.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166270451-58f60397-6d9e-4376-b7df-1686867ab94a.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166271917-7e0c1cce-0b79-448a-a514-99f8756d3300.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166287912-f43cbbd7-50dc-4774-94d1-f16c0de01b25.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166288927-a2c917ea-a149-4cb8-b536-c70ac66f513d.png" />
</p>


## Part 3: Lab on Synth Sim mismatch and blocking statement
### Sub-Part 1: Lab Synth sim mismatch blocking statement part1

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166290706-6f329a92-dd5b-47ec-8573-67b93934763e.png" />
</p>


<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166290171-5d2160c2-8bcb-498e-8eb0-dc6341dc23dd.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166291001-760e54da-d3a9-41bf-a234-5391ccef958c.png" />
</p>



<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166290877-05148f10-f17c-494d-8905-ebf49085001a.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166291267-1f4d50ce-e059-4ea2-87a2-55c8777a8f87.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166291521-1da8339e-84fe-4fea-b560-287bdb3536dc.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166291756-70438bae-c598-44b6-9ee7-c155ce71ddc8.png" />
</p>



### Sub-Part 2: Lab Synth sim mismatch blocking statement part2

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166292251-b94095a9-a623-4371-8669-a18eca58e2f2.png" />
</p>


<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166292411-bbb51a21-ee45-4fca-b1e5-e6296e2076ba.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166292659-6698e12a-d893-4abf-b532-62d28e5dd2c3.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166292802-3249c1fb-75f8-496c-a0a4-a563294b7019.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166294176-75804ede-f980-4f79-9860-4977ecd365e8.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166294548-0abd054f-cb81-4145-b1be-944cd23fed88.png" />
</p>


# Day 5: If,Case,For loop and For generate
## Part 1: Lab on 'Incomplete IF Case'
### Sub-Part 1: Lab Incomplete IF part1
<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166295930-4951f0ad-73d1-48d1-a841-3f9262c4b0be.png" />
</p>


<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166296069-0119e5b9-cdb6-45c8-a63a-28c00a4e4706.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166296351-866bdba1-a62e-4bbd-acf0-8d06aef0709b.png" />
</p>
<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166296602-a658b808-d681-4ee0-8c2a-cbad29f5d3ca.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166296883-9a46d5b9-e245-4011-ae85-8711bbc116a7.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166297129-fe688bd4-014e-4e9b-b02d-67dfa3f9b623.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166297283-b0c6f1c4-a3e1-4aca-83d1-324ef2c9abdf.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166297405-a9bbc183-39a0-47a0-8cad-fa7f2a1d59ae.png" />
</p>




### Sub-Part 2: Lab Incomplete IF part2


<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166297886-27b90775-8913-4349-8b4e-3f742e5fa7e4.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166298082-5f7b6034-74a3-49d1-8ba0-259cf2c4df99.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166298553-97cbb85d-84fe-4f0b-be84-dde7046de0fa.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166298803-7a6b2f58-4ca1-49c8-9c09-94c634bf49a8.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166298968-e4b894a3-0610-4f76-ae3e-1ffbc7f86832.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166299081-65c479d5-4f3f-40f0-a2b4-43a92da5757f.png" />
</p>


## Part 2: Lab incomplete overlapping
### Sub-Part 1: Lab incomplete overlapping Case part1

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166299833-3cbec761-220c-46b9-8211-012f62378274.png" />
</p>


<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166299961-cd184f89-10cf-4a50-bcc1-78b794559b43.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166300261-182be6a8-e01a-4fd0-877c-88b577655c3d.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166300539-65117db2-8b41-4245-8bf2-2bac18b518f7.png" />
</p>
<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166300837-8fba0e09-83ef-417c-b9b0-1bbadd2609ad.png" />
</p>
<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166301024-c7c9403b-8465-46be-8193-bd3f019eecf9.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166302257-d579c01e-424f-4301-8d1b-310d3d15f170.png" />
</p>
<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166302356-1f42af1f-c197-4a2e-95c3-4c8d5ae3a944.png" />
</p>


### Sub-Part 2: Lab incomplete overlapping Case part2
<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166303021-53f47c68-aeb2-46c4-8695-39dc218f70ce.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166303392-8795882a-c47d-4df2-ac6e-94f12538573c.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166303742-260b7183-61e4-48fc-a4bf-b90184eaa8dc.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166303904-78729dd2-1c25-46b3-83cf-48aeab25fb1a.png" />
</p>
<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166304036-8c89f176-2f3d-4527-9e49-ccbd5286c34c.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166304157-8ed746b9-e74d-47b9-a3e7-5c615fcd71ec.png" />
</p>

### Sub-Part 3: Lab incomplete overlapping Case part3

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166304537-ba93d1c4-643d-43e7-8e4c-13244efcbda3.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166304714-21fef08c-f629-4b49-9173-d95c49256fff.png" />
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166304820-b5a7ffc7-6f7b-453d-bcd9-edeb364d2120.png" />
</p>
<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166304904-bd7b5138-ad8f-45c4-8e60-bb47749099c2.png" />
</p>
















































        
     
         














































































































































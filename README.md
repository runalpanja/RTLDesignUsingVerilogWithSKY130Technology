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



  -  [Day 2: Timing libs,hierarchical vs flat synthesis and efficient flat coding styles]()
      - [Part 1: Introduction to Timing .libs]()
         - [Sub-Part 1: Introduction to dot Lib part1]()
         - [Sub-Part 2: Introduction to dot Lib part2]()
         - [Sub-Part 3: Introduction to dot Lib part3]()


      - [Part 2: Hierarchical vs. Flat synthesis]()
         - [Sub-Part 1: Hier synthesis flat synthesis part1]()
         - [Sub-Part 2: Hier synthesis flat synthesis part2]()
         
    
      - [Part 3: Various flop coding styles and optimization]()
         - [Sub-Part 1: Why Flops and Flop coding styles part1]()
         - [Sub-Part 2: Why Flops and Flop coding styles part2]()
         - [Sub-Part 3: Lab flop synthesis simulations part1]()
         - [Sub-Part 4: Lab flop synthesis simulations part2]()
         - [Sub-Part 5: Interesting optimisations part1]()
         - [Sub-Part 6: Interesting optimisations part2]()
     









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


### Sub-Part 2: Sequential Logic Optimizations

<p align="center">
<img src="https://user-images.githubusercontent.com/100710081/166158155-fdd8ef77-5e9a-4d09-8508-3fc63ed6a1b3.png" />
</p>



























### Sub-Part 3: Introduction to optimizations Part 3







## Part 2: Introduction to Open-Source simulator iverilog
### Sub-Part 1: Introduction to iVerilog Simulator



## Part 3: Introduction to Open-Source simulator iverilog
### Sub-Part 1: Introduction to iVerilog Simulator












































































# The 'Hack' Computer

### Objective
To build a computer from the absolute basic logical gate- NAND for all combinational chips and D Flip-Flop for all sequential chips. 

### Technical Specification of 'Hack'


### General Architechture of 'Hack'



### Setting Up

#### Simulation Tools

### Project Structure

```
hack_computer
│   README.md
│
└───01
│   |   And: .hdl, .tst, .out, .cmp    
|   |   And16: .hdl, .tst, .out, .cmp  
|   |   DMux: .hdl, .tst, .out, .cmp  
|   |   DMux4Way: .hdl, .tst, .out, .cmp  
|   |   DMux8Way: .hdl, .tst, .out, .cmp  
|   |   Mux: .hdl, .tst, .out, .cmp  
|   |   Mux4Way16: .hdl, .tst, .out, .cmp  
|   |   Mux8Way16: .hdl, .tst, .out, .cmp  
|   |   Mux16: .hdl, .tst, .out, .cmp  
|   |   Not: .hdl, .tst, .out, .cmp  
|   |   Not16: .hdl, .tst, .out, .cmp  
|   |   Or: .hdl, .tst, .out, .cmp  
|   |   Or8Way: .hdl, .tst, .out, .cmp  
|   |   Or16: .hdl, .tst, .out, .cmp  
|   |   Xor: .hdl, .tst, .out, .cmp  
|
└───02
│   │   Add16: .cmo, .hdl, .out, .tst
|   |   ALU: .cmp, .hdl, .out, .tst
|   |   ALU-nostat: .cmp, .tst
|   |   FullAdder: .cmp, .out, .tst
|   |   HalfAdder: .cmp, .hdl, .out, .tst
|   |   Inc16: .cmp, .hdl, .out, .tst
|   |   Or16Way: .hdl
|
└───03
|   |   Bit: .cmp, .hdl, .out, .tst
|   |   PC: .cmp, .hdl, .out, .tst
|   |   RAM4K: .cmp, .hdl, .out, .tst
|   |   RAM8: .cmp, .hdl, .out, .tst
|   |   RAM16K: .cmp, .hdl, .out, .tst
|   |   RAM64: .cmp, .hdl, .out, .tst
|   |   RAM512: .cmp, .hdl, .out, .tst
|   |   Register: .cmp, .hdl, .out, .tst
|
└───04
|   |   Computer: .cmp, .hdl, .out, .tst
|   |   ComputerAdd: .cmp, .hdl, .out, .tst
|   |   ComputerAdd-external: .cmp, .hdl, .out, .tst
|   |   ComputerMax: .cmp, .hdl, .out, .tst
|   |   ComputerMax-external: .cmp, .hdl, .out, .tst
|   |   ComputerRect: .cmp, .hdl, .out, .tst
|   |   ComputerRect-external: .cmp, .hdl, .out, .tst
|   |   CPU: .cmp, .hdl, .out, .tst
|   |   CPU-external: .cmp, .hdl, .out, .tst
|   |   Memory: .cmp, .hdl, .out, .tst
|
└───05
|   |   Add: .asm, .hack
|   |   Assembler.py
|   |   Makefile
|   |   Max: .asm, .hack
|   |   MaxL: .asm, .hack
|   |   Pong: .asm, .hack
|   |   PongL: .asm, .hack
|   |   README
|   |   Rect: .asm, .hack
|   |   RectL: .asm, .hack
|   |   test6.sh
|
└───tools
|   |   Assembler: .bat, .sh
|   |   CPUEmulator: .bat, .sh
|   |   HardwareSimulator: .bat, .sh
|   |   JackCompiler: .bat, .sh
|   |   TextComparer: .bat, .sh
|   |   VMEmulator: .bat, .sh
|   |   Noam Nisan, Shimon Schocken - The Elements of Computing Systems_ Building a Modern Computer from First Principles-The MIT Press (2005).pdf
|   
|   └───bin
|   └───builtInChips
|   └───builtInVMCode
|   └───OS

'''

### Hardware Description Language (HDL)

* HDL is a **functional/declarative** language 
* Order of HDL statements is **insignificant**
* Only prerequisite to use a build-in/user-defined chip is the knowledge of its **interface**

An HDL definition of a chip consists of a **header section** and a **parts section**.  <br>
The **header section** specifies the chip interface, namely the chip name and the names of its input and output pins. <br>
The **parts section** describes the names and topology of all the lower-level parts (other chips) from which this chip is constructed. Each part is represented by a statement that specifies the part name and the way it is connected to other parts in the design.

#### Testing

1. Manual Testing
2. Script Testing

The script lists a series of testing scenarios, designed to simulate the various contingencies under which the chip will have to operate in ‘‘real-life’’ situations.<br>

The script instructs the simulator to bind the chip inputs to certain data values, compute the resulting output, and record the test results in a designated output file.

### 'Hack' Assembbly Language


### 'Hack' Arithmetic Logic Unit (ALU)


### Memory Units

#### Bit

#### Register

#### Counter


### Interfacing (Input Output)

#### Output Device- **Screen**

#### Input Device- **Keyboard**


### CPU Architechture of 'Hack'


### References
1. Digital Logic and Computer Design- M. Morris Mano
2. The Elements of Computing Systems- Noam Nisan and Shimon Schocken






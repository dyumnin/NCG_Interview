# Dyumnin Semiconductors, Take home coding test for new college graduates.
Take home coding test.

Instructions:
## Step 1:
1. Clone this repository.
2. Create a branch with "candidate/{your name} as the branch name.
3. Create a Xilinx project called ddr4 for part  xcku115-flvd1517-1-c
4. and use the Xilinx ddr4 MIG generator to generate a DDR4 controller and physical layer IP with AXI4 Interface and 72 bit datawidth
5. Checkin all the generated files and tag it as Step1

## Step 2:
 
 Write a verilog module which 
 1. At reset sets the address to 0.
 2. Has a simple interface (enable(input),ready(output) data(input)) On one end which  takes in 8 bit numbers, concats them to generate a 72 bit number and writes this result to the ddr4 axi interface generated in step 1. and increments the address.
 
 Write another module which has an interface of (enable, ready, address(in), data(out)) and interfaces to the same DDR logic in Step 1. and returns the data in DDR for the specified address.

Checkin the files and tag it as Step2

## Step 3:
Checkin the testplan for the dut containing logic in step1 and step2 and tag it as Step3

## Step 4:

Implement the verification env and write and verify atleast 2 test(should contain a ddr write and read).
If you know python, then you can do the verification using cocotb.

## Step 5.

Create a pull request on the original repo with your code submission.


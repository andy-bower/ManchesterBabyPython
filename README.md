# ManchesterBaby
Manchester Baby (Small Scale Experimental Machine)

## Usage: 
	python3 ManchesterBaby.py <filename>
## example: 
	python3 ManchesterBaby.py Samples/hfr989.asm

## About

The [Manchester Small Scale Experimental Machine](https://en.wikipedia.org/wiki/Manchester_Small-Scale_Experimental_Machine) was the worlds first computer capable of executing a stored program.  The 32-bit architecture utilised an instruction set using only 3 bits allowing 8 possible instructions.  The program was stored in 32 memory locations (or store lines) with both data and program sharing storage (von Neumann architecture).

The Python Emulator implements a simplified version of the Manchester Baby.  The main program is able to read simple assembler files and execute the programs contained.  The program displays the status of the machine at the start and end of the program run.


## Instruction Set
* JMP Copy content of the specified line into the CI
* JRP Add the content of the specified line into the CI
* LDN Copy the content of the specified line, negated, into the accumulator
* STO Copy the content of the accumulator to the specified store line
* SUB Subtract the content of the specified line from the accumulator
* CMP If the accumulator is less than 0 increment the CI
* STP Halt the Baby and light the ‘stop lamp’


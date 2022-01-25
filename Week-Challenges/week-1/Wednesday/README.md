## Answers Wednesday 12/01/2022

### 1 - Learn about binary, decimal and hexadecimal numbers
- Binary numbers: Is a number expressed in the Base 2 (0-1).
- Decimal numbers: Base 10 number and requiring 10 different numerals (0,1,2,3,4,5,6,7,8,9)
- Hexadecimal numbers: Base 16 number. The system has this numerals (0,1,2,3,4,5,6,7,8,9) and the two digit numbers are represented by single symbol (A= 10,B= 11,C= 12,D= 13,E= 14,F= 15)

### 2 - Translate the year you where born to binary, decimal and hexadecimal
- Decimal number: 1998
- Binary: 11111001110
  * It can be express like 1024 + 512 + 256 + 128 + 64 + 8 + 4 + 2
  * The answer is: 11111001110
- Hexadecimal: 7CE
  * 1998/16 = 124.875 (0.875*16= 14) - E
  * 124/16 = 7.75 (0.75*16= 12) - C
  * 7/16 = 0.4375 (0.4375*16= 7) - 7
    
### 3 - Translate 51966 into hexadecimal and binary
- Decimal number: 51966
- Binary: 1100101011111110
  * It can be express like 32768 + 16384 + 2048 + 512 + 128 + 64 + 32 + 16 + 8 + 4 + 2
  * The answer is: 1100101011111110
- Hexadecimal: CAFE
  * 51966/16 = 3247.875 (0.875*16= 14) - E
  * 3247/16 = 202.9375 (0.9375*16= 15) - F
  * 202/16 = 12.625 (0.625*16= 10) - A
  * 12/16 = 0.75 (0.75*16= 12) - C

### 4 - Use a Low-level language, for example MIPS aseembler, to do so, you will need to follow [this](https://github.com/corecodeio/bootcamp-from-scratch/blob/main/src/technologies/2022/week1/resources/MIPS.md) guide. We recomend to check the guide first but also [this](https://courses.cs.vt.edu/cs2506/Fall2014/Notes/L04.MIPSAssemblyOverview.pdf) presentation could be helpful.
-- Done

### 5 - Base on the examples and the guide of the low-level language:
- #### 5.1 - Create a program to add two numbers given by the user
`.data
	num1: .asciiz "\nFirst number: "
	num2: .asciiz "\nSecond number: "
.text`

`main:
	li $v0, 4
	la $a0, num1
	syscall
	li $v0, 5
	syscall
	move $t0, $v0
	li $v0, 4
	la $a0, num2
	syscall
	li $v0, 5
	syscall`

- #### 5.2 - Create a program that display your name
`.data message: .asciiz "\nWilson Barrientos\n" .text main: li $v0, 4 la $a0, message syscall`
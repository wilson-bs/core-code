# core-code
Core Code Bootcamp

## Answers Tuesday 11/01/2022

### 1 
- Compilation needs a compiler to transform the code into something that permits the PC to understand the instructions.
This option takes all the code and if it finds some mistake does not permit finish the compilation process.
- Interpretation means that does not require a compiler, it is making the process while every code line is running.

### 2
- It is compiled, because requires a compiler to translate the code to a binary byte-code.

### 3
1. Start
2. Set the value of dollar compare to local currency
3. Dollar = 7.70
4. Read local_currency
5. result = local_currency * Dollar
6. print (result)
7. End

### 4
-- Read about Pseudocode

### 5
- It is helpful since it allows you to have a natural language code that can serve as a base for when you start coding in the programming language to be used.
Having already defined the variables, functions, conditionals, cycles, etc.

### 6
1. Start
2. currentYear = 2022
3. Read bornYear
4. aprox_age = currentYear - bornYear
5. print (aprox_age)
6. End

### 7
-- Read about flowcharts

### 8
- It makes it possible to understand the flow of the code, knowing how it reacts to user inputs, making debugging easier in the event of errors or inconsistencies in the results obtained as expected.

### 9
- Some examples are:
  * High-level languages: Javascript, Java, C#
  * Low-level languages: Assembler

-----------------------------------------------------
## Answers Wednesday 12/01/2022

### 1 
- Binary numbers: Is a number expressed in the Base 2 (0-1).
- Decimal numbers: Base 10 number and requiring 10 different numerals (0,1,2,3,4,5,6,7,8,9)
- Hexadecimal numbers: Base 16 number. The system has this numerals (0,1,2,3,4,5,6,7,8,9) and the two digit numbers are represented by single symbol (A= 10,B= 11,C= 12,D= 13,E= 14,F= 15)

### 2
- Decimal number: 1998
- Binary: 11111001110
  * It can be express like 1024 + 512 + 256 + 128 + 64 + 8 + 4 + 2
  * The answer is: 11111001110
- Hexadecimal: 7CE
  * 1998/16 = 124.875 (0.875*16= 14) - E
  * 124/16 = 7.75 (0.75*16= 12) - C
  * 7/16 = 0.4375 (0.4375*16= 7) - 7
    
### 3
- Decimal number: 51966
- Binary: 1100101011111110
  * It can be express like 32768 + 16384 + 2048 + 512 + 128 + 64 + 32 + 16 + 8 + 4 + 2
  * The answer is: 1100101011111110
- Hexadecimal: CAFE
  * 51966/16 = 3247.875 (0.875*16= 14) - E
  * 3247/16 = 202.9375 (0.9375*16= 15) - F
  * 202/16 = 12.625 (0.625*16= 10) - A
  * 12/16 = 0.75 (0.75*16= 12) - C

### 4
-- DONE

### 5
#### 5.1
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

#### 5.2
`.data message: .asciiz "\nWilson Barrientos\n" .text main: li $v0, 4 la $a0, message syscall`

-----------------------------------------------------
## Answers Thursday 13/01/2022

### 1 - Search for real word applications of Javascript
- Web Development
- Games
- Mobile Applications
- Desktop Aplications
- Web Servers
- IoT (Internet of Things)

### 4 - Follow the github course
In progress...

-----------------------------------------------------
#Week 2
## Answers Monday 17/01/2022
### 1 - Follow the github course
In progress...

### 2
--Done

### 3
--Done

### 4
https://www.codewars.com/users/wilson_bs/

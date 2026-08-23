Binary Numbers :
----
Binary Numbers are of base/radix 2 - and thus they use only 2 digits [ 0 , 1 ] 

Binary number 11010.11 is 26.75

Number Base Conversion : 
---
- The conversion of a number in base r to decimal is done by expanding the number in a power
series and adding all the terms
- the conversion of a decimal integer to a number in base r is done by dividing the number and all successive quotients by r and accumulating the remainders.
  
- The conversion of a decimal fraction to a binary is accomplished by a method similar to that of used for integers , however multiplication is used instead of division
- eg:
  ![image](https://github.com/NihalSinghBisht/rtl-design-notes/blob/main/01-Digital-Electronics/Digital%20Systems%20and%20Binary%20Numbers/image1.jpg?raw=true)

- The conversion of decimal numbers with both integer and fraction parts is done by cmverting the integer and the fraction separately and then combining the two answers

Complements :
----
- Complements are used in digital computer to simplify the subtraction operation and for  logical manipulation. Simplifying operations leads lo simpler, less expensive circuits to implement the operations
- there are two types of complements for each base r system : the radix complement and the diminished radix complement --> r's complement and the (r-1)'s complement
- thus , 1's and 2's complement for binary numbers and 9's and 10's complement for the decimal numbers


Radix Complement :
----
- the r's complement of an n digit number in N in base r is given by r^n - N , N !=0 and is O for n=0 
- we note that the r's complement is obtained by adding 1 to the (r - 1)'s complement

- a short trick ( img 4 )
- ![image](https://github.com/NihalSinghBisht/rtl-design-notes/blob/main/01-Digital-Electronics/Digital%20Systems%20and%20Binary%20Numbers/image4.png?raw=true)


Subtraction with complements : 
----
using the r's complement 
image 5
![image](https://github.com/NihalSinghBisht/rtl-design-notes/blob/main/01-Digital-Electronics/Digital%20Systems%20and%20Binary%20Numbers/image5.png?raw=true)

example : image 6 
![image](https://github.com/NihalSinghBisht/rtl-design-notes/blob/main/01-Digital-Electronics/Digital%20Systems%20and%20Binary%20Numbers/image6.png?raw=true)
- When subtracting with complements, we recognize the negative answer from the absence of the end carry and the complemented result


Using the (r-1)'s complement 
- Since (r-)'s complement is one less than the r's complement and because of this the result is one less than the correct difference when an end carry occurs !
Removing the end carry aod
adding I to the sum is refd to as end-around carry

- if theres no end carry : image 7
- ![image](https://github.com/NihalSinghBisht/rtl-design-notes/blob/main/01-Digital-Electronics/Digital%20Systems%20and%20Binary%20Numbers/image7.png?raw=true)


Signed Binary Numbers : 
----
- To represent negative numbers we need a notation for the negative values
- It is customary to represent the sign with a bit placed in the leftmost position of the number. The convention is to make the sign bit 0 for positive and 1 for negative
- USER DECIDES if the number is signed or unsigned !!
- THERE ARE 3 CONVENTIONS
    - signed magnitude
    - signed complement (1's)
    - signed complement (2's)
 
- Signed complement method :
   - In this system, a negative number is indicated by its complement.
     Whereas the signed-magnitude system negates a number by changing its sign, the             signed-complement system negates a number by taking its complement
   - The signed-complement system can use either the 1's or the 2's complement,
     but the 2's complement is the most common
   - eg : image 8
   - ![image](https://github.com/NihalSinghBisht/rtl-design-notes/blob/main/01-Digital-Electronics/Digital%20Systems%20and%20Binary%20Numbers/image8.png?raw=true)


Binary Codes 
----
If we inspect the bits of a computer at random, we will find that most of the time they
represent some type of coded information rather than binary numbers.

BCD CODE 
----
image 9 

the table shows that for one decimal digit we require 4 bit code , for k decimal digits we'll require 4k bits in BCD 
image 10 


Gray Code 
------
- The advantage of the Gray code over the straight binary number
  sequence is that only one bit in the code group changes in going from one number to the next
- For eg in going from 7 - 8 (gray code changes from 0100 to 1100 changing only the first bit , the other 3 bits remain the same)


ASCII Character Code 
----
- The standard binary code for the alphanumeric characters is the American Standard Code
  for lnformation Interchange (ASCII).
- It uses 7bits to code 128 characters

Error Detecting Code 
----
- To detect errors in data communication and processing, an eighth bit is sometimes added to the
ASCII character to indicate its parity
- The parity bit is helpful in detecting errors during the transmission of information from one location to another - this function is handled by generating an even parity bit at the sending end for each character , now the 8 bit characters that include parity bits are transmitted to their destination - the parity bit is checked at the receiving end - but the even combination of errors goes undetected 


Binary Storage and Registers 
-----
- Registers
   - collection of latches is known as a register (a register stores multiple bits)
   - composed of logic gates that are interconnected in a desired manner
 

Register Transfer 
-----
- An operation that consists of transfer of binary information from one set of registers to another set of registers



   

  


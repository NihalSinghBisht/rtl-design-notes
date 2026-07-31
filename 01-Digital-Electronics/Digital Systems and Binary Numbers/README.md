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
- Complements are used in digital romputem lo simplify the submaion operation and for  logical manipulation. Simplifying operations leads lo simpler, less expensive circuits to implement the operations
- there are two types of complements for each base r system : the radix complement and the diminished radix complement --> r's complement and the (r-1)'s complement
- thus , 1's and 2's complement for binary numbers and 9's and 10's complement for the decimal numbers


Radix Complement :
----
- the r's complement of an n digit number in N in base r is given by r^n - N , N!=0 and is O for N=0 
- we note that the r's complement is obtained by adding 1 to the (r - 1)'s complement

- a short trick ( img 4 )

Subtraction with complements : 
----
using the r's complement 
image 5

example : image 6 

- When subtracting with complements, we recognize the negative answer from the absence of the end carry and the complemented result


Using the (r-1)'s complement 
- Since (r-)'s complement is one less than the r's complement and because of this the result is one less than the correct difference when an end carry occurs !
Removing the end carry aod
adding I to the sum is refd to as end-around carry

- if theres no end carry : image 7


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





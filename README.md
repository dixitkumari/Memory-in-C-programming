# Memory-in-C-programming

Hexadecimal representation in c  
In hexadecimal number system we use 16 different digits so its base is 16. 
List of all hexadecimal digits

<img width="788" height="601" alt="image" src="https://github.com/user-attachments/assets/5ea0ebbc-0c5d-4669-a0ea-37ffc8136521" />

To convert the binary number into hexadecimal number we have to make a group of four binary numbers from right to left 

 
Binary number = 11000111110101 
Group of four digits from right side are : 
0011
0001
1111
0101

<img width="675" height="59" alt="image" src="https://github.com/user-attachments/assets/99feade5-3352-4552-99f0-4a4a6124001a" />

equivalent hexadecimal number will be 31F5


 **address range which can be represented in 20 bit**

 <img width="721" height="59" alt="image" src="https://github.com/user-attachments/assets/b31160c2-7ccf-4554-bb1a-16cb40cf3b80" />

in C programming any hexadecimal no. starts with 0x or 0X 
so the memory address in turbo c 3.0 of all the variable must be within 0x00000 to 0xFFFFF

 
2^10 = 1KB 
2^20 = 1MB 
2^30 = 1GB ; where 10 , 20 , 30 are in bit


**Memory cell in computer**

entire RAM has been divided in numbers of equal parts which are known as memory cells .


<img width="725" height="599" alt="image" src="https://github.com/user-attachments/assets/5d9c66f3-9efe-4326-8948-2d137f98884b" />

Each cell can store one-byte data
Data are stored in the  
binary number system. That is a character data reserves one  
memory cell while floating data reserves four memory cells.


Each memory cell has unique address. Address is always in 
whole number and must be in increasing order . 


**for example** take 
int a = 4 

When the program is compiled or executed, the system allocates memory to hold the variable. The amount of memory allocated depends on the variable’s data type. For example, an integer variable may typically require 4 bytes of memory . This is called  memory allocation.


<img width="798" height="88" alt="image" src="https://github.com/user-attachments/assets/40fd2c6e-66d8-4dc0-ad0b-daab51539ab7" />


the memory address of first cell is 0x5000 , so the memory address of the next memory cell would be 0x5001 since the integer data always stores at  
continuous memory
 location and
 always in increasing order 
 as we know memory address  


 **RAM**  has been divided into two parts : 
  {1} **EXTENDED MEMORY** 
  {2} **RESIDENCE MEMORY**


  <img width="721" height="492" alt="image" src="https://github.com/user-attachments/assets/b4b73e00-91e7-41ea-9a86-b3855bf18e44" />


in Turbo C 3.0 compiler size of residence memory is only 1 MB and the extended memory is useless to us as any programme that we executes it is stored in residence memory only . 



**physical address of computer** 
All the c variables are stored in the residence memory. 
In turbo C 3.0, 20 bits address of the memory cell is 
known as physical address or real address. In 20 bits,  
we can represent address from 0x00000 to 0xFFFFF. That  
is all c variables must have memory address within this  
range. 


<img width="776" height="657" alt="image" src="https://github.com/user-attachments/assets/1d696b4e-6329-455a-93fc-a8a284b23b78" />

Memory address of any variable is decided by Compiler


 we can say in 16 bits compilers address must be  
within 0x0000 to 0xFFFF and in 32 bits compilers memory  
address must be within 0x00000000 to 0xFFFFFFFF


<img width="794" height="45" alt="image" src="https://github.com/user-attachments/assets/04b47733-f1f8-41ce-b4e8-ff9cb214ccd4" />

for 32 bytes address memory would be 4 GB



**Segmentation in c programming language**

Residential memory of RAM of size 1MB has divided into 16  
equal parts. These parts is called segment. Each segment  
has size is 64 KB. 
16 * 64 KB = 1 MB 


<img width="691" height="394" alt="image" src="https://github.com/user-attachments/assets/ca9afad2-1f57-4711-a370-6a790eb128a0" />

This process of division is known as segmentation. 

Each segment has divided into two parts. 
1. Segment no (4 bit) 
2. Offset address (16 bit)

   <img width="539" height="243" alt="image" src="https://github.com/user-attachments/assets/607a6885-c0a3-4d5d-a946-e60ffccf77d5" />


**DATA SEGMENT IN C**

All the segments are used for specific purpose. Like segment number 15 is 
used for ROM, segment number 14 is used for BIOS 


<img width="703" height="594" alt="image" src="https://github.com/user-attachments/assets/276aad93-fb47-48c5-9296-19eb76cb38cb" />

Segment number eight has special name which is known as data segment. This 
segment has been divided into four parts. This is very important for c 
programming 


<img width="937" height="321" alt="image" src="https://github.com/user-attachments/assets/4e1b1870-d1d4-4b19-9e81-7c5f10b3c003" />


# VM_Squad
This projects is the CS433 Group project
Contributers are: 
Raul Perez
Aaron Brunette
Andrew Zhang


This project consisted of writing a program that translates logical to physical addresses for a virtual address space of size 2^16 = 65,536 bytes. 

The program will read from a file containing logical addresses and, using a TLB as well as a page table, will translate each logical address to its corresponding physical address and output the value of the byte stored at the translated physical address. 

The goal behind this project is to simulate the steps involved in translating logical to physical addresses.

The program will read a file containing several 32-bit integer numbers that represent logical addresses. However, it only looks at 16-bit addresses, so it masks the rightmost 16 bits of each logical address. These 16 bits are divided into an 8-bit page number and an 8-bit page offset.


Memory specifics:

28 entries in the page table

Page size of 28 bytes

16 entries in the TLB

Frame size of 28 bytes

256 frames

Physical memory of 65,536 bytes (256 frames × 256-byte frame size)

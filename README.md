# EXPERIMENT--01-ALP-FOR-8086
```
Name :  Syed Mokthiyar S M
Roll no :212222230156
Date of experiment : 13.8.2024
```


## Aim: To Write and execute ALP on fundamental arithmetic and logical operations
## Components required: 8086  emulator 
## Theory 
Running The Emulator (emu8086) Intro 8086 Microprocessor Emulator, also known as EMU8086, is an emulator of the program 8086 microprocessor. It is developed with a built-in 8086 assembler. This application is able to run programs on both PC desktops and laptops. This tool is primarily designed to copy or emulate hardware. These include the memory of a program, CPU, RAM, input and output devices, and even the display screen. There are instructions to follow when using this emulator. It can be executed into one of the two ways: backward or forward. There are also examples of assembly source code included. With this, it allows the programming of assembly language, reverse engineering, hardware architecture, and creating miniature operating system (OS). The user interface of 8086 Microprocessor Emulator is simple and easy to manage. There are five major buttons with icons and titles included. These are “Load”, “Reload”, “Step Back”, “Single Step”, and “Run”. Above those buttons is the menu that includes “File”, “View”, “Virtual Devices”, “Virtual Drive”, and “Help”. Below the buttons is a series of choices that are usually in numbers and codes. At the leftmost part is an area called “Registers” with an indication of either “H” or “L”. The other side is divided into two, which enables users to manually reset, debug, flag, etc. What is 8086 emulator emu8086 is an emulator of Intel 8086 (AMD compatible) microprocessor with integrated 8086 assembler and tutorials for beginners. Emulator runs programs like the real microprocessor in step-by-step mode. it shows registers, memory, stack, variables and flags.


 ## Running the Emulator :
1.	Download and install emu8086 (www.emu8086.com) It is usually installed in C:\EMU8086 subfolder in the “Windows” directory
2.	  Run  emu8086 icon (on the desktop or in the c:\EMU8086 folder of window) It has green color 
 
 
3.		write the code for the appropriate program for ADDITION,SUBTRACTION, MULTIPLICATION,  DIVISION operations 

4.	 Compile the program and check for the errors 
5.	Run (once there is no syntax error) 

6.	Click OK to see/view the output of your program on the Emulator screen. 


7.	After running the program, another menu screen will be displayed, where you have the option to “View” symbol table,
8.	 


![image](https://user-images.githubusercontent.com/36288975/189273263-d65baae9-4b8f-4723-afb3-c0ffa4052b04.png)











9.	Click on emulate to start emulation 








![image](https://user-images.githubusercontent.com/36288975/189273273-9bb36ec1-e2e8-4892-8d35-37707332bfdc.png)








10.	If no errors are found click on run the program and check the status of various flags in the flags tab as shown below 






![image](https://user-images.githubusercontent.com/36288975/189273277-113a2a33-4a40-4ff8-95a5-ecd3a1f504fe.png)







## Programs for arithmetic  operations

## Addition  
```c
org 100h
mov al,024h;
mov bl,al;
add bl,al;
mov [0123h],bl;
ret
```

## Output 

![318728554-ce0a7579-1e04-4f7e-8427-af7e0467ae2b](https://github.com/user-attachments/assets/0424a209-2eb3-41ca-aa11-0611d3f3172e)
 
 
## Subtraction :
```c
org 100h
mov al,024h;
mov bl,[0123h+02];
sub bl,al;
mov [0123h+04],bl;
ret
```
 
## Output  

![318728973-c8cc0918-d169-4573-bd2c-acd61e534281](https://github.com/user-attachments/assets/94912a59-cc00-466c-9ded-d28059069de9)

## Multiplication:
```c
org 100h
mov bx,0015h;
mov al,[bx];
mul bl;
mov [0015h+04],al;
ret
```
 ## Output :
 
![318729702-cb7911a3-753b-444b-ad1d-50114c64ca97](https://github.com/user-attachments/assets/303cafe6-fe7c-451b-b96b-aaa31cb3601e)


## Division :
```c
org 100h
mov bx,0040h;
mov al,[bx+02];
div bl;
mov [0040h+04],al;
ret
```

## Output : 

![318730288-8e1b0784-89f4-4e15-aada-85f2871a5ea2](https://github.com/user-attachments/assets/6e6147c5-eeb5-4161-9797-1f63ef239bc0)

## Programs for logical operations

## AND
```c
org 100h
mov bx,1000h;
and bx,1111h;
mov [0040h+02],bx;
ret
```
## output

![318730796-380eb8b2-be95-414c-9eef-e7455ac8083a](https://github.com/user-attachments/assets/92da8c10-70c2-4b86-b5fe-98b24802542c)

## OR
```c
org 100h
mov ax,[0040h+06];
mov bx,1000h;
or ax,bx;
mov [0040h+02],ax;
ret
```

## output

![318731268-372bd3ba-09b4-47c0-8cd3-2a6c5e9447b0](https://github.com/user-attachments/assets/fed96215-4ac2-46fe-aba6-b8f68d610e5a)

## NOT
```c
org 100h
mov bx,0040h;
mov ax,[bx]; 
not al;
mov [0040h+04],ax;
ret
```

## output
![318732277-57ff6c88-2341-4eb3-bbfc-b1f9cb8fe8cc](https://github.com/user-attachments/assets/e2155d04-ee23-4ff8-bf8a-3352bbb5b2bb)

## XOR
```c
org 100h
mov bx,0040h;
mov ax,[bx]; 
xor ax,bx;
mov [0040h+04],ax;
ret
```

## output

![318732494-4ef2fb5c-0e99-4427-93b6-7cafa2ae77ff](https://github.com/user-attachments/assets/8beaf27b-29e7-49cb-b6e2-527ad00df6b2)

## Result :
 
Thus, ALP for fundamental arithmetic and logical operations are executed successfully.









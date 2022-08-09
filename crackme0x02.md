https://github.com/Maijin/radare2-workshop-2015/tree/master/IOLI-crackme/bin-linux

Check the file.

![image](https://user-images.githubusercontent.com/93418272/183669154-1190be60-2153-4d3e-85c8-6c1388ae50b5.png)


Test the program out.

![image](https://user-images.githubusercontent.com/93418272/183669172-8f068de8-1a0b-4644-8e58-2a4b27b6da30.png)


Analyze the program in GDB.

![image](https://user-images.githubusercontent.com/93418272/183669201-e80210ed-1a1c-416a-8763-15fa362a7c7f.png)


There are two ways to find the password.

The lines inside the orange box can be equated to give us an answer.

![image](https://user-images.githubusercontent.com/93418272/183669270-7607e182-0451-4392-aaa8-08b0c4a2e920.png)


Set a breakpoint at the cmp line and print out the variable for [ebp-0xc]

![image](https://user-images.githubusercontent.com/93418272/183669292-51a12e05-3f9b-41e2-8be9-62600826000c.png)


We can also analyze the program in Ghidra.

Assembly:

![image](https://user-images.githubusercontent.com/93418272/183669328-acd7da07-676d-4197-9120-234f907aaff8.png)


Decompile:

![image](https://user-images.githubusercontent.com/93418272/183669348-0bd7746d-0448-4f07-bf79-d1c161471d2d.png)


Password is hard coded User Input is compared with password

Test the password

![image](https://user-images.githubusercontent.com/93418272/183669371-8e691d8e-5d06-4056-9c47-3588f6563070.png)

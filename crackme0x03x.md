https://github.com/Maijin/radare2-workshop-2015/tree/master/IOLI-crackme/bin-linux

Check the file.

![image](https://user-images.githubusercontent.com/93418272/183892904-b98418ae-79fd-4afd-abed-b84732d00355.png)


Test the program out.

![image](https://user-images.githubusercontent.com/93418272/183892920-1d436783-c578-4db7-b100-5814023d77c5.png)


Analyze the program in GDB.

![image](https://user-images.githubusercontent.com/93418272/183892941-801b3b85-421a-481d-a955-7e3d96525415.png)


crackme0x03x is very similar to crackme0x02x but has a test function built instead of compare. 

There are two ways to find the password.

![image](https://user-images.githubusercontent.com/93418272/183893015-7a68d075-9f97-4048-a9cd-6c8f48462074.png)


The lines inside the orange box can be equated to give us an answer.

![image](https://user-images.githubusercontent.com/93418272/183893034-6caa0219-03f1-4d85-907e-9ec5caa15fd8.png)


Set a breakpoint at the test function and print out the variable for [ebp-0xc]

![image](https://user-images.githubusercontent.com/93418272/183893101-8d03f789-259d-4931-ad87-d7e2477935ff.png)


Disassemble the test function 

![image](https://user-images.githubusercontent.com/93418272/183893077-b65c7031-2bd5-477d-9183-b164bfdbffc5.png)


Run a breakpoint to find out the value of the strings.

![image](https://user-images.githubusercontent.com/93418272/183893123-10b72c3e-064e-454a-93d5-4176bb369cca.png)


Looks like its encrypted strings and just an obfuscation for the challenge.

Test the password

![image](https://user-images.githubusercontent.com/93418272/183893142-60834f3c-7601-4ad6-9f7d-e2a5350f1cd1.png)

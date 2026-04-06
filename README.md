# Digital-Signal-Processing--Convolution
## Aim:
                  To perform linear convolution using MAT LAB.
## Software Required:
MAT LAB R2012
## Algorithm:
Step 1: Open mat lab. Write the program.

Step 2: Read the first input sequence.

Step 3: Read the second impulse sequence.

Step 4: Plot the input sequences with x-label and y-label with suitable title. 

Step 5: Perform convolution for both the sequences using conv2() function.
  
Step 6: Plot the sequence with x-label and y-label with suitable title

Step 7: Terminate the program.

## PROGRAM: 
```
clc;
clear all;
close all;
a= input('enter the stating x(n)');
x = input(' enter the x(n) sequence');
n=a:1:length(x)+a-1;
figure(1);
stem(n,x);
xlabel('time');
ylabel('amplitude');
title('input sequence');
b=input('enter the starting h(n)');
y=input('enter the h(n) sequence');
m=b:1:length(y)+b-1;
figure(2);
stem(m,y);
xlabel('time');
ylabel('amplitude');
title('impulse response')
z=conv2(x,y);
nl=a+b:1:length(z)+a+b-1;
figure(3);
stem(nl,z);
xlabel('time');
ylabel('amplitude');
title('linear convolution')
```

## OUTPUT:
<img width="696" height="620" alt="image" src="https://github.com/user-attachments/assets/4f130606-3075-474a-8cde-1463d4ecd20e" />
<img width="692" height="622" alt="image" src="https://github.com/user-attachments/assets/9c564aa7-2c00-4cdb-9f28-a80ac5526741" />
<img width="696" height="626" alt="image" src="https://github.com/user-attachments/assets/e8bc6821-1c5f-4334-8ecd-11ed041a8c94" />


## RESULT:
<img width="533" height="1600" alt="image" src="https://github.com/user-attachments/assets/627a1122-fb08-439e-95b8-ba5d7f2eab19" />


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
~~~
clc; % clear screen
clear all; % clear screen
close all; % close all figure windows
% INPUT SEQUENCE
a=input('enter the starting x(n)');
x=input('enter the x(n) sequence');
n=a:1:length(x)+a-1;
figure(1);
stem(n,x);
xlabel('time');
ylabel('amplitude');
title('input sequence');
% IMPULSE SEQUENCE
b=input('enter the starting h(n)');
y=input('enter the h(n) sequence');
m=b:1:length(y)+b-1;
figure(2);
stem(m,y);
xlabel('time');
ylabel('amplitude');
title('impulse response')
% LINEAR CONVOLUTION
z=conv2(x,y);
n1=a+b:1:length (z)+a+b-1; 
figure(3);
stem(n1,z);
xlabel('time');
ylabel('amplitude');
title('linear convolution');
~~~

## OUTPUT:

![15064f4e-4d43-4af6-ac6d-da87f47a2b4b](https://github.com/user-attachments/assets/7f1749b0-9dfb-4451-b063-952013a52a7d)

![70e5d4c5-caf3-45e1-9a4d-86928f7fe26e](https://github.com/user-attachments/assets/072ba344-de73-4be1-bb8f-e27a6fe290fb)

![8549475d-f995-42d8-8427-7fc5bc5a2980](https://github.com/user-attachments/assets/5fc53c9c-ab84-486b-b068-c1901857bdb7)

## RESULT:

![83e50d58-1766-495e-9b8a-9b2ef802f5c6](https://github.com/user-attachments/assets/f1ef7d74-2084-40fe-a863-da8f957754ed)

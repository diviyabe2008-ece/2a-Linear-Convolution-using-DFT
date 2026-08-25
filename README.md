## EXPT 2
## LINEAR CONVOLUTION-USING-DFT

## AIM:
To perform and verify linear convolution operation of two given sequences using SCILAB.

## APPARATUS REQUIRED:
PC installed with SCILAB

## PROGRAM:
## LINEAR CONVOLUTION
```
clc;
clear;
x = [1 1 1 1];
h = [1 2 3 4];
m = length(x);
n = length(h);
a=0:1:m-1;
b=0:1:n-1;
subplot(3,1,1);
plot2d3(a,x);
xlabel('Time');
ylabel('Amplitude');
title('Graphical Representation of Input Signal X');
subplot(3,1,2);
plot2d3(b,h);
xlabel('Time');
ylabel('Amplitude');
title('Graphical Representation of Impulse Signal h');
for i = 1: n+m-1
conv_sum = 0;
for j = 1:i
if (((i-j+1) <= n)&(j <=m))
conv_sum = conv_sum + x(j)*h(i-j+1);
end;
y(i) = conv_sum;
end;
end;
disp(y,'Convolution Sum using Direct Formula Method = ')
subplot(3,1,3);
plot2d3(y)
title('Graphical Representation of output Signal y');
```


### CALCULATIONS:

<img width="1600" height="1412" alt="WhatsApp Image 2026-08-25 at 9 28 34 AM" src="https://github.com/user-attachments/assets/cbebd795-0d9c-4b6a-8026-1874d87c1b96" />

<img width="956" height="1599" alt="WhatsApp Image 2026-08-25 at 9 29 23 AM" src="https://github.com/user-attachments/assets/e9e81f51-9ff4-48a4-86b3-c1d066c2eecf" />



### SAMPLE OUTPUT:

<img width="753" height="657" alt="WhatsApp Image 2026-08-25 at 9 33 11 AM" src="https://github.com/user-attachments/assets/189f1ee9-6e90-43d0-afe5-00bb540bb030" />




## RESULT:
Thus, the linear convolution of the two given sequences were performed and its result was verified.

<img width="1600" height="1412" alt="WhatsApp Image 2026-08-25 at 9 28 34 AM" src="https://github.com/user-attachments/assets/cbebd795-0d9c-4b6a-8026-1874d87c1b96" />


## RESULT:
Thus, the linear convolution of the two given sequences were performed and its 

## RESULT:
Thus, the linear convolution of the two given sequences were performed and its 

## RESULT:
Thus, the linear convolution of the two given sequences were performed and its 
.
.
.
.
.
.
## RESULT:
Thus, the linear convolution of the two given sequences were performed and its 

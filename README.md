# SIMULATION-OF-MEAN-AND-VARIANCE-USING-SCILAB
# AIM:
To write a program for mean, variance and cross correlation in SCILAB and verify the output.

# EQUIPMENTS Needed

•	Computer with i3 Processor

•	SCI LAB

# Algorithm
1.	Define	the	Function:	Specify the	function	you	want	to	simulate.	For	example, f(x)=sin⁡(x)f(x) = \sin(x)f(x)=sin(x) or any other function.
2.	Generate Sample Points: Decide on the range and the number of sample points. Generate these sample points within the desired range.
3.	Evaluate the Function: Compute the function values at each of these sample points.
4.	Compute Mean, Variance and Cross Correlation: Use Scilab's functions to calculate the mean and variance of the computed function values.
5.	Display Results: Output the computed mean variance and Cross Correlation PROCEDURE
•	Refer Algorithms and write code for the experiment.
•	Open SCILAB in System
•	Type your code in New Editor
•	Save the file
•	Execute the code
•	If any Error, correct it in code and execute again
•	Verify the generated results


# PROGRAM
```
clear;
clc;
clear;
function X=f(x);
    z=4*(1-x)^2;
    X=x*z;
endfunction
a=0;
b=1;
EX=intg(a,b,f);
function Y=c(y);
    z=4*(1-y)^2;
    Y=y*z;
endfunction
EY=intg(a,b,c);
disp(EX,"Mean of X =")
disp(EY,"Mean of Y =")
function X=g(x);
    z=4*(1-x)^2;
    X=x^2*z;
endfunction
a=0;
b=1;
EX2=intg(a,b,g);
function Y=h(y);
    z=4*(1-y)^2;
    Y=y^2*z;
endfunction
EY2=intg(a,b,h);
vX2=EX2-(EX)^2;
vY2=EY2-(EY)^2;
disp(vX2,"Variance of X");
disp(vY2,"Variance of Y");

x= [1,3,5,7,8,6,4,2]; 
y= [2,4,6,8,7,5,3,1];
n1=max(size(y))-1;
n2=max(size(x))-1;
r=corr(x,y,n1);
plot2d3('gnn',r);

```

# TABULATION:

<img width="825" height="1280" alt="image" src="https://github.com/user-attachments/assets/973cf3bc-8c11-43ad-b584-674ee5071ccc" />



# CALCULATION:

<img width="1600" height="1509" alt="image" src="https://github.com/user-attachments/assets/943becde-08c4-40d3-a2d0-2d23b227191c" />
<img width="724" height="1280" alt="image" src="https://github.com/user-attachments/assets/840f5664-29b6-4f0d-ae25-acdff77e38a1" />
<img width="969" height="1280" alt="image" src="https://github.com/user-attachments/assets/9285b97e-639f-4d42-943c-f16ec4122158" />



# CONSOLE WINDOW:

<img width="364" height="177" alt="Screenshot 2026-06-01 134743" src="https://github.com/user-attachments/assets/a53ca9bd-08bf-46d3-92e8-85ea84892cbe" />

# OUTPUT WAVEFORM:

<img width="1600" height="871" alt="image" src="https://github.com/user-attachments/assets/65983f79-71f3-4a70-8cd7-a2821d8b99a4" />

 


# RESULT:
Thus the mean , variance and cross correlation are executed in Scilab and output is verified.

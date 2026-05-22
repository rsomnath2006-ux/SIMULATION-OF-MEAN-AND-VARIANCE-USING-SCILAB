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
function X=f(x)
    z=2*(2-x)^2
    X=x*z
endfunction
a=0;
b=1;
EX=intg(a,b,f);
function Y=c(y)
    z=2*(2-y)^2
    Y=y*z
endfunction
EY=intg(a,b,c);
disp(EX,"i)Mean of X=")
disp(EY,"Mean of Y=")

function X=g(x)
    z=2*(2-x)^2
    X=x^2*z
endfunction
a=0;
b=1;
EX2=intg(a,b,g);
function Y=h(y)
    z=2*(2-y)^2
    Y=y^2*z
endfunction
EY2=intg(a,b,h);
vX2=EX2-(EX)^2;
vY2=EY2-(EY)^2;
disp(vX2,"ii) Variance of X");
disp(vY2,"Variance of Y");

x=[1 3 4 6 7 9 2 8];
y=[2 5 8 4 6 1 3 7];
n1=max(size(y))-1;
n2=max(size(x))-1;
r=corr(x,y,n1);
plot2d3('gnn',r);
```
# TABULATION:
<img width="1204" height="1600" alt="WhatsApp Image 2026-05-22 at 2 05 48 PM" src="https://github.com/user-attachments/assets/c8147ae8-5421-4e4d-8d10-702aa8dc85fe" />

# CALCULATION:
<img width="1536" height="1587" alt="mean" src="https://github.com/user-attachments/assets/c91d65fb-f12f-4bac-93bb-1fcc7fd19e79" />
<img width="1204" height="1600" alt="variance" src="https://github.com/user-attachments/assets/01662bcc-85db-47e2-8e04-b5653fff8356" />


# CONSOLE WINDOW:

<img width="383" height="388" alt="Mean and variance con" src="https://github.com/user-attachments/assets/55651085-f773-461d-bd76-837ae5977ced" />

# OUTPUT WAVEFORM:

<img width="761" height="737" alt="Mean and variance graph" src="https://github.com/user-attachments/assets/d7f0ab59-93ce-4b11-bcc6-2106876585e6" />
 


# RESULT:
Thus the mean , variance and cross correlation are executed in Scilab and output is verified.

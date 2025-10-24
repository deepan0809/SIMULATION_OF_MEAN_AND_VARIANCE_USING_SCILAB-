# SIMULATION_OF_MEAN_AND_VARIANCE_USING_SCILAB

AIM:

To write a program for mean, variance and cross correlation in SCILAB and verify the output. 

EQUIPMENTS Needed 

• Computer with i3 Processor 


• SCI LAB 


Algorithm 
1. Define the Function: Specify the function you want to simulate. For example, 
f(x)=sin⁡(x)f(x) = \sin(x)f(x)=sin(x) or any other function. 
2. Generate Sample Points: Decide on the range and the number of sample points. Generate 
these sample points within the desired range. 
3. Evaluate the Function: Compute the function values at each of these sample points. 
4. Compute Mean, Variance and Cross Correlation: Use Scilab's functions to calculate the 
mean and variance of the computed function values. 
5. Display Results: Output the computed mean variance and Cross Correlation 

PROCEDURE 
• Refer Algorithms and write code for the experiment. 
• Open SCILAB in System 
• Type your code in New Editor 
• Save the file 
• Execute the code 
• If any Error, correct it in code and execute again 
• Verify the generated results

PROGRAM
```
function X=f(x),
    z=6*(1+x)^2,
    X=x*z
endfunction
a=0;
b=1;
EX=intg(a,b,f)
function Y=c(y),
    z=6*(1+y)^2,
    Y=y*z
endfunction
EY=intg(a,b,c);
disp("Mean of X =",EX)
disp("Mean of Y =",EY)
function X=g(x),
    z=6*(1+x)^2,
    X=x^2*z
endfunction
a=0;
b=1;
EX2=intg(a,b,g);
function Y=h(y)
    z=6*(1+y)^2,
    Y=y^2*z
endfunction
EY2=intg(a,b,h);
vX2=EX2-(EX)^2;
vY2=EY2-(EY)^2;
disp("Variance of X",vX2);
disp("Variance of Y",vY2);
x=input("type in the reference sequence=");
y=input("type in the second sequence=");
n1=max(size(y))-1;
n2=max(size(x))-1;
r=corr(x,y,n1);
plot2d3('gnn',r);   
```

OUTPUT
<img width="1506" height="932" alt="image" src="https://github.com/user-attachments/assets/6b5fc2ad-0a5d-4d85-89a6-4a5a4a020ab9" />

 
TABULATION
<img width="802" height="1040" alt="image" src="https://github.com/user-attachments/assets/e5991df5-8a2b-465b-9131-59fee596600d" />



RESULT: 
Thus the mean , variance and cross correlation are executed in Scilab and output is verified. 


java cTHE HONG KONG POLYTECHNIC UNIVERSITY 
 
ENG2002 Computer Programming Homework 
 
A. Instructions 
 
1. At the beginning of each Python file, add a comment to show your student ID and name. 
2. This assignment comprises 3 parts. You may use a new file for each part or a single Jupyter Notebook file. 
3. Your programs need to be well commented. You may refer to your course notes (ch4.pdf) on how comments are 
made. Lacking comments will result in down-grading of your submission. 
4. Your programs need to have a good structure. Never write the whole program in a single function. You should 
write supporting functions. 
5. Do NOT share your source program with your classmates. Plagiarism will make you and your friends all get zero 
mark. 
6. The deadline of submission is 13 October 2024 and you need to submit your file to Teams as an attachment. 
B. The Programming Task 
 
Background 
 
A simple resistor–capacitor (RC) circuit is an electric circuit composed of one resistor and one capacitor as shown below: 
The capacitor C could be charged to V0 and then be discharged by the resistor R. The formula for exponential decay of 
resistor voltage is given by: 
 
 !( ) =  "	 # !
"# (1) 
 
where V0 is the capacitor voltage at time t = 0. The time required for the voltage to fall to 36.8% of the initial value is 
called the time constant ( ) and is given by: 
 
  =    (2) 
 
 
Q1. Create a new file in Jupyter Notebook with the name "part1". On starting, the application should call a function 
userMenu() that shows the following main menu: 
 
[a] Find time constant 
[b] Find discharge voltage 
[c] Find discharge time 
[d] Find best curve from experimental data 
[x] Exit 
 
Key in your choice (a, b, c, d or x to exit): • The user is expected to enter a character of 'a', 'b', 'c', 'd' or 'x' only. When any other character is entered, 
userMenu() will display "Wrong input, enter again!" and the above main menu is shown again. For 
this part, if the user enters 'b' or 'c' or 'd', the above menu will be shown again and your program does not need 
to do anything. 
 
• If the user enters 'a', userMenu() will display "Please enter resistance (R): ". The user should input 
a value of type float. It is assumed that the user always enters a positive float value for R and your program 
does not need to check this. Then, userMenu() will display "Please enter capacitance (C): ". The 
user should input a positive value for C. If the user enters 0 or a negative value, userMenu() will prompt the 
user for re-entering until a positive value has been entered (you may assume that the user always enters a value 
of type float for this and your program does NOT need to check this.) Then, the function timeConst() is 
called, which uses the user-input values of R and C as input parameter values, and returns the value of the time 
constant, which is of type float. Note that this returned value should be printed by userMenu() and the 
function timeConst() must NOT print anything on screen. 
 
• If the user enters 'x', userMenu() will print "Goodbye!" on the screen. The whole program then ends (without 
showing the main menu.) 
 
• The following Python code MUST be used. 
 
 
#your Name 
#student number 
 
from math import exp, log #use math functions in part 2 
 
#Implement the required functions below: 
 
#def timeConst(R, C) #Find time constant of a simple RC circuit 
#def userMenu() #shows the user menu and process user input 
 
userMenu() #call function to display user menu and process user input 
 
 
• The sample outputs given below should be realised by your 代 写ENG2002、Python
代做程序编程语言program on executing it inside Jupyter Notebook. 
Notice that the character(s) following a ‘:’ is/are entered by the user. 
 -------------------------------------- PASS line ---------------------------------- Q2. Create a NEW file with the name "part2". Copy the content of the source file in Q1 to this file. Modify the 
program developed for Q1 to perform the following tasks: 
 
• Rewrite the function userMenu()such that if the user enters 'b', it will display "Enter initial voltage 
(V0): " on the screen. The user should input a positive value of type float and you should create a function 
input_p()to handle this. Then, userMenu()will display "Enter resistance (R): " on the screen. The 
user should input a positive value of type float and the function input_p() should be used. Afterward, 
userMenu()will display "Enter capacitance (C): " on the screen. The user should input a positive value 
of type float and the function input_p() should also be called. Then, userMenu()should call a function 
disVoltage() which uses the values of V0, R, C as input parameters. disVoltage()will display "Enter 
discharge time (t): " on the screen. The user should input a positive value of type float and the function 
input_p()should be used. disVoltage()will then display the discharge voltage using equation (1). You may 
use exp()function in the math module. The function disVoltage() should have no returned value. 
 
• Rewrite the function userMenu()such that if the user enters 'c', it will display "Enter initial voltage 
(V0): " on the screen. The user should input a positive value of type float and the function input_p() 
should be used. Then, userMenu()will print "Enter resistance (R): " on the screen. The user should 
input a positive value of type float and the function input_p() should be used. Afterward, userMenu()will 
display "Enter capacitance (C): " on the screen. The user should input a positive value of type float 
and the function input_p() should also be called. Then, userMenu()should call a function disTime() which 
uses the values of V0, R, C as input parameters. disTime()will display "Enter discharge voltage (Vr): 
" on the screen. The user should input a positive value of type float and the function input_p()should be 
used. disTime()will then display the discharge time by solving equation (1). You may use log()function in 
the math module. The function disTime() should have no returned value. 
 
• The sample outputs given below should be realised by your program on executing it inside Jupyter Notebook. 
Notice that the character(s) following a ‘:’ is/are entered by the user. 
 
 ---------------------------------- CREDIT line ------------------------------------ 
 
Q3. Create a NEW file with the name "part3". Copy the content of the source file in Q2 to this file. Modify the 
program developed for Q2 to perform the following tasks: 
 
• Rewrite the function userMenu()such that if the user enters 'd', it will call the function bestCurve() and then 
the function will call input_p() to get the input data from the user. It will display the result on the screen 
inside the function. Get back to the main menu after the result is shown. 
 • To find the best curve, you need to transform equation (1) into straight line, y = m x + b and then use the following 
formulae to find the best straight line: 
 
where 
 
• The sample outputs given below should be realised by your program on executing it inside Jupyter Notebook. 
Notice that the character(s) following ‘:’ is/are entered by the user. 
 
---------------------------------- DISTINCTION line ------------------------------- 

         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com

This is the code for a simple line following bot designed with the following features:

    ⦿ Differential drive 
    ⦿ Dual H-Bridge
    ⦿ Three IR sensors 

As I progressed through this task, I refined my logic and consequentially my code (which was executed on Arduino IDE). Below is the final logic of the line-following bot presented in the form of a tabular column for easy understanding.

![image](https://github.com/sne-1807/line-following-bot-records/assets/124518945/c29e4083-7243-4c58-9b9f-4b687b9947bf)

Each IR sensor returns a boolean value, 1 if the line is detected and 0 if not. Based on the combination of boolean ouput, the bot follows a differnt control logic, but in all cases, the bot needs to perform some specific repeated motion until it reaches the condition 010 where the bot is smack-dab on the line and it can move forward. 

As the boolean sequential combination of sensor output is equivalent to a binary number in a loose sense, I converted the binary number to the corresponding decimal number to run it smoothly through switch cases.

In this repository, I have documented the evolution of my code, and will keep adding to it as I learn new things
while I build the final line following bot using hardware components.

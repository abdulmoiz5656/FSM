# Finite State Machine
## FSM
A simple working of fsm below.\
The fsm model is also attached below.\
"0" indicates "no" and "1" indicates "yes" according to fsm model.\
As the machine will be in idle state from starting, as the machine recives the command of "0" it will remain at the it's idle state but as the machine recives the command "1" the machine will move to the next stage, and from there the machine can go one way from two ways depends on what command is recived by the machine , if the input is "0" the machine will go to failed state but if the input is "1" the machine will move to success state which is the accepting state, and after being on falied or success state if machine recive any command it will move back to idle state.
!["FSM"](images/fsm.jpg)
## Truth table
Below is the truth table for the fsm\
!["Truth table"](images/table 1.jpg)
## K Map
Below is the K Map for the fsm model.\
!["K Map"](images/K Map.jpg)
## Boolen Equation
the boolen equation showed by the images below\
!["state 0](images/state 1.jpg)
!["state 1](images/state 2.jpg)
the drived equation in combined form\
$$S_0 = S_0'S_1$$
$$S_1 = S_0'I_0$$
$$O_0 = S_0'S_1I_0$$
## code 
To run this code properly you have to be sure that terminal space is larger.\
```
make run
./main.o
```
## Machine 
As the first state of machine is an idle state as below:\
!["idle state"](images/m 1.jpg)

Now if the input is:\
"0" the machine remains at idle state\
"1" the machine moves to next step.\

As the next step is confirming step as below:\
!["Confirming state"](images/m 2.jpg)

So now from here if the input is:\
"0" the machine moves to the fail state\
"1" the machine moves to sucess state\

As if the input is zero the machine moves to fail state which is shown as\
!["failed State"](images/m 4.jpg)

so from fail state if the machine recives an input "0" or "1" it will moves back to idle state.\

As if the input is "1" the machine moves to sucess state as shown\
!["sucess State"](images/m 3.jpg)

From here wheather the input is "0" or "1" the machine moves to idle state back.\
So from failed state or from sucess state the machine moves back to the idle state.

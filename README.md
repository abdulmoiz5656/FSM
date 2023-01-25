Finite State Machine
In here, we will see how the FSM works in the Vending machine.
The FSM image can be found here:
Let say "0" indicates "No" and "1" indicates "Yes"
When the machine starts, the first state will be in the IDLE state. 
If the user put "0" in the idle state, the machine will stay in idle state until the user puts "1" which will move to the next state. 
The next state is the CONFIRM state, the CONFIRM state has two ways to go if it is inputted. First, by inputting 0 in that state, it will go to the "FAILED" state which is not an accepting state. However, 
if it is inputted "1", it will go to the "SUCCESS" state or the accepting state. Lastly, in the "FAILED" and "SUCCESS" state, 
if the user input any input values to the machine, it will go back to the IDLE state.


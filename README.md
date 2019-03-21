# Slot Machine in Python

This program has been awarded an A+ with 100% score.

View and run the program online without Anaconda: 

Slotmachine:
https://colab.research.google.com/drive/1zRoXm9VT3zyb-YT3KcetboPVmSKUwKGM

## About the Slot Machine

A simple command line version of a slot machine is created. The slot machine consists of three columns that display one of three fruits: 🍎🍐🍊. When the slot machine begins, the player is asked to place a bet from their initial credit (which is 10 by default).  

For each play of the slot machine there are three possible outcomes:
1. Full house – all 3 columns contain the same value. Player wins an amount equal to the bet and this is added to their credit.
2. Half house – 2 of the 3 columns contain the same value. Player wins half the amount bet.
3. Empty house - all 3 columns contain different values. Player loses bet.

An emoji package is used for this game. To install please use: pip install emoji --upgrade 

### Structure
As by requirement, 3 classes with methods and 1 function have been created: 

**1. Purse**: It has a balance that is initialized to 10. Purse manages the players credit, whit 3 methods: 
1. get_balance
2. debit
3. credit

**2. Column**: Supplies the face of each column with fruits. It has 1 method that changes the fruit randomly when the pull_handle method on Slot is invoked: 
1. change_face

**3. Slot**: Each Slot has three Columns representing 3 fruits. Slot has 4 methods: 
1. pull_handle
2. take_bet
3. show_slot
4. score_slot

**One funtion to run the machine: run_slot_machine**

As per requirement this function validates the input (integer number between 2 and the available credit) and runs the game. When the slot machine begins, the player is asked to place a bet from their initial credit (defaults to 10).  
When the user types 'N', the game stops.
It is chosen to use exception handling here.

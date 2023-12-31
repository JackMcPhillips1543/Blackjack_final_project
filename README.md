# Java Swing Blackjack Game

## Overview

This project is a fully functional Blackjack game written in Java, following the Model-View-Controller (MVC) design principle. It was developed as the final project for CSCI 2300 (Object-Oriented Programming) in collaboration with Adem Durakovic and Amar Hadzic.

## Getting Started

To run the game, make sure you have the Java JDK installed. If not, you can install it from [here](https://docs.oracle.com/en/java/javase/20/install/overview-jdk-installation.html#GUID-8677A77F-231A-40F7-98B9-1FD0B48C346A)

Clone this repository into the directory of your choice, and then use the terminal to navigate to the project directory.

The source code can be found in the `/app/src/main/java/blackjack directory`.

## Features

### Model
The model folder contains the essential components of the game, including:

**Player Model:**
The player model encapsulates the logic used by the player throughout the game. It maintains the player's current hand, balance, and debt. Additionally, this model allows users to save and resume games, as it is serializable.

**Gustavo the Loan Shark Model:**
Gustavo's model tracks the player's debt and includes functions that allow borrowing money and paying off debt.

**Dealer Model:**
The dealer model manages the dealer's hand and follows the specific rules that dealers must adhere to in Blackjack games.

**Table Model:**
The table model simulates the real-world table, holding both the player and the dealer models. It decides the winner of each round of betting and resets for the next round.

### View
The View folder contains the Graphical User Interface (GUI) components of the game, primarily managed by the `BlackJackGui class`. The GUI includes buttons and icons necessary for user interaction.

Key design principles employed in the GUI development:

**Encapsulation:** The GUI components, such as player buttons and chips, are designed to be easily modifiable for future updates and modifications.

**Inheritance:** Inheritance is utilized for the player and chip buttons, allowing them to retain the features of the JButton class while modifying their functionality and appearance.

**Observer Pattern:** The GUI and the Model are connected using the observer pattern. The GUI observes the model and updates accordingly when there are changes in the game state.

### Controller
The controller handles the interaction between the user and the game. It includes methods for:

 * Placing Bets
 * Paying off the "loan shark" (Gustavo)
 * Hitting, Standing, Splitting
To ensure flexibility and ease of future modifications, the controller follows the controller interface pattern.


## How to Play
1. Once you have Java JDK installed and are in the project directory use the ``` gradle run ``` command to start the game.
2. Place your bets to start the round.
3. Follow the on-screen buttons to make decisions during the game (Hit, Stand, Split, etc.).
4. The dealer will follow the Blackjack rules, and the winner will be determined at the end of each round.
   
If you're unfamiliar with the rules of blackjack, you can check them out [here](https://bicyclecards.com/how-to-play/blackjack/).

Enjoy playing Blackjack! Good luck!
   


# Java Swing Blackjack Game

## A fully functional Blackjack game written in Java using the Model-View-Controller principle to create a game

###This Project was created for CSCI 2300 (Object Oriented Programming) and made in collaboration with Adem Durakovic and Amar Hadzic


This project was assigned as a final project meant to show our knowledge of the design principles we had learned over the semester. Gradle is used to run the app. To navigate to the source code follow the path /app/src/main/java/blackjack

##Model
The model folder holds the model representation of Gustavo the Loan Shark, the player, the dealer, and the board.

##View
The View folder contains all of the GUI components. The BlackJackGui creates all of the buttons and icons that will appear on the screen for the user as well as the logic for each button when it is clicked. 
 
  - We used the encapsulation design principle to make the different player buttons and chips easily modifiable for future modification.

  - Our group employed the inheritance software design principle with the player and chip buttons, to keep the features of the JButton class but modify the functionality and appearance

  - The GUI and the Model use the observer pattern. The GUI observes the model and updates when the state of the model changes.

##Controller
The controller contains all of the methods that the player will use. These consist of:
  - Placing Bets
  - Paying off the "loan shark"
  - Hitting, Standing, Splitting

The controller uses a controller interface.

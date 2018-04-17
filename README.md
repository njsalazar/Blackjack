# Blackjack
Blackjack game in Python

Two identical files, one a .ipynb Juypter Notebook, one a .py Python file.  Either one works to play the game.



To play a hand of Blackjack the following steps must be followed:

1. Create a deck of 52 cards
2. Shuffle the deck
3. Ask the Player for their bet
4. Make sure that the Player's bet does not exceed their available chips
5. Deal two cards to the Dealer and two cards to the Player
6. Show only one of the Dealer's cards, the other remains hidden
7. Show both of the Player's cards
8. Ask the Player if they wish to Hit, and take another card
9. If the Player's hand doesn't Bust (go over 21), ask if they'd like to Hit again.
10. If a Player Stands, play the Dealer's hand. The dealer will always Hit until the Dealer's value meets or exceeds 17
11. Determine the winner and adjust the Player's chips accordingly
12. Ask the Player if they'd like to play again

First, the suits, ranks, and values are defined.  
Then, a Card class is created with suit and rank attributes.  
Next, a Deck class is created with all the cards generated and shuffle and deal methods created.
Then, a Hand class is created to hold cards and calculate the value of those cards. A method is created to adjust the value of an Ace to be either 1 or 11.
Last, a Chips class is created to keep track of a player's chips and bets.

Next, functions are defined.  A function is created to take bets in the form of an integer provided it is less than the amount of chips a player has.
A hit function is created to add cards to the hand.
Next, a function is defined to ask the player if they want to hit or stand. If they stand, the dealer's turn begins.
Two functions are needed to display the cards.  One to show the player's entire hand and one of the dealer's cards while keeping the other hidden, and one to show all cards in both hands.
Lastly, functions are created to handle all possible end of game situations: the player wins, the player busts, the dealer wins, the dealer busts, the player and dealer push.

Once the game is setup, the actual gameplay can begin.  First, the deck is created and shuffled and two cards are dealt to each player. The player's "bank" of chips is set up and the player is asked how many chips they would like to bet.  The player's hand is revealed and one of the dealer's cards is shown.  The player is asked to hit or stand, and after each hit, the player's hand is shown.  If they player goes over 21, they bust.  If the player stands without busting, the dealer plays.  The dealer's other card is revealed and they begin hitting until they either bust or go over 17 at which point they stand.  When the dealer stands, their hand is compared to the player's to determine who wins.  The player's chip total is printed and the player is asked to play again.  If they want to play again, the game starts over.

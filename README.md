# Python-blackjack

############### Blackjack Project #####################

Requirements:

Deal both user and computer a starting hand of 2 random card values.  
Detect when computer or user has a blackjack. (Ace + 10 value card).  
If computer gets blackjack, then the user loses (even if the user also has a blackjack). If the user gets a blackjack, then they win (unless the computer also has a blackjack).  
Calculate the user's and computer's scores based on their card values.  
If an ace is drawn, count it as 11. But if the total goes over 21, count the ace as 1 instead.  
Reveal computer's first card to the user.  
Game ends immediately when user score goes over 21 or if the user or computer gets a blackjack.  
Ask the user if they want to get another card.  
Once the user is done and no longer wants to draw any more cards, let the computer play. The computer should keep drawing cards unless their score goes over 16.  
Compare user and computer scores and see if it's a win, loss, or draw.  
Print out the player's and computer's final hand and their scores at the end of the game.  
After the game ends, ask the user if they'd like to play again. Clear the console for a fresh start.  

############### Our Blackjack House Rules #####################

The deck is unlimited in size.  
There are no jokers.  
The Jack/Queen/King all count as 10.  
The the Ace can count as 11 or 1.  
Use the following list as the deck of cards:  
  cards = [11, 2, 3, 4, 5, 6, 7, 8, 9, 10, 10, 10, 10]  
The cards in the list have equal probability of being drawn.  
Cards are not removed from the deck as they are drawn.  

##################### Steps #####################

Step 1: Blackjack game built as per logic gathered from website: 
   https://games.washingtonpost.com/games/blackjack/


Step 2: Build breakdown of program requirements: 
   Requirements as listed at top of this page

Step 3: Download and read this flow chart I've created: 
![Blackjack_Flowchart](https://user-images.githubusercontent.com/9038980/210604957-7e1d93db-1be0-4185-afdd-67751f06a4d4.PNG)

Step 4: Create a deal_card() function that uses the List below to *return* a random card.

Fixed bugs:
1. When score goes over 21 and and there's an Ace in the cards, replace 1 in the same position where the Ace was.
2. If dealer/computer gets a blackjack, then the dealer wins even if the Player has a blackjack as well






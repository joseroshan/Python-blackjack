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

Step 3: Build flow chart: 
![Blackjack_Flowchart](https://user-images.githubusercontent.com/9038980/210604957-7e1d93db-1be0-4185-afdd-67751f06a4d4.PNG)

Step 4: Create a deal_card() function that uses the List below to *return* a random card.  

Step 5: Deal the user and computer 2 cards each using deal_card()

Step 6: Create a function called calculate_score() that takes a List of cards as input and returns the score.  

Step 7: Inside calculate_score() check for a blackjack (a hand with only 2 cards: ace + 10) and return 0 instead of the actual score. 0 will represent a blackjack in our game.  

Step 8: Inside calculate_score() check for an 11 (ace). If the score is already over 21, remove the 11 and replace it with a 1.  

Step 9: Call calculate_score(). If the computer or the user has a blackjack (0) or if the user's score is over 21, then the game ends.  

Step 10: If the game has not ended, ask the user if they want to draw another card. If yes, then use the deal_card() function to add another card to the user_cards List. If no, then the game has ended.

Step 11: The score will need to be rechecked with every new card drawn and the checks in Step 9 need to be repeated until the game ends.  

Step 12: Once the user is done, it's time to let the computer play. The computer should keep drawing cards as long as it has a score less than 17.

Step 13: Create a function called compare() and pass in the user_score and computer_score. If the computer and user both have the same score, then it's a draw. If the computer has a blackjack (0), then the user loses. If the user has a blackjack (0), then the user wins. If the user_score is over 21, then the user loses. If the computer_score is over 21, then the computer loses. If none of the above, then the player with the highest score wins.

Step 13: Create a function called compare() and pass in the user_score and computer_score. If the computer and user both have the same score, then it's a draw. If the computer has a blackjack (0), then the user loses. If the user has a blackjack (0), then the user wins. If the user_score is over 21, then the user loses. If the computer_score is over 21, then the computer loses. If none of the above, then the player with the highest score wins.  

Step 14: Ask the user if they want to restart the game. If they answer yes, clear the console and start a new game of blackjack and show the logo from art.py.

Fixed bugs:
1. When score goes over 21 and and there's an Ace in the cards, replace 1 in the same position where the Ace was.
2. If dealer/computer gets a blackjack, then the dealer wins even if the Player has a blackjack as well
3. If Player and the dealer are both over, Player loses.  


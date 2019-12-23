# blackjack
Basic blackjack to practice unit testing.

You might need to right click on the pom.xml and select the add maven to get it to build right in intellij.

# Goal
The goal is to be able to write the blackjack game such that when you run the application for the first time you have a 
very reasonable expectation that it will work perfectly.

# Approach
You can take a TDD (Test Driven Development approach. Generally means that you write the unit tests first and then write the code.
or in other words the tests drive the development of the code).

You can also write the code first and then fill in with tests afterwards. 
I tend to write a hybrid of both.

Another things you can do is to just start writing code. This will get you thinking about the task.  You can then delete
it and start again or start refactoring the method into several objects and methods.
 
# Hints and Recommendations
Wrap calls to the System or other code you have no control over.  For instance, wrap the console input in your own object
so you can mock the console. This will allow you to control the input for testing.

Attempt to use the SOLID principles: https://www.baeldung.com/solid-principles

Use //todo comments liberally as needed. If you use an IDE like intellij, the IDE can keep track of todo comments so you
can remember to go back to them.
 
# Rules of Blackjack

The goal of the game is to have a hand that is higher than the dealers hand but not go higher than 21 points.

Each card is assigned a point value. (Two is worth 2, three is 3, etc.  Jack, queen, king is worth ten.  Ace can either be 1 or 11)

A player is given 2 cards. One face up and one face down.  The player is allowed to look at both of their cards but may not
view other player's face down card. Each player is playing against the Dealer who is a sort of automated player.

The player then must decide if they want to receive another card ("hit") to add to their hand total or to not receive another car
("stay"). You are allowed to hit as many time as you want until you either stay or go over 21 points ("Go Bust").  If you 
go bust, then you will have lost before the dealer's turn.

Once all the players have finished, then it's the dealer's turn.  The dealer will always hit until their score is 17 or higher.
Which, at this point, they will either stay or have gone bust.

If the dealer has gone bust, then all the remain players that have not gone bust will have won.  If dealer hasn't got bust,
then the player or dealer with the highest point wins.  Ties are ties.


 


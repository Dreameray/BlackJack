# BlackJack Game

A simple Java implementation of the classic card game BlackJack (also known as 21) with a graphical user interface.

## Overview

The game follows standard BlackJack rules where the goal is to beat the dealer by getting a hand value as close to 21 as possible without exceeding it.

## Features

- Complete BlackJack gameplay with hit and stand options
- Visual card representation with proper card graphics
- Automatic calculation of hand values
- Special handling for Aces (can be valued at 1 or 11)
- Dealer AI that follows standard casino rules (hits until 17)
- Game result display (win/lose/tie)

## How to Play

1. Run the application to start a new game
2. You and the dealer are each dealt two cards (one of the dealer's cards remains hidden)
3. Choose to "Hit" to draw another card or "Stay" to keep your current hand
4. If you exceed 21 points, you lose automatically (bust)
5. Once you stand, the dealer reveals their hidden card and draws until reaching at least 17 points
6. The winner is determined by comparing hand values (highest hand under 21 wins)

## Game Rules

- Number cards (2-10) are worth their face value
- Face cards (Jack, Queen, King) are worth 10 points
- Aces are worth 11 points, but switch to 1 point if the hand would otherwise bust
- The dealer must hit until they have at least 17 points
- If the player exceeds 21 points, they lose regardless of the dealer's hand
- If the dealer exceeds 21 points, the player wins
- If neither busts, the higher hand value wins

## Technical Implementation

The game is built using Java with Swing for the graphical user interface. It features:

- Object-oriented design with a Card class to represent playing cards
- Dynamic rendering of card graphics
- Event-driven gameplay using action listeners
- Proper management of game state and logic

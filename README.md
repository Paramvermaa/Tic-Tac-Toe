# Tic-Tac-Toe
Built an unbeatable version of Tic-Tac-Toe; implemented minimax algorithm using javascript to predict best moves for
varying difficulty levels along with the reverse implementation of the game, for web-based application having winning chance of 95%

![image](https://github.com/Paramvermaa/Tic-Tac-Toe/assets/112919138/51469fa7-e5f2-4432-86dd-a1058d00c22d)
Mini-max algorithm is a recursive or backtracking algorithm which is used in decision-making and game theory. It provides an optimal move for the player assuming that opponent is also playing optimally.
**Pseudo-code for MinMax Algorithm:**
function minimax(node, depth, maximizingPlayer) is  
if depth ==0 or node is a terminal node then  
return static evaluation of node  
  
if MaximizingPlayer then      // for Maximizer Player  
maxEva= -infinity            
 for each child of node do  
 eva= minimax(child, depth-1, false)  
maxEva= max(maxEva,eva)        //gives Maximum of the values  
return maxEva  
  
else                         // for Minimizer player  
 minEva= +infinity   
 for each child of node do  
 eva= minimax(child, depth-1, true)  
 minEva= min(minEva, eva)         //gives minimum of the values  
 return minEva  
Working of Min-Max Algorithm:
The working of the minimax algorithm can be easily described using an example. Below we have taken an example of game-tree which is representing the two-player game.
In this example, there are two players one is called Maximizer and other is called Minimizer.
Maximizer will try to get the Maximum possible score, and Minimizer will try to get the minimum possible score.
This algorithm applies DFS, so in this game-tree, we have to go all the way through the leaves to reach the terminal nodes.
At the terminal node, the terminal values are given so we will compare those value and backtrack the tree until the initial state occurs.

![image](https://github.com/Paramvermaa/Tic-Tac-Toe/assets/112919138/0bfaa331-1a89-4584-bfa9-f7b7fb50a4b6)

Tech Stack Used: Html, Javascript, Vanilla CSS

***Souce:https://www.javatpoint.com/mini-max-algorithm-in-ai***

#Prime Game

Maria and Ben are playing a game. Given a set of consecutive integers starting from 1 up to and including n, they take turns choosing a prime number from the set and removing that number and its multiples from the set. The player that cannot make a move loses the game.

They play x rounds of the game, where n may be different for each round. Assuming Maria always goes first and both players play optimally, determine who the winner of each game is.

<ul>
<li>Prototype:<code>def isWinner(x, nums)</code></li>
<li>where x is the number of rounds and nums is an array of n</li>
<li>Return: name of the player that won the most rounds</li>
<li>If the winner cannot be determined, return None</li>
<li>You can assume n and x will not be larger than 10000</li>
<li>You cannot import any packages in this task</li>
</ul>
Example:

<code>x = 3, nums = [4, 5, 1]</code>
##<b>First round: 4

<ul>
<li>Maria picks 2 and removes 2, 4, leaving 1, 3</li>
<li>Ben picks 3 and removes 3, leaving 1</li>
<li>Ben wins because there are no prime numbers left for Maria to choose</li>
</ul>

##<b>Second round: 5</b>

<ul>
<li>Maria picks 2 and removes 2, 4, leaving 1, 3, 5</li>
<li>Ben picks 3 and removes 3, leaving 1, 5</li>
<li>Maria picks 5 and removes 5, leaving 1</li>
<li>Maria wins because there are no prime numbers left for Ben to choose</li>
</ul>

##<b>Third round: 1</b>

Ben wins because there are no prime numbers for Maria to choose
<b>Result: Ben has the most wins

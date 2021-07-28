## Realistic addition: the effect of starting money

![](GoldenDollar.png){:.inline}{: style="width:20%"}

In an official game of Monopoly you receive 1500 euros of money at the start and you earn 200 euros each time you pass or land on START. Such a finite amount of money has an effect on the speed with which you can buy streets. In this assignment we'll find out exactly what that effect is.

**Note:** We're going to make an adjustment to your existing code from the previous part of the assignment; an expansion. You don't need to create a new file and at the end of the assignment you can just hand in the code from `monopoly.py`. It will contain both "Moving around" and "Starting money".

For your new program you'll have to edit the function `simulate_monopoly()`, in such a way that each game starts with a specified number of starting money and that you keep track of how much money the player has left after each purchase and lap. You'll also have to verify, each time you land on a property that is for sale, whether the player has enough money left to make the purchase. The expectation is that the game will take more turns, before all streets are in possession of the player, than in the first part of the assignment where money was not a factor.

For a **single** game the code looks like this:

    number_of_throws = simulate_monopoly(starting_money)

Here too, just like in "Moving around", we'll have to simulate a large number of games. Make sure the starting money of the player is supplied in the function call as input argument: `simulate_monopoly_games(total_games, starting_money)`. This function will pass that amount of `starting_money` to each individual simulation.

Start out with 3000 euros of starting money and lower that amount by 500 each time: 2500, 2000, 1500, 1000, 500, and 0 euro. Simulate for each choice of starting money 2500 different games to accurately calculate the average number of throws required to collect all streets. Finally create a graph of the average amount of throws on the vertical axis and the amount of starting money on the horizontal axis.

In the official game of Monopoly each player is assigned 1500 euros at the start. `Print` for that specific amount of starting money the number of throws that are required to buy all streets in the following way:

{: .language-python}
	Monopoly simulator: 1 player, 1500 euros starting money, 10000 games
    It took an average of XXX throws for the player to collect all streets

Use the difference between the average number of throws with 1000 euro or 2000 euros of starting money to get an idea of the effect (number of throws the game is shorter/longer) of having 100 euros more or less starting money each time.

**Tips:**

   1. You're allowed to manually change the number of starting money each time.

   2. You can test your code by providing the player with a huge amount of starting money. With a million euros you effectively create the same situation as you did for Donald Trump mode in "Moving around".

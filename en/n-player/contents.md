# Many players

One important aspect of good design is generality. Is you code very specific to the problem at hand? Or is it easy to extend to other use cases.

Create a file called `monopoly-nplayer.py` and copy the `simulate_monopoly(starting_money_p1, starting_money_p2)` function (and everything else that is needed to run it).

### Assignment

* The goal is change `simulate_monopoly(starting_money_p1, starting_money_p2)` in such a way that it works for any amount of players. 
* In stead of having the two input parameters, `starting_money_p1` and `starting_money_p2`, it should accept a single list with the amount of starting money for each player.
* You should be able to call the function like this:

        starting_money = [1500, 1600, 2000] # money for [player1, player2, player3]
        simulate_monopoly(starting_money)

* This should work for any length of `starting_money`, where the length of the list implies the number of players and the elements the respective amount of starting money for each players.
* If you had an excellent design in your previous solution, this assignment is going to be really eassy. Otherwise this might take a lot of redesign.
* Think about how to test it.
    * If you run it for exactly two players you should be able to reproduce the exact results of the previous assignment.
    * Can you think of other ways to verify your code is working correctly?
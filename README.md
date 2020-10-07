# football_with_linear_algrebra

Goal: Accurately predict an NFL playoff bracket given regular season data


Different strategies:

Try to find rankings of teams, such that for every game between teams i and j, the difference between team i's score and team j's score is equal to their difference in ranking

Create a matrix that is 32 by 32, such that every entry Aij is equal to the total number of points scored by team i against team j, with some normalization. Next, try to find some strength vector S such that, when multiplying A by S, we get another proportional vector. This becomes an equation where we can use eigenvalues and eigenvectors to find a solution



Conclusion:

In the end, the first of these two methods was the most accurate, but only after taking all nonzero terms in our matrix and making them small values like 1^(-15)

Able to predict superbowl winner as first or second best team for all three years tested on (2010, 2011, 2013)

Able to predict upsets, when higher seeded teams lost early on

pitfalls: did badly when there was too high of an upset, like the 16-0 patriots losing in the super bowl

NOTE: The actual full paper is also included in this repository, if you would like to view that as well

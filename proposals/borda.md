### Use Modified Borda Count for Preference Voting

**Author**
Anthony Shull

##### Problem

Voting methods are inherently flawed. They are easy to manipulate. Worse, they can lead to no result or a result that contradicts the actual wishes of the group without even being manipulated.

Let's say you have six candidates, five positions, and 30 voters. If all votes are distributed evenly, you could end up with all six candidates getting 25 votes. There is no way to force a run-off. You're stuck.

Now, imagine that one of the six candidates is Pythagoras. He and his group of four followers realize that they can increase the power of their votes simply by withholding votes. Normally, with 30 people and five positions you would have 150 total votes. But, the Pythagoreans decide that they will only vote for Pythagoras. Removing all of their votes from the pool for the time being, and again distributing votes evenly, each candidate gets 20 votes with a remainder of five.

We'll distribute those five to Pythagoras's opponents so that they each have 21 votes and he only has 20. But, when we then add in the five Pythagoreans' votes, he jumps to 25 votes and escapes a run-off. If they had used all of their votes, and they were distributed evenly, we would again have the situation where everyone would have 25 votes.

To give another example, let's say the votes are not evenly distributed. Thirty voters are electing three persons out of a pool of five candidates. The Pythagoreans haven't voted yet. So, the breakdown of votes is 19, 17, 16, 12, and 11 with Pythagoras in last place. If he and his four conspirators vote only for him, he moves from 11 to 16 votes and wins in the election. If, on the other hand, they have to use all of their votes, there is no way for him to avoid a run-off. 

##### Solution

We should use the [Modified Borda count][mbc] for all votes of preference--all votes that are not simply "yes" or "no" or between only two candidates.

Again, an illustration works best. Lets say you have *five* candidates and *three* positions. As a voter, you are asked to give *three* points to your top preference, *two* points to your second choice, *one* point to your third choice. You give *zero* points to the candidates you don't prefer. This is called a Borda count.

This method is open to abuse which the Modified Borda count helps to mitigate. If a voter chooses to only vote for *two* candidates, then they can only give *two* and *one* points. If they only vote for *one* candidate they only get *one* point.

[mbc]: https://en.wikipedia.org/wiki/Borda_count#Modified_Borda_count
### Use Modified Borda Count for Preference Voting

**Author**
Anthony Shull

##### Problem

Voting methods are inherently flawed. They are easy to manipulate. Worse, they can lead to no result or a result that contradicts the actual wishes of the group without even being manipulated.

Let's say you have six candidates, five positions, and 30 voters. If all votes are distributed evenly, you could end up with all six candidates getting 25 votes. There is no way to force a run-off. You're stuck.

Now, let's give an example in which the votes are not evenly distributed. Thirty voters are electing three persons out of a pool of five candidates. One candidate is Pythagoras. Because of his advanced understanding of math, he knows that he can increase his chances of winning by minimizing the total number of votes. He has convinced four followers to vote for him. Usually, when you have 30 people and 3 candidates you would have 90 votes in the pool. If you consider first all the votes of the non-Pythagoreans, you have 75 votes. These breakdown as 19, 17, 16, 12, and 11 with Pythagoras in last place. If he and his four conspirators vote only for him, he moves from 11 to 16 votes and he can force a run-off without any prior knowledge of the other vote totals. If, on the other hand, they have to use all of their votes, they will have to strategically use 10 votes among four candidates. If even one of those 10 votes goes to the person that already has 16 votes, Pythagoras loses. 

See more: [Disposing Dictators, Demystifying Voting Paradoxes] (http://www.amazon.com/Disposing-Dictators-Demystifying-Voting-Paradoxes/dp/0521731607/)

##### Solution

We should use the [Modified Borda count][mbc] for all votes of preference--all votes that are not simply "yes" or "no" or between only two candidates.

Again, an illustration works best. Lets say you have *five* candidates and *three* positions. As a voter, you are asked to give *three* points to your top preference, *two* points to your second choice, *one* point to your third choice. You give *zero* points to the candidates you don't prefer. This is called a Borda count.

This method is open to abuse which the Modified Borda count helps to mitigate. If a voter chooses to only vote for *two* candidates, then they can only give *two* and *one* points. If they only vote for *one* candidate they only get *one* point.

[mbc]: https://en.wikipedia.org/wiki/Borda_count#Modified_Borda_count
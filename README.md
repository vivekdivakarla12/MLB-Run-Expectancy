# MLB-Run-Expectancy

From Chapter 5 of Analyzing Baseball Data with R, by Max Marchi and Jim Albert. 

### Setup
To start this chapter, I read the all2011 and fields csv files, which contain the play-by-play data for the 2011 season. After reading in this data, variables were created for runs in the remainder of the inning, and the run expectancy matrix was set up.
Runner 1, 2, and 3 show if there were players on base during an at bat, and for each combination there is a different calculation of how many runs are expected to be scored. 
<img width="703" alt="Screenshot 2023-11-22 at 1 15 59 PM" src="https://github.com/vivekdivakarla12/MLB-Run-Expectancy/assets/11672096/901d5d15-34dc-479b-8bec-c98b5c78ff41">

### Example - Albert Pujols' Run Expectancy
After creating the run expectancy matrix, the goal of the next step is to run an example on one player - in this instance it is St. Louis Cardinals First Baseman Albert Pujols. 
After loading his data, I viewed how many times he was at bat with each combination of players on base throughout the season, and how many runs he created on each combination. Looking at the table, he had the most at bats with no runners on or a runner on first base, and he produced the most runs in those at bats. 

<img width="193" alt="Screenshot 2023-11-22 at 1 25 32 PM" src="https://github.com/vivekdivakarla12/MLB-Run-Expectancy/assets/11672096/ce4bd9e9-cba5-44fa-bada-5b22952446b4">

After creating the table, I graphed each the same situation, with each dot being an at bat. The biggest takeaway from this graph is when there are more runners on base, the range of run values increase, as there are different possible outcomes. 

<img width="468" alt="Screenshot 2023-11-22 at 1 27 45 PM" src="https://github.com/vivekdivakarla12/MLB-Run-Expectancy/assets/11672096/44b976eb-5815-4001-9014-3bb978d4a9d3">

### Example - Opportunity and Success for All Hitters
The next section includes all hitters who had at least 400 plate appearances in the 2011 season. The main variables I am looking at are run value and Runs.Start, which is the run opportunity for players. The main question in this section is if there is a relationship between the variables, shown by the scatterplot below. 
For the players who generated over 40 runs, almost all of them had a run opportunity over 275, except for Mike Napoli, who was close to 200. This was a big outlier season for Napoli, as he had the highest OPS (1.046) and OPS+ (173) of his career by far. He was batting lower in the order compared to the other players, but still made the most of his opportunities. 
<img width="1388" alt="Screenshot 2023-11-22 at 1 33 54 PM" src="https://github.com/vivekdivakarla12/MLB-Run-Expectancy/assets/11672096/50757212-42e9-48e9-8197-7b6c27cc5cdb">

### Conclusion
I learned a lot from this chapter, and this book has helped me become more comfortable in R, especially when it comes to analyzing baseball data. If I was able to get access of 2023 play-by-play data, I would be interested in recreating these graphs and comparing them to see how the game has changed in the last 12 years. 

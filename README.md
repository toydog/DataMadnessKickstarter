# DataMadnessKickstarter
An analysis on the success of Kickstarter Projects (UM Project)

https://vimeo.com/401928960 

Brian Huynen, I6097103 - Tim Smeets, I6071641

Given the dataset is majorly clean, not much preprocessing was required. It was of greatest interest to keep the main_category, deadline, launched, state, usd_pledged_real and usd_goal_real columns to answer our questions.

We picked main_category over category to make it easier to visualize our findings – it is a hassle to plot a clear graph over the 159 sub-categories as opposed to the 15 main categories. Furthermore, usd_pledged_real and usd_goal_real are defined as the actual amount of money set as goal and yielded from the campaign in USD, which keeps the analysis consistent (since not all projects use the same valuta for its campaign). To define the duration of the project, we used the datetime library to determine the length in days by converting deadline and launched to a date object and subtracting the launchtime from the deadline.

For our analysis, we subdivided the allocated goal budget in four categories:

    • 0 to 1000 USD
    • 1000 – 10000 USD
    • 10000 – 50000 USD
    • 50000 USD and above

Furthermore, we subdivided the duration of projects in three categories:

    • Below 30 days (~1 month)
    • Between 30 and 60 days (~1 to 2 months)
    • Over 60 days (over 2 months)

Doing this allowed us to get a more detailed overview of success rates within projects of different caliber.

Lastly, we plotted a couple of correlation graphs in regards to project duration, goal allocation and the success of a campaign. The idea behind this is to determine in what way the duration and goal are related to a project being successful. From this can be concluded that the size of the goal budget seems to be more detrimental to a project being successful than its length. This correlation remains the same when checking the correlation between duration and success within each goal category and the correlation between goal and success within each duration category.

Conclusion:

From our observations it can be concluded that popular categories do not necessarily guarantee a greater chance of success. It is far more important to not set your goals too high and not make your campaign too long.

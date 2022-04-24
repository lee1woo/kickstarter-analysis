# Kickstarting with Excel

## Overview of Project

### Purpose
    - Fortunately, Louise's play *Fever* was close to reaching its fundraising goal soon after its launch date. In order to measure and better evaluate this performance, I am presenting an analysis of other campaigns on Kickstarter by comparing Louise's experience with other campaign project's launch dates and funding goals. By presenting Lousie with a visualization of outcomes based on launch date as well as funding goals, Louise should be able to use this analysis to inform her decisions moving forward.

## Analysis and Challenges
    - Explain how you performed your analysis using images and links to code, as well as any challenges you encountered and how you overcame them. If you had no challenges, describe any possible challenges or difficulties that could be encountered.
    

### Analysis of Outcomes Based on Launch Date

    - In order to show Louise outcomes based on launch date, I created a pivot table, filtered by parent category and years. In order to do so,  I had to first convert the convert unix timestamps to a readable format. I used the following formula:
     
     ``` 
      =(((J2/60)/60)/24)+DATE(1970,1,1)
     ``` 

    - This allowed me to read the date. After doing so, I used the Years function 'Years()' to extract the year from the "Data Created Conversion" Column. After extracting the years, I created a pivot table and placed outcomes in columns, date created conversion to rows, and count of outcomes to values. This allowed me to filter the data by month and see how many successful, failed, and canceled plays there were over the years.
  
  ![screenshot](https://user-images.githubusercontent.com/102992388/164991277-afa8c7cd-d523-4a23-a039-ea8ee82f6d5a.png)


### Analysis of Outcomes Based on Goals

### Challenges and Difficulties Encountered

    - 

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
    - May is the best month to launch a Kickstarted campaign. Not only did it have the most successful campaigns launched, it also had the highest percentage of successful campaigns relative to total campaigns launched at nearly 67%. It's failure rate was also relatively low, at 31.32%, which was the lowest failure rate out of all months. The worst month to launch a campaign is in December. Only 37 campaigns were successful for a success rate of 49.33%, which was the worst performing month of the year. It also had the highest failure rate at 46.67%. In general, the summer months were more active and successful. 

- What can you conclude about the Outcomes based on Goals?
    - The most successful goals were those that were less than $1,000. There was a general negative correlation between goal and success rate from $1,000 to $29,999. However, strangely enough, after setting a goal of $30,000 you see a positive correlation between goal amount and percentage successful. In fact, the 35,000 to 39,999 range and 40,000 to 44,999 range were tied for third. Yet, we have to be careful about making too large of a generalization because the sample size for these larger campaigns were much smaller. This can indicate a bias or skewed results. For instance, it can be a case that larger campaigns were launched by individuals with prior experience or those who were well-connected to powerful players. Perhaps those who launch a project at $50,000 already knows that that they have a high chance of succeeding because they have rich and powerful friends. 

- What are some limitations of this dataset?
    - Some of the limitations of this dataset is the fact that there were not that many plays launched that had a fundraising goal of higher than $20,000. It is difficult to state anything definitive with such a small data set. For instance, there was only one play that was launched in the $45,000 to $49,999 range, which failed. Some may inadvertently say then individuals must avoid setting a goal at this range because it has a 100% failure rate. However, this is not a fact that can be extrapolated from this dataset.

- What are some other possible tables and/or graphs that we could create?
    - A bar graph, or specifically a clustered column graph can come in handy. 
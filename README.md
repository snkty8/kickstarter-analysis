# An Analysis of Kickstarter Campaigns
Trends of Kickstarter analysis
Analysis of Challange 1

1. Overview of Project: Explain the purpose of this analysis.

	This is analysis shows how different play campaigns compared in 
	relation to thier launch date and funding goals.
	
2. Analysis and Challenges: Explain how you performed your 
	analysis using images and links to code, as well as any 
	challenges you encountered and how you overcame them. 
	If you had no challenges, describe any possible challenges 
	or difficulties that could be encountered.
	
	The pivot table was a little confusing at first.  Getting the
	correct information into each correct section (filter, rows, columns, etc...).
	By trial and error, I was able to get everything into the correct
	position.
	
	In the next section, the correct syntax was hard to come up 
	with in the function section.  The first was not a problem.
	I knew I needed column D for goal, column F for outcome, and 
	column R for plays. Finding those less than 1000 was the easy 
	part in comparision, but coming up with the correct syntax for
	less than and greater was a bit harder.  After playing around, 
	and the use of google, I was able to find the correct way to use
	the function.  This is the URL that was the most helpful:

	https://support.microsoft.com/en-us/office/countif-function-e0de10c6-f885-4e71-abb4-1f464816df34
	
	I was able to come up with this 
	formula:

	=COUNTIFS(KickStarter!D:D,">=1000",KickStarter!D:D,"<=4999",KickStarter!F:F,"successful",KickStarter!R:R,"plays")

  I adjusted the function for the rest of the values in the remaining rows.
	
3. Results: Answer the following questions in complete and coherent sentences.
	What are two conclusions you can draw about the Theater Outcomes by Launch Date?
	What can you conclude about the Outcomes based on Goals?
	What are some limitations of this dataset?
	What are some other possible tables and/or graphs that we could create?
	
	
	Purly looking at the data presented, May, June, and July have more successful
	results than the rest of the months. These months are usually the warmest of 
  	the year.  People are typically out and about.  Supporting and attending a play
  	would be more successful, from a weather stand point. December has the 
	lowest results, this is the same month as Christmas.  The general public
	are usually focused on shopping for Christmas gifts, rather than spending 
	money on other things. With the same thought, Januray is more than likely
	low because poeple are trying to catch up from spending so much 
	during the month of December. (Image of the chart below)

![image](https://github.com/snkty8/kickstarter-analysis/blob/main/resources/Theater_Outcomes_vs_Launch.png)	
	
	The lower the goal, the more successful they were in acheiving.  
	This is clearly seen in the excel file, as well as the Outcomes Vs Goals Chart.

![image](https://github.com/snkty8/kickstarter-analysis/blob/main/resources/Outcomes_vs_Goals.png)
	
	None of the live shows are taken into account.  The is somewhat skewed due 
	this the fact.  It doesn't take into account if these shows 
	met thier goals or not.  Location would be a good focal point, as well.  Although I've made assumptions about the weather being a factor, I cannot say for certain this was the case. Actual statical analysis would have nice to see if there are 
	any outliers, or shows that stood out.

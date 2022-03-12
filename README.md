## **Kickstarter Campaign Outcomes Based on Launch Dates and Funding Goals**

### Overview of Project

#### The purpose of this project is to analyze how different crowdfunding campaigns for plays faired in relation to their launch dates and funding goals.

### Analysis and Challenges

#### Analysis of Outcomes Based on Launch Date
- A new column was created in the Kickstarter worksheet and was named "Years"
- A pivot table was created with "Parent Category" and "Years" as filters; "outcomes" as both column and values; and "date created conversion" as rows.
- The pivot table was filtered in Parent category to theater
- The pivot table was also filtered in the setting section to not include "live" from the output
- A line chart was created from the pivot table.  The line chart shows the trends of successfull, failed, and canceled campaigns based on the month of launch date.
- Unnecessary labels were taken out from the chart.
#### Analysis of Outcomes Based on Goals
- A new worksheet was created named "Outcome Based on Goals"
- In this worksheet, 8 rows were created namely: goal, number successful, number failed, number canceled, total projects, percentage successful, percentage failed and percentage canceled
- The goal fields were filled in beginning with <1000 and with increments of about 5000 up to greater than 50000
- The "COUNTIFS" formula was used to calculate the number of successful field by using this syntax:
		- =COUNTIFS(Kickstarter!$F:$F,"successful",Kickstarter!$R:$R,"plays",Kickstarter!$D:$D,"<1000")
- The same formula was applied to find the number of failed and canceled campaigns
#### Challenges and Difficulties Encountered
- When analyzing Outcomes Based on Launch Date, the challenge encountered with this analysis was that, in the row column, when "date created converted" was chosen, the pivot table created included also the years and quarters instead of just the month of the year.  I was able to fix this by dragging the "year" and "quarter" out of the row field so only the months show in the output
- When analyzing Outcomes Based on Goals, the challenge is that I had to manually change the formula for each count.  At this point, I have know of no faster way to do this but to change the "COUNTIFS" arguments.

### Results

- Outcomes Based on Launch Date analysis shows that May is the best month to launch a crowdfunding campaign and December is the worst month to launch a crowdfunding campaign.

- Outcomes based on Goals analysis shows that:
####
- A crowdfunding goal of less than $5,000 will has a success rate of 73-76%.
- A crowdfunding goal between $5,000-$24,999 have a success rate of 45-55%
- A crowdfunding goal between $25,000-$34,999 have a success rate of 20-27%
- Surprisingly, a crowdfunding goal between $35,000-$49,000 have a success rate of 67%
- A crowdfunding goal between $45,000-$49,000 has 0% success rate
- A crowdfunding goal of $50,000 or more has a 17% success rate


### The Limitations of the Data Set is that we could probably use data that tells us what platform the crowdfunding campaign was launched on or what were the demographics of the donors.

Possible tables we can create are the %Successful outcomes based on Month launched; since Louise is in the US, it’s probably better to filter all the analysis with the country, US.

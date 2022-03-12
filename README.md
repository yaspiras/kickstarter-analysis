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
- The challenge encountered with this analysis was that, in the row column, when "date created converted" was chosen, the pivot table created included also the years and quarters instead of just the month of the year.
- I was able to fix this by dragging the "year" and "quarter" out of the row field so only the months show in the output
- The challenge is that I had to manually change the formula for each count.  At this point, I have know of no faster way to do this but to chang the "COUNTIFS" arguments.

### Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

- What can you conclude about the Outcomes based on Goals?

- What are some limitations of this dataset?

- What are some other possible tables and/or graphs that we could create?

*Problem Statement:

1.Find the average Customer Satisfaction rating.
2.Determine the overall number of calls answered and abandoned.
3.Analyze overall call resolution statistics.
4.Calculate the average speed of answer (in seconds) by agents.
5.Determine the number of calls per month.
6.Analyze agent-wise call statistics.


DAX Used:

1.Answer call

Answer = CALCULATE(COUNT(Sheet1[Call Id]), FILTER(Sheet1, Sheet1[Answered (Y/N)] = "Y"))
This DAX formula calculates the total number of calls that were answered.

2.Resolved Call:

Resolved (Y) = CALCULATE(COUNT(Sheet1[Call Id]), FILTER(Sheet1, Sheet1[Resolved] = "Y"))
This DAX formula calculates the total number of calls that were resolved.

*Insights:

The average Customer Satisfaction rating is 3.40, which falls short of the target of 4.50. Efforts are needed to improve customer satisfaction.

The dashboard shows that 4.05K calls were answered (using the Answer measure), while 0.95K calls were not answered. The call center needs to identify and address the reasons for unanswered calls to enhance customer satisfaction.

Approximately 3.65K calls were resolved (using the Resolved measure), whereas 1.35K calls remained unresolved. The call center should focus on resolving these unresolved calls to improve customer satisfaction.

The average speed of answer by agents was recorded at 67.52 seconds.

Number of Calls Answered:
January: 1,455
February: 1,298
March: 1,301

Number of Calls Not Answered:
January: 317
February: 318
March: 311

Overall Calls Per Month:
January: 1,772
February: 1,616
March: 1,612
Agent Statistics:

Agent-wise data is available on the dashboard, allowing for a focus on the performance of each agent individually.

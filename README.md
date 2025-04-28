# MIST4610GroupProject2
# Team Name
Sp25_21479_Group2
# Team Members 
1. Buckner, Alexa [@amb21398]()
2. Eloore, Neha [@neloore]()
3. Nguyen, Hung @[triumviratesys]()
4. Spraker, Dabney @[dps24510]()
5. Dorrien, Leah [@leahdorrien2]()
# Dataset Description
  For this project, our group chose to use a dataset entitled Selected Online Casino Gambling which can be found at this link https://catalog.data.gov/dataset/selected-online-casino-gaming-data. We obtained our data from a US Data Gov website that was provided, https://catalog.data.gov/dataset. This dataset contains selected online casino gambling data for four licensces in the state of Connecticut. The range of time that this dataset covers is October 21st, 2021 through March 31st, 2025. It lists data from four gambling licensees in the state, including their operating license, financials including wages, monthly payments, patron winnings and losses, and gambling revenue for every fiscal year. 
  
  Three of the four licensees included in this data set are related to the Native American Mohegan tribe in Connecticut, who are a federally recognized tribe that has been operating the Mohegan Sun casino since 1996. It is common for Native American tribes to be heavily involved in the gambling industry as they are often given more leeway from regulators.
  
1. Mohegan Tribe On-Reservation: Refers to Mohegan tribe’s general gambling operations on their federal reservation.

2. MPTN On-Reservation: Mashantucket Pequot Tribal Nation. The Mohegan tribe were a part of the Pequot tribe until the early-mid 17th century. Refers to the Pequot tribe’s general gambling operations on their federal reservation.

3. MPI Master Wagering License, CT, LLC: A “master” license that covers many other licenses (i.e. key employee license, live employee license). Allows the tribe to operate online casino gaming, sports wagering, and fantasy contests.

4. Mohegan Digital, LLC: A subsidiary of Mohegan Gaming & Entertainment. Handles online gaming gambling platforms, for instance e-bingo or sports betting. 

Each row is data from one license for a particular month.

Explanations of column information can be found below.

- Licensee: In order to be considered a valid online gambling company by Connecticut, the party must obtain a license. The following data is string data and lists the names of the party’s who are licensee’s for online gambling. 

- Fiscal Year: The fiscal year is the 12 month accounting period where companies and organizations track their finances. The following data is string data that lists the beginning year and ending year for their record keeping. This is relevant in helping these organizations keep track of which winnings were associated with each fiscal year.

- Month Ending: The month ending is used for the purposes of calculating monthly payments for that month’s period. Organizations have to make a monthly payout to the state of the 15th of the following month that revenue was gained. For example, the organization can have data from the Month of January– the month ending would be January 31st at 12:00am to notify the organization that the revenue obtained by the business must be contributed towards the monthly payments on the 15th the following month to the state (February 15th). The following data is Date & Time data.

- Wagers: Wagers determine the number of wagers made for each license in a specific month. The following data is Number (whole) data.
Patron Winnings: The patron winnings is the number of wagers that patrons won. The following data is Number (whole) data

- Cancelled Wagers: The cancelled wagers represents the number of wagers that the licensee has canceled or written off by month. The following data is Number (whole) data.

- Online Casino Gambling Win/(Loss): How much each casino/licensee earned during the month from online wagers in dollars. Win/Loss = Wagers - Patron Winnings - Canceled Wagers.

- Promotional Coupons or Credits Wagered (3): Coupons/credits used in place of currency for the purposes of online gambling, as a promotional tool to entice potential customers. 

- Promotional Deduction (4): How much is actually deducted from gambling revenue during the month from promotional coupons/credits. 

- Total Gross Gambling Revenue: How much revenue each casino earned during the month. Online Win/Loss - Promotional Deduction. 

- Payment (5): How much each casino pays out to its employees in dollars. Payment rate is 18% of Gross Gaming Revenue until September 2026, 20% for all subsequent periods, and does not apply to negative revenue.

# Question 1 and Importance
Is there a correlation between promotional coupons/credits wagered and total gross gambling revenue? How does the correlation differ betweens licesnsees?

  By examining the relationship between promotional coupons and gross gambling revenue, we can assess the efficiency of promotions as a marketing tool. This then informs long-term marketing strategy as well as present product/sales mix. 
  
  The question is especially salient within the dataset we are using, as all four licensees are online gambling operations. For mobile gambling applications in particular, promotional coupons are often seen in the form of “free” in-game currency offerings, or “risk-free” bets. It is the conventional wisdom that such microtransactions substantially enhance the feedback loops that make online gambling so enticing and thus an extremely effective money-maker. By providing an on-ramp that introduces prospective players to the experience, these promotions can have a strong effect on gross revenue. While this makes rather intuitive sense, others have proposed the idea that the mechanism that makes these games so addictive is the stress of losing, or at least the risk of losing it all. 
  
  Through this online gambling data from Connecticut, we can test these theories and the effectiveness of promotional coupons and credits.
  
  State and federal governments have concerns about promotional deductions taking away from the taxable base of a firm’s revenue. As such, policies like Connecticut’s Act 21-23 have gradually lowered the maximum percentage of revenue that can be deducted as promotional deductions from 25% to 15%. 


# Question 1 Tableau Visualization
<img width="800" alt="image" src="https://github.com/user-attachments/assets/e15e2588-7cee-44b8-908d-81df5262f464" />

- for the On-Reservations (much smaller operations)

<img width="797" alt="image" src="https://github.com/user-attachments/assets/ebf1d238-1097-4359-9efb-099d27b8b6ed" />

- for the LLCs (much larger operations)
# Question 1 Analysis
  The data was split into two sections due to a difference in scope and scale. Separating the graphs allowed us to clearly see the pattern, if existent, between promotional coupons/credits wagered versus the gross gambling revenue of a particular license. This visualization focuses on long term effectiveness of promotional coupons. 
  
  As seen in the second graph, there is an extremely strong correlation between these two for the Mohegan Digital LLC with each line mirroring the other on every drop and peak in the graph. This suggests that they are implementing their promotions in the most effective way causing gross revenue to rise when more promotional coupons/credits are used. This also suggests that they have the highest return on investment from these promotions.
  
  While not close to as strong as Mohegan Digital LLC's correlation, MPI Master Wagering License CT, LLC shows a correlation between promotional coupons/credits especially in the last six months of the year suggesting that their implementation of promotions is having an impact on revenue and is giving them atleast some return on investment.
  
  The on-reservation online gambling data, however, that is exhibited in the first screenshot, shows no clear long term relationship. This suggests that their implementations of promotions are not leading to higher gross gambling revenues. This means that they are more likely than not losing money on promotions rather than gaining and need to adapt their strategy. 
  
  It is important to also note that taxes are not taken into account when looking at gross gambling revenue. Since promotions can be taken away from the taxable base of a licensee's revenue, there is postive tax break that comes from promotions. This means that the promotional coupons have a positive effect on profit that is not shown in the visualizations and should be taken into account when looking at ROI.

# Question 2 and Importance
What is the total number of wagers placed across all licensees during a specific fiscal year? Does start time of operations have an effect?

  Regardless of the type of gambling operation being run, it is obvious that the total number of the wagers for a particular firm/licensee placed will reflect both overall market growth and the relative performance of said licensee. There were several possible dynamics that we wanted to consider when analyzing the results of this.
 
  It can inform us of the status of the marketas a whole, whether it is growing, stabilizing, or dying. It will also show if there are any dominant players with sustainable competitive advantages. The start dates are important to consider to see the impact first-mover advantage in the online gambling market. While the visualization will be hard to draw direct causations from, the patterns can help guide furhter research into why licensees are performing in these ways.

# Question 2 Tableau Visualization
<img width="800" alt="image" src="https://github.com/user-attachments/assets/7de50e1b-0992-4ff4-a403-55856241f3af" />

- for the On-Reservations (much smaller operations)

<img width="791" alt="image" src="https://github.com/user-attachments/assets/c93917c6-6d67-4a0a-bb73-dfd836c4cd3b" />

- for the LLCs (much larger operations)
# Question 2 Analysis
  There are a few important things to consider when examining the visuals for this question. Most importantly there are differing start dates for licensees and not all years contain the same amount of operating months due to the data ending in March rather than at the end of the 24/25 fiscal year. 

The start dates of each license are as follows
- Mohegan Digital LLC and MPI Master Wagering License CT, LLC (Oct. 2021)
- MPTN On-Reservation (Dec. 2021) 
- Mohegan Tribe On-Reservation (May 2022)

  The LLCs, both Mohegan Digital and MPI Master Wagering License CT, were the first movers in this market and have sustained much higher wager numbers than the smaller operations of the on reservation licensees. Because the difference is so drastic, over 8 billion compared to 30 million at their respective peaks, the graphs were again split into LLC and on-reservation to be able to see the trends clearly. While first-mover advantage is on the larger operations' side, the difference in operations is probably mostly due to the size of their companies and establishment in other markets before Connecticut.
  
  MPI Master Wagering consistently leads in wager volume each year, suggesting higher user engagement or broader reach compareed to its competitors. The consistency of their dominance shows that they have a sustainable advantage and likely better operations separate from any early market advantage. 

  When looking at the overall market focusing on the bigger players, it seems that the market is beginning to fail, but it is more likely stabilizing, still growing but at a decreasing rate, when accounting for the fact that 24/25 is missing multiple months worth of wager numbers. This growing but at a decreasing rate would be consistent with the difference between 22/23 and 23/24 making it all the more likely the true state of the market.

  The smaller on-reservation licensees offer another perspective on the advantage of getting into the market early. While neither joined at the time of the LLCs, MPTN On-Reservation had a small establishment advantage over Mohegan Tribe On-Reservation after starting operations earlier; however, this evened out by the 24/25 fiscal year suggesting that it is not a sustainable advantage.


# Tableau Workbook
The file is attached.

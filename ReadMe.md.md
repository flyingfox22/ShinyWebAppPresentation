Malaysia Home Loan Calculator And Payment Schedule Simulation App
========================================================
author: Thomas Lee Wai Siong
date: January 25th, 2016
transition: rotate
transition-speed: fast
rtl: false
font-family: 'Helvetica'
Why you should understand your monthly house loan repayments before getting a new loan application?

What is House Loan Calculator?
========================================================
incremental: true
type: prompt

Malaysia home loan calculator to estimate your monthly house loan repayments.
In order to know your monthly house loan repayments, you must provide the infomations below:

- Property price in Malaysian Ringgit
- Down payment amount in Malaysian Ringgit
- Housing loan period in Years
- Loan interest rate in Percentage.

Why you should be aware of your house loan repayments
========================================================
incremental: true
type: alert

- Recent US rate hike puts Malaysia on the moderate risk.
- The language used by the FOMC in their latest statement suggests that the pace of rate hikes will be **gradual** as opposed to **measured**.
- The FOMC also released projections that signalled four rate hikes of 25 basis points each in 2016.
- In the short-term, there is a high possibility of central banks around the world
making monetary policy adjustments in response to the the Fed rate hike including **Malaysia**
- Malaysia Overnight Policy Rate (OPR) unchanged at **3.25%**
- Current FED Rate **0.25%** to **0.50%**


How do you find out your monthly repayments?
========================================================

The formula for housing loan monthly repayments is

```r
propertyPrice<-500000
downPayment<-50000
interestRate<-4.25
loanPeriod<-35

loanAmount <- propertyPrice - downPayment
interestRate <-interestRate/100
loanPeriod <- loanPeriod * 12 
payment <-(loanAmount) * (((1 + interestRate/12)^ loanPeriod) * interestRate)/(12 * (((1+interestRate/12)^ loanPeriod) - 1))
round(payment,2)
```

```
[1] 2060.52
```

Malaysia Home Loan Calculator And Payment Schedule Simulation App
========================================================
incremental: true
- Estimate monthly home loan repayment amount.
- Generate pie chart of housing loan principal versus interest amounts.
- Generate principal, interest and balance loan repayment chart, over loan period.
- Generate principal, interest and balance loan repayment table, by year.
- You can access the Shiny App at [here](https://leewaisiong.shinyapps.io/ShinyWebApp/)
- You can access the Shiny GitHub Code at [here](https://github.com/flyingfox22/ShinyWebApp)
- You can access the Presentation Code at [here](https://github.com/flyingfox22/ShinyWebAppPresentation) and [here](https://github.com/flyingfox22/ShinyWebAppPresentation)


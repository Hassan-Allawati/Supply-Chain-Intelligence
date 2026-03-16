🚢 Maritime-Procurement Risk Audit
Sohar Port Strategic Data Analysis
📝 Executive Summary

As a Chief Commercial Officer (CCO), I conducted a multi-objective audit to bridge the gap between internal procurement performance and external global maritime benchmarks. By joining internal shipment data with UNCTAD maritime efficiency metrics, I identified $1.8M in high-risk capital tied to suppliers operating in congested port regions.
The Results (Evidence)

The following table is the output of the Strategic Risk Join (Objective 4). It correlates our financial exposure with real-world port delays.

    Key Insight: Gamma_Co represents our highest risk profile, with nearly $1.9M in "Value at Risk" and a regional port delay of 1.60 days (Russian Federation).

Project Objectives & SQL Logic
Objective 1: Value at Risk (Financial Exposure)

I calculated the total value of all non-delivered orders to identify where our capital is "frozen."

    Logic: SUM(Quantity * Negotiated_Price) filtered by Order_Status.

Objective 2: Lead-Time Audit

A performance review of internal supplier reliability.

    Logic: Used DATE_DIFF to measure the gap between Order and Delivery dates.

Objective 3: Maritime Benchmarking

Analyzing external "bottlenecks" using the Maritime Port Performance Dataset.

    Logic: Filtered for 'Container ships' in the '2023-S2' period to get the most recent median wait times.

Objective 4: The Strategic "Logic Bridge"

Since the datasets did not share a common ID, I built a Common Table Expression (CTE) to map suppliers to their home regions.
🚀 Business Recommendation

    Mitigation: Immediate review of Gamma_Co's contract due to the combination of high financial exposure and high regional port congestion.

    Optimization: Diversify high-priority shipments toward Alpha_Inc in Singapore, where port turnaround is 46% faster.

How to read the files:

    /SQL_Queries: Contains the raw scripts for each objective.

    /Datasets: Contains the procurement and maritime data source files.

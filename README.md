# Udemy Advanced SQL: MySQL Data Analysis & Business Intelligence

# Introduction 
<details>
<summary> click here for more </summary>
<br>
👩🏻‍💼 THE SITUATION

You’ve just been hired as an eCommerce Database Analyst for Maven Fuzzy Factory, an online retailer which has just launched their first product.

📈 THE BRIEF

As a member of the startup team, you will work with the CEO, the Head of Marketing, and the Website Manager to help steer the business.

You will analyze and optimize marketing channels, measure and test website conversion performance, and use data to understand the impact of new product launches.

✏️ THE OBJECTIVE

Use SQL to:

Access and explore the Maven Fuzzy Factory database
Become the data expert for the company, and the go-to person for mission critical analyses
Analyze and optimize the business’ marketing channels, website, and product portfolio

</details>

## Table of Contents
[Entity Relationship Diagram](#Entity_Relationship_Diagram)
<details>
  <summary> click here to expand ERM </summary>
  <img width="718" alt="Screenshot 2022-12-08 at 09 26 17" src="https://user-images.githubusercontent.com/66598945/206374847-1901a945-bf9b-4dfc-a02f-9cbffe4ff426.png">
  <br>
 <p>We will be working with six related tables, which contain eCommerce data about:
   <li> Website Activity</li>
   <li> Products </li>
   <li> Orders and Refunds </li>
   
We'll use MySQL to understand how customers access and interact with the site, analyze landing page performance and conversion, and explore product-level sales.</p>

  </details>

[Analyzing Traffic Sources](#Analyzing_Traffic_Sources)
<p>Traffic Source Analysis

<li>Understanding where the customers are coming from and which channels are driving the highest quality traffic.</li>
<li>Typically, traffic sources are email, social media, search engine, and direct traffic.</li>
<li>Looking at conversion rate (CVR) which is the percentage of the traffic that converts into sales or revenue activity.</li> </p>

<p>Why is it important to conduct Conversion Rate Analysis?

<li>Shift budget towards search engines, campaigns, or keywords driving the highest conversion rate.</li>
<li>Compare user behaviour across traffic sources to customize messaging strategy.</li>
<li>Identify opportunities to eliminate paid marketing channel or scale performing traffic.</li> </P>

<p>In this section, we will learn about
<li>Analyzing top traffic source</li>
<li>Bid optimization and trend analysis<li>
</p>

# Q1:Finding Top Traffic Sources
<img width="520" alt="Screenshot 2022-12-08 at 10 52 00" src="https://user-images.githubusercontent.com/66598945/206392449-f1b6eebb-a5ca-4550-a9ee-cff3d8d9bc86.png">
<li>Stakeholder (ST)'s request: Breakdown of sessions by UTM source, campaign and referring domain up to 12-04-2012</li>
<li>Results: utm_source | utm_campaign | http_referer | sessions (count)</li>
<li>Steps: Filter results up to sessions before '2012-04-12' and group results by utm_source, utm_campaign and http_referer</li>
<br>
<img width="351" alt="Screenshot 2022-12-08 at 10 57 44" src="https://user-images.githubusercontent.com/66598945/206392974-23a0c180-5e9f-4048-a00a-e4a5a5a5e80e.png">
<br>
<img width="495" alt="Screenshot 2022-12-08 at 10 58 02" src="https://user-images.githubusercontent.com/66598945/206393112-429bd548-4ad0-4c23-bfd6-49a79d15004a.png">
<br>
<img width="511" alt="Screenshot 2022-12-08 at 11 09 19" src="https://user-images.githubusercontent.com/66598945/206393759-6ce1e7ca-df25-460c-ba8b-105a01c0568f.png">

<p> Insights </P>

<li>Drill deeper into gsearch nonbrand campaign traffic to explore potential optimization opportunities</li>
<li> Await further instruction from Tom </li>

# Q2: Traffic Conversion Rates
<img width="294" alt="traffic_conversion" src="https://user-images.githubusercontent.com/66598945/206400905-45e108c3-d241-49bc-82c3-b695e3f528ad.png">
<li>ST request: Calculate CVR from session to order. If CVR is 4% >=, then increase bids to drive volume, otherwise reduce bids.</li>
<li>Results: sessions (count) | orders (count) | conversion rate</li>
<li>Steps: Filter sessions < 2012-04-12, utm_source = gsearch and utm_campaign = nonbrand</li>
  <br>
  <img width="562" alt="Screenshot 2022-12-08 at 11 40 30" src="https://user-images.githubusercontent.com/66598945/206403083-27dd2c5b-86bf-4e2e-ba21-042ccfa2507b.png"> 
  <br>
  <img width="280" alt="Screenshot 2022-12-08 at 11 40 48" src="https://user-images.githubusercontent.com/66598945/206403248-3b4b35fd-0723-45e9-85cf-a30a7c079c9e.png">
<br>
  
<br>
<img width="292" alt="traffic_conversion2" src="https://user-images.githubusercontent.com/66598945/206400972-2057f071-f24d-4b77-ba04-b92448329b55.png">  
  <br>
  <p>Insights: Conversion rate is 2.92%, which is less than 4%, hence we're overspending on gsearch nonbrand campaign and have to reduce bids. To monitor impact of bid reduction for the campaign.</p>
  
  # Bid Optimization & Trend Analysis
  <p>Analysing for bid optimization is understanding the value of various segments of paid traffic to optimize marketing budget.</p>
 <li> Our job is to figure out the right amount of bid for various segments of traffic based on our potential revenue.</li>
<ul>How do we do that?
  <li>Use conversion rate and revenue per click to figure out how much you should spend per click to acquire customers.</li>
  <li>Understand how website and products are performing for subsegments of traffic to optimise within channels.</li>
  <li>Analyse impact of bid changes have on ranking</li>
</ul>
  
[Analyzing Website Performances](#Analyzing_Website_Performances?)
[Mid-Course Project](#Mid-Course_Project)
[Analysis for Channel Portfolio Management](#Analysis_for_Channel_Portfolio_Management?)
[Analyzing Business Patterns and Seasonality](#Analyzing_Business_Patterns_and_Seasonality)
[Product Analysis](#Product_Analysis)
[User Analysis](#User_Analysis)
[Final Project](#Final_Project)

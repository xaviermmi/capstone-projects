# Food claims process
![brazilian_food-unsplash](https://github.com/xaviermmi/capstone-projects/assets/122324304/d3c401ca-149a-43f9-9520-6acdd19d5332)

## 1. Introduction
<p>Vivendo is a fast food chain in Brazil with over 200 outlets. As with many fast food
establishments, customers make claims against the company. For example, they blame Vivendo for suspected food poisoning.</p>
<p>The legal team, who processes these claims, is currently split across four locations. The new
head of the legal department wants to see if there are differences in the time it takes to close
claims across the locations.</p>

## 2. Project instructions
The legal team has given us a dataset where each row is a claim made against the
company. They would like us to answer the following questions:
<li>How does the number of claims differ across locations?
<li>What is the distribution of time to close claims?
<li>How does the average time to close claims differ by location?</li>

## 3. Dataset
<div style="background-color: #ebf4f7; color: #595959; text-align:left; vertical-align: middle; padding: 15px 25px 15px 25px; line-height: 1.6;">
    <div style="font-size:20px"><b>datasets/claims.csv</b></div>
<ul>
    <li><b>Claim ID:</b> Character, the unique identifier of the claim.</li>
    <li><b>Time to Close:</b> Numeric, number of days it took for the claim to be closed.</li>
    <li><b>Claim Amount:</b> Numeric, initial claim value in the currency of Brazil. For example, “R$50,000.00” should be converted into 50000.</li>
    <li><b>Amount Paid:</b> Numeric, total amount paid after the claim closed in the currency of Brazil.</li>
    <li><b>Location:</b> Character, location of the claim, one of “RECIFE”, “SAO LUIS”, “FORTALEZA”, or “NATAL”.</li>
    <li><b>Individuals on Claim:</b> Numeric, number of individuals on this claim.</li>
    <li><b>Linked Cases:</b> Binary, whether this claim is believed to be linked with other cases, either TRUE or FALSE.</li>
    <li><b>Cause:</b> Character, the cause of the food poisoning injuries, one of ‘vegetable’, ‘meat’, or ‘unknown’. Replace any empty rows with ‘unknown’.</li>
</ul>
    </div>
  
## 4. Skills
<p>This project is showcasing some data validation, exploratory analysis and visualization techniques.</p>
<p>In terms of code, we use :
<ol>
<li><code>pandas</code> for data validation and EDA
<li><code>matplotlib</code> for base plot and subplots framework
<li><code>pandas</code> and <code>seaborn</code> for more advanced dataviz (built on top of matplotlib)
</li></ol>
</p>

## 5.Notebook structure
The project notebook is organized in 3 parts :
<ol>
<li>Imports & setup
    <ul>
      <li>libraries
      <li>viz parameters
      <li>load dataset</li>
    </ul>
<li>Data preparation
    <ul>
      <li>validation
      <li>cleaning</li>
    </ul>
<li>Exploration & visualization
    <ul>
      <li>Preliminary EDA
      <li>Answering 1st question : How does the number of claims differ across locations?
      <li>Answering 2nd question : What is the distribution of time to close claims?
      <li>Answering 3rd question : How does the average time to close claims differ by location?</li>
    </ul>
</li></ol>

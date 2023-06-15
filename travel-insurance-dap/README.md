# Case Study - Travel Insurance company
![umbrella-unsplash](https://github.com/xaviermmi/capstone-projects/assets/122324304/12c47507-3fb5-4a03-a54f-e7155c807e4c)

## 1. Introduction
<p>Travel Assured is a travel insurance company. <br>
Due to the COVID pandemic, they have had to
cut their marketing budget by over 50%. It is more important than ever that they advertise in the right places and to the right people.
Travel Assured has plenty of data on their current customers as well as people who got quotes but never bought insurance.</p>

## 2. Project instructions
What the business wants to know:
<li>Are there differences in the travel habits between customers and non-customers?
<li>What is the typical profile of customers and non-customers?</li>

## 3. Dataset
<div style="background-color: #ebf4f7; color: #595959; text-align:left; vertical-align: middle; padding: 15px 25px 15px 25px; line-height: 1.6;">
    <div style="font-size:20px"><b>datasets/travel_insurance.csv</b></div>
<ul>
    <li><b>Age:</b> Numeric, the customer’s age</li>
    <li><b>Employment Type:</b> Character, the sector of employment</li>
    <li><b>GraduateOrNot:</b> Character, whether the customer is a college graduate</li>
    <li><b>AnnualIncome:</b> Numeric, the customer’s yearly income</li>
    <li><b>FamilyMembers:</b> Numeric, the number of family members living with the customer</li>
    <li><b>ChronicDiseases:</b> Numeric, whether the customer has any chronic conditions</li>
    <li><b>FrequentFlyer:</b> Character, whether a customer books frequent tickets</li>
    <li><b>EverTravelledAbroad:</b> Character, has the customer ever travelled abroad</li>
    <li><b>TravelInsurance:</b> Numeric, whether the customer bought travel insurance</li>
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
The project notebook is organized in n parts :
<ol>
<li>Imports & setup
    <ul>
      <li>libraries
      <li>viz parameters</li>
    </ul>
<li>Dataset load and cleaning
    <ul>
      <li>data validation
      <li>datatypes update</li>
    </ul>
<li>Preliminary EDA
<li>Q1:Differences between customers and non-customers' travel habits
  <ul>
    <li>Flyers' frequency of flights
    <li>Flyers' international-flights habits</li>
  </ul>
<li>Q2:Typical profile of customers and non-customers
  <ul>
    <li>Ordering personal features
    <li>Ordering professional features
    <li>Personal profiles
    <li>Professional profiles</li></ul>
<li>Conclusion and recommendations
</li></ol>

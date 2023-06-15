# Case Study - Recipe site traffic
![website-recipe-unsplash](https://github.com/xaviermmi/capstone-projects/assets/122324304/99eb6651-38b1-46ef-a778-80837c71b736)

## 1. Introduction
<p>Tasty Bytes was founded in 2020 in the midst of the Covid Pandemic. The world wanted inspiration so we decided to provide it. We started life as a search engine for recipes, helping
people to find ways to use up the limited supplies they had at home.</p>
<p>Now, over two years on, we are a fully fledged business. 
For a monthly subscription we will put together a full meal plan to ensure you and your family are getting a healthy, balanced diet whatever your budget. Subscribe to our premium plan and we will also deliver the ingredients
to your door.</p>

## 2. Project instructions
<p>The final target of this case study is to improve traffic on the website. Indeed, traffic means more subscriptions, so this is really important to the company.
Marketing department has noticed that the home page has a high impact on the traffic to the rest of the website, which goes up by as much as 40% if a popular recipe is picked.</p>
<p>Our objective is to help the Product Manager, who is responsible for choosing which recipes to display on the homepage each day.
At the moment, he chooses his favorite recipe from a selection and display that on the home page.
But he needs to know how to decide if a recipe will be popular and, if possible, automate it.</p>
<p>The marketing department wants us :
<ol>
<li>to predict which recipes will be popular 80% of the time
<li>to predict which recipes will lead to high traffic ; that is to say minimize the chance of showing unpopular recipes.</li></ol>
</p>

## 3. Dataset
<p>The product manager has tried to make this easier for us and provided data for each recipe, as well as whether there was high traffic when the recipe was featured on the home page.</p>

<div style="background-color: #ebf4f7; color: #595959; text-align:left; vertical-align: middle; padding: 15px 25px 15px 25px; line-height: 1.6;">
    <div style="font-size:20px"><b>datasets/recipe_site_traffic_2212.csv</b></div>
<ul>
    <li><b>recipe:</b> Numeric, unique identifier of recipe</li>
    <li><b>calories:</b> Numeric, number of calories</li>
    <li><b>carbohydrate:</b> Numeric, amount of carbohydrates in grams</li>
    <li><b>sugar:</b> Numeric, amount of sugar in grams</li>
    <li><b>protein:</b> Numeric, amount of protein in grams</li>
    <li><b>category:</b> Character, type of recipe. Recipes are listed in one of ten possible groupings (Lunch/Snacks', 'Beverages', 'Potato','Vegetable', 'Meat', 'Chicken, 'Pork', 'Dessert', 'Breakfast', 'One Dish Meal').</li>
    <li><b>servings:</b> Numeric, number of servings for the recipe</li>
    <li><b>high_traffic:</b> Character, if the traffic to the site was high when this recipe was shown, this is marked with “High”.</li>
</ul>
    </div>
  
## 4. Skills
<p>This project is showcasing some exploratory analysis and machine learning concepts (supervized, unsupervized, pipelines, etc.) illustrated with visualization techniques.</p>
<p>In terms of code, we use :
<ol>
<li><code>pandas</code> for data validation and EDA
<li><code>matplotlib</code> and <code>seaborn</code> for advanced dataviz
<li><code>scikit-learn</code> for preprocessing, machine-learning pipelines and cross-validations
</li></ol>
</p>

## 5.Notebook structure
The project notebook is organized in n parts :
<ol>
<li>Big picture of the problem
    <ul>
      <li>Problem definition
      <li>Import libraries, setup dataviz parameters and load data
      <li>Data validation
        <ul>
          <li>raw descriptive stats and data types
          <li>numeric datatype distribution
          <li>object datatype
          </li></ul>
      <li>Conclusion and promising imputation & transformations
        </li>
    </ul>
<br>
<li>Exploratory Data Analysis
    <ul>
      <li>Splitting features from label : Category-stratified train_test_split
      <li>Deep-insight of data (scaled distributions, correlations) : missing data, detailed distributions & correlations
      <li>Feature engineering : (categorized) PCA, features clustering
      <li>Imputation of missing values : KNNImputer, SimpleImputer iterated on categories
      <li>Promising further transformations</li>
    </ul>
<br>
<li>Preprocessing
    <ul>
      <li>Custom transformers (from category clsutering and iterated numerical imputation)
      <li>Usual transformers (PowerTransformer)
      <li>Preprocessing pipeline</li></ul>
<br>
<li>Model development
  <ul>
    <li>LogisticRegression (baseline model)
    <li>Ensemble-learning (alternative model)
    <li>Models fitting and prediction
    <li>Basic model evaluation
    <li>Predicting probabilities</li>
  </ul>
<br>
<li>Model detailed evaluation
  <ul>
    <li>Classification report & confusion matrix
    <li>ROC-curve benchmark
    <li>Cross val scores
      <ul>
        <li>complete computation
        <li>general performance overview
        <li>segmented performance visualization</li></ul>
    </li></ul>
<br>
<li>Metric for the Business-team to monitor recipe popularity
<br><br>
<li>Conclusion</li>
</li></ol>

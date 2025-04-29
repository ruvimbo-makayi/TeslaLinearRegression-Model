<h1>Tesla Stock Time Series Linear Regression Model</h1>
<b/>
  
  - [Data Source: Kaggle](https://www.kaggle.com/datasets/simronw/tesla-stock-data-2024/data)

<h2>Project Overview</h2>
<p>This project focuses on building a Linear Regression model to predict the Adjusted Close price of Tesla stock using historical time series data from 2010 to 2024. The goal was to apply fundamental data analysis and machine learning techniques to create a simple, interpretable model capable of forecasting stock price movements based on past performance.</p>

<h2>Problem Statement</h2>
<p>The aim was to:</p>
<ul>
  <li>Understand Tesla stock trends using exploratory data analysis (EDA)</li>
  <li>Apply a 30-day rolling average for smoothing fluctuations</li>
  <li>Engineer lag features (e.g., Lag 1, Lag 3) to model the temporal dependency</li>
  <li>Build and evaluate a linear regression model</li>
  <li>Visualize how well the model predicts actual stock prices</li>
</ul>
<h2>Tools & Technologies used</h2>
<ul>
  <li><strong>Python</strong></li>
  <li><strong>Pandas</strong> – Data cleaning & transformation</li>
  <li><strong>Matplotlib & Seaborn</strong> – Data visualization</li>
  <li><strong>Scikit-learn</strong> – Model training and evaluation</li>
  <li><strong>Plotly Express</strong> – Interactive charts</li>
  <li><strong>Google Colab</strong> – Project development</li>
</ul>
<h2> Key Steps</h2>
  <ol>
    <li><strong>Data Preprocessing</strong>
      <ul>
        <li>Parsed and cleaned the dataset</li>
        <li>Set <code>Date</code> as the index</li>
        <li>Handled missing values and converted date types</li>
      </ul>
    </li>
    <li><strong>Feature Engineering</strong>
      <ul>
        <li>Created a 30-day rolling average column</li>
        <li>Generated lagged values of the <code>Adj Close</code> (Lag 1, Lag 3, etc.)</li>
        <li>Focused on predicting <code>Adj Close</code> using <code>Lag 1</code></li>
      </ul>
    </li>
    <li><strong>Modeling</strong>
      <ul>
        <li>Split data into training and test sets</li>
        <li>Built a <strong>Linear Regression</strong> model using <code>Lag 1</code> as the feature</li>
        <li>Calculated <strong>Mean Absolute Error (MAE)</strong> for training and testing sets</li>
        <li>Compared baseline MAE with model MAE</li>
      </ul>
    </li>
    <li><strong>Visualization</strong>
      <ul>
        <li>Created time series plots to show trends and rolling averages</li>
        <li>Plotted <code>Actual vs Predicted</code> prices using Plotly</li>
        <li>Evaluated model performance visually and statistically</li>
      </ul>
    </li>
  </ol>
  <h2>Results</h2>
  <ul>
    <li><strong>Baseline MAE (using mean as prediction):</strong> ~7.68</li>
    <li><strong>Linear Regression Test MAE:</strong> ~6.49 with Lag 1</li>
    <li>The model was able to <strong>closely follow actual price trends</strong>, especially in short-term predictions.</li>
  </ul>

  <h2>Conclusion</h2>
  <p>This project demonstrates that even a simple linear regression model, with thoughtful feature engineering, can produce <strong>strong predictive performance</strong> on stock data.</p>

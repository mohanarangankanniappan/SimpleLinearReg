<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Simple Linear Regression</title>
    <style>
        body {
            font-family: Arial, Helvetica, sans-serif;
            line-height: 1.6;
            margin: 40px;
            max-width: 900px;
        }
        h1, h2, h3 {
            color: #2c3e50;
        }
        hr {
            margin: 30px 0;
        }
        ul {
            margin-left: 20px;
        }
        figure {
            margin: 30px 0;
            text-align: center;
        }
        figcaption {
            font-size: 0.9em;
            color: #555;
            margin-top: 8px;
        }
        .equation {
            background: #f4f4f4;
            padding: 10px;
            font-family: "Courier New", monospace;
            text-align: center;
            margin: 15px 0;
        }
    </style>
</head>
<body>

<h1>📈 Simple Linear Regression</h1>
<h3>Theory and Mathematical Background</h3>

<hr>

<h2>Introduction</h2>
<p>
Simple Linear Regression is a supervised machine learning and statistical technique used to model
the relationship between one independent variable and one dependent variable.
</p>
<p>
It assumes that the relationship between the variables can be approximated using a straight line.
This method is widely used for prediction, trend analysis, and understanding variable influence.
</p>

<hr>

<h2>Linear Regression Model</h2>
<p>The mathematical form of Simple Linear Regression is:</p>

<div class="equation">
y = m x + c
</div>

<p><strong>Where:</strong></p>
<ul>
    <li><strong>x</strong> – Independent variable (input)</li>
    <li><strong>y</strong> – Dependent variable (output)</li>
    <li><strong>m</strong> – Slope of the regression line</li>
    <li><strong>c</strong> – Intercept of the regression line</li>
</ul>

<p>This equation represents a straight line that best fits the observed data.</p>

<hr>

<h2>Slope (m)</h2>
<p>
The slope represents the rate of change of the dependent variable with respect to the independent variable.
</p>

<p><strong>Interpretation:</strong></p>
<ul>
    <li>Positive slope → y increases as x increases</li>
    <li>Negative slope → y decreases as x increases</li>
    <li>Zero slope → y does not change with x</li>
</ul>

<p>
The magnitude of the slope indicates how strongly the independent variable influences the dependent variable.
</p>

<hr>

<h2>Intercept (c)</h2>
<p>
The intercept is the value of the dependent variable when the independent variable is zero.
</p>
<p>
It defines the point where the regression line crosses the y-axis and provides a baseline value for predictions.
</p>

<hr>

<h2>Mean of Variables</h2>
<p>The mean of the independent variable <strong>x</strong> is:</p>

<div class="equation">
x̄ = (x₁ + x₂ + … + xₙ) / n
</div>

<p>The mean of the dependent variable <strong>y</strong> is:</p>

<div class="equation">
ȳ = (y₁ + y₂ + … + yₙ) / n
</div>

<p>These mean values are used in computing the regression parameters.</p>

<hr>

<h2>Estimation of Slope (m)</h2>
<p>
The slope is computed using the Least Squares Method, which minimizes the sum of squared differences
between actual and predicted values.
</p>

<div class="equation">
m = Σ[(x − x̄)(y − ȳ)] / Σ[(x − x̄)²]
</div>

<p>
This formula ensures that the regression line is the best possible linear fit for the given data.
</p>

<hr>

<h2>Estimation of Intercept (c)</h2>
<p>Once the slope is calculated, the intercept is obtained using:</p>

<div class="equation">
c = ȳ − m x̄
</div>

<p>
This guarantees that the regression line passes through the mean point (x̄, ȳ).
</p>

<hr>

<h2>Prediction Using the Model</h2>
<p>Predicted values are computed using:</p>

<div class="equation">
ŷ = m x + c
</div>

<p>Where ŷ represents the predicted value of the dependent variable.</p>

<hr>

<h2>Residual Error</h2>
<p>
Residual error is the difference between the actual value and the predicted value.
</p>

<div class="equation">
e = y − ŷ
</div>

<p>
Residuals are used to evaluate the accuracy and goodness of fit of the regression model.
</p>

<hr>

<h2>Assumptions of Simple Linear Regression</h2>
<ul>
    <li><strong>Linearity</strong> – The relationship between x and y is linear</li>
    <li><strong>Independence</strong> – Observations are independent</li>
    <li><strong>Homoscedasticity</strong> – Constant variance of residuals</li>
    <li><strong>Normality</strong> – Residuals are normally distributed</li>
</ul>

<p>Violation of these assumptions may reduce model reliability.</p>

<hr>

<h2>Advantages</h2>
<ul>
    <li>Easy to understand and interpret</li>
    <li>Computationally efficient</li>
    <li>Works well for linearly related data</li>
    <li>Serves as a baseline model for advanced algorithms</li>
</ul>

<hr>

<h2>Applications</h2>
<ul>
    <li>Salary prediction based on experience</li>
    <li>Sales and demand forecasting</li>
    <li>House price estimation</li>
    <li>Financial trend analysis</li>
    <li>Economic modeling</li>
</ul>

<hr>

<h2>Results</h2>

<figure>
    <img src="https://github.com/user-attachments/assets/da25c4ee-b339-4b26-87c7-5c6f466bf340"
         width="640" height="480" alt="Input Data">
    <figcaption>Figure 1: Input Data Distribution</figcaption>
</figure>

<figure>
    <img src="https://github.com/user-attachments/assets/206b7151-ef6e-4122-a598-ca51aeaa5016"
         width="640" height="480" alt="Regression Line">
    <figcaption>Figure 2: Fitted Regression Line</figcaption>
</figure>

<figure>
    <img src="https://github.com/user-attachments/assets/81900947-176d-40b7-8f06-b400f4efd548"
         width="640" height="480" alt="Actual vs Predicted">
    <figcaption>Figure 3: Actual vs Predicted Values</figcaption>
</figure>

<figure>
    <img src="https://github.com/user-attachments/assets/e88027ef-c603-4a4a-a682-d482b968b3bd"
         width="640" height="480" alt="Residual Error">
    <figcaption>Figure 4: Residual Error Plot</figcaption>
</figure>

<hr>

<h2>Conclusion</h2>
<p>
Simple Linear Regression is a fundamental technique in machine learning and data analysis.
Despite its simplicity, it provides valuable insights into data relationships and forms the
foundation for more advanced predictive models.
</p>

</body>
</html>

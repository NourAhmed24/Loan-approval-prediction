<!DOCTYPE html><html lang="en">


<body>
    <div class="readme-container">
        <h1>Loan Approval Prediction using Machine Learning 🏦</h1>

<p>This repository presents a machine learning solution to predict the likelihood of a loan application being approved. The goal is to provide financial institutions with an automated, data-driven tool to streamline the decision-making process.</p>
        
  <hr>
   <h2>🎯 Project Goal</h2>
        <p>The core objective is to develop a <strong>robust classification model</strong> that can accurately predict the target variable, <strong><code>Loan_Status</code> (Y/N)</strong>, based on applicant features.</p>
        
<hr>

<h2>💾 Dataset & Data Snapshot</h2>

<p>The analysis is performed on the provided file, <strong><code>LoanApprovalPrediction.csv</code></strong>.</p>
        
<h3>Key Data Insights 💡</h3>
        <ul>
            <li><strong>Total Records:</strong> 598 loan applications.</li>
            <li><strong>Missing Data:</strong> Null values are present in several critical columns, including <code>Dependents</code>, <code>LoanAmount</code>, <code>Loan_Amount_Term</code>, and <code>Credit_History</code>. Data imputation will be a necessary preprocessing step.</li>
            <li><strong>Credit History:</strong> The mean value for <code>Credit_History</code> is 0.843, suggesting a majority of applicants meet the credit guidelines.</li>
        </ul>
    <h3>Feature Columns 📊</h3>
        <table>
            <thead>
                <tr>
                    <th>Feature Name</th>
                    <th>Description</th>
                    <th>Data Type/Range</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td><code>Loan_ID</code></td>
                    <td>Unique identifier.</td>
                    <td>Categorical (String)</td>
                </tr>
                <tr>
                    <td><strong><code>Loan_Status</code></strong></td>
                    <td><strong>Target Variable: Y (Approved) / N (Rejected)</strong>.</td>
                    <td>Categorical</td>
                </tr>
                <tr>
                    <td><code>ApplicantIncome</code></td>
                    <td>Applicant's monthly income.</td>
                    <td>Numerical (Min: 150, Max: 81000)</td>
                </tr>
                <tr>
                    <td><code>CoapplicantIncome</code></td>
                    <td>Co-applicant's monthly income.</td>
                    <td>Numerical</td>
                </tr>
                <tr>
                    <td><code>LoanAmount</code></td>
                    <td>Loan amount in thousands.</td>
                    <td>Numerical</td>
                </tr>
                <tr>
                    <td><code>Credit_History</code></td>
                    <td>Applicant's credit score history (1.0 or 0.0).</td>
                    <td>Binary/Numerical</td>
                </tr>
                <tr>
                    <td><code>Gender</code>, <code>Married</code>, etc.</td>
                    <td>Demographic and property information.</td>
                    <td>Categorical</td>
                </tr>
            </tbody>
        </table>

 <hr>

 <h2>🛠️ Methodology & Models</h2>

<p>The analysis notebook (<code>LoanApproval.ipynb</code>) follows a standard Machine Learning pipeline:</p>
        <ul>
            <li><strong>Exploratory Data Analysis (EDA):</strong> Using <code>matplotlib</code> and <code>seaborn</code> to understand distributions and relationships.</li>
            <li><strong>Data Preprocessing:</strong> Handling missing values and preparing categorical features. <strong>Feature Scaling</strong> (<code>StandardScaler</code>) is utilized to normalize numerical features.</li>
            <li><strong>Model Training:</strong> The project employs two popular classification algorithms:
                <ul>
                    <li><strong>Logistic Regression</strong></li>
                    <li><strong>Random Forest Classifier</strong></li>
                </ul>
            </li>
            <li><strong>Evaluation:</strong> Models are evaluated using standard metrics, including <strong><code>accuracy_score</code></strong>, <strong><code>confusion_matrix</code></strong>, and <strong><code>classification_report</code></strong>.</li>
        </ul>

<hr>
     <h2>📁 File Structure</h2>

 <pre>
loan-approval-prediction/
├── LoanApproval.ipynb      # 👈 The primary Jupyter Notebook for analysis and modeling
├── LoanApprovalPrediction.csv # 👈 The raw loan application dataset
└── README.md               # This file
        </pre>
        
 <hr>
        
<h2>🚀 Getting Started</h2>

 <p>To replicate this analysis:</p>
        <ol>
            <li>Clone the repository.</li>
            <li>Ensure you have the Python dependencies (pandas, numpy, sklearn, etc.) installed.</li>
            <li>Execute the cells in the <strong><code>LoanApproval.ipynb</code></strong> notebook sequentially to perform the data cleaning, modeling, and evaluation.</li>
        </ol>

 </div>
</body>
</html>

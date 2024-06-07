# Finac-Plus-project
Financial Statement Table Classification Report
The goal of this project was to develop a machine learning model to classify tables from financial statements into predefined categories. The categories include Income Statements, Balance Sheets, Cash Flows, Notes, and Others. The project aimed to automate the process of categorizing financial tables, which is a crucial step in financial analysis and reporting.
Data Collection and Preprocessing
The dataset consisted of HTML files containing financial tables.
BeautifulSoup library was used to extract text from HTML files.
The text data was cleaned and preprocessed to remove HTML tags, special characters, and stopwords.
The preprocessed data was then converted into numerical features using TF-IDF vectorization.
3. Model Selection and Training
Three classification models were evaluated:

Logistic Regression: Simple and interpretable model, but may be limited in complex relationships.
Random Forest: Ensemble model that can handle non-linear relationships and high-dimensional data.
Support Vector Classifier (SVC): Effective for high-dimensional data, especially with non-linear decision boundaries.
The dataset was split into training and testing sets (80-20 split). Each model was trained on the training set and evaluated on the test set using accuracy and the classification report (precision, recall, F1-score) for each category.

4. Results
Logistic Regression:

Accuracy: 92.48%
Notable performance: Balance Sheets (precision: 0.98, recall: 0.96, F1-score: 0.97)
Challenges: Notes category (precision: 0.89, recall: 0.88, F1-score: 0.88)
Random Forest:

Accuracy: 94.46%
Notable performance: Cash Flow (precision: 1.00, recall: 0.83, F1-score: 0.91)
Challenges: Notes category (precision: 0.93, recall: 0.91, F1-score: 0.92)
Support Vector Classifier:

Accuracy: 94.65%
Notable performance: Cash Flow (precision: 1.00, recall: 1.00, F1-score: 1.00)
Challenges: Notes category (precision: 0.94, recall: 0.89, F1-score: 0.92)
5. Model Comparison and Analysis
Support Vector Classifier outperformed the other models with the highest accuracy and F1-scores.
Random Forest showed competitive performance, especially in the Cash Flow category.
Logistic Regression performed well but showed limitations in handling complex relationships, especially in the Notes category.
6. Future Improvements
Ensemble Methods: Explore ensemble methods like Voting or Stacking to combine the strengths of multiple models.
Feature Engineering: Experiment with advanced text preprocessing techniques and feature engineering to improve model performance.
Hyperparameter Tuning: Further tune the hyperparameters of the models to achieve better results.
Cross-validation: Use cross-validation to ensure the models' robustness and generalizability.
7. Conclusion
The project successfully developed machine learning models to classify financial statement tables into predefined categories.
The Support Vector Classifier demonstrated the highest accuracy and F1-scores, indicating its effectiveness for this task.
Further refinement and optimization of the models could lead to even better classification performance.






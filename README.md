🎓 Placement Prediction using Logistic Regression

A simple machine learning project that predicts whether a student will be placed or not placed based on their CGPA and IQ, using Logistic Regression.

📌 Overview

This project walks through a complete, beginner-friendly ML pipeline:

Load and clean the dataset
Visualize the data
Split into training and testing sets
Scale the features
Train a Logistic Regression model
Evaluate accuracy
Visualize the decision boundary
📂 Dataset

The dataset (placement.csv) contains 100 student records with the following columns:

Column	Description
cgpa	Student's CGPA (Cumulative GPA)
iq	Student's IQ score
placement	Target label — 1 = Placed, 0 = Not Placed

An extra unnamed index column from the original export is dropped during preprocessing.

🛠️ Tech Stack
Python 3
NumPy & Pandas – data handling
Matplotlib – data visualization
Scikit-learn – train/test split, scaling, logistic regression, accuracy metrics
mlxtend – decision boundary plotting
🚀 Project Workflow
1. Data Preprocessing
Load placement.csv with pandas
Inspect shape and structure with .head(), .shape(), .info()
Drop the unnecessary Unnamed: 0 index column
2. Data Visualization
Scatter plot of cgpa vs iq
Colored scatter plot showing placement outcome (0 → not placed, 1 → placed)
3. Train-Test Split
Features (x): cgpa, iq
Target (y): placement
Split using train_test_split (90% train / 10% test)
4. Feature Scaling
Standardized features using StandardScaler to bring cgpa and iq to the same scale
5. Model Training
Trained a LogisticRegression model on the scaled training data
6. Evaluation
Generated predictions on the test set
Measured performance using accuracy_score
7. Decision Boundary Visualization
Plotted the model's decision boundary using mlxtend.plotting.plot_decision_regions
📊 Results

The Logistic Regression model achieved strong accuracy on the test split, cleanly separating placed vs. non-placed students based on CGPA and IQ. The decision boundary plot visually confirms the model's classification regions.

Note: The test set is small (10 samples), so accuracy may vary between runs depending on the random train/test split.

📁 Project Structure
├── ml_project.ipynb    # Jupyter notebook with the full ML pipeline
├── placement.csv        # Dataset used for training/testing
└── README.md             # Project documentation
▶️ How to Run
Clone the repository
bash
   git clone <your-repo-url>
   cd <your-repo-folder>
Install dependencies
bash
   pip install numpy pandas matplotlib scikit-learn mlxtend
Run the notebook
bash
   jupyter notebook ml_project.ipynb
Run all cells from top to bottom to reproduce preprocessing, training, and evaluation.
🔮 Future Improvements
Add more features beyond CGPA and IQ (e.g., communication skills, internships, projects)
Try other classification algorithms (KNN, SVM, Random Forest) and compare performance
Use cross-validation instead of a single train/test split for a more robust accuracy estimate
Deploy the model as a simple web app (e.g., using Streamlit or Flask)
🙋 Author

Feel free to connect, fork this project, or suggest improvements via pull requests!

📜 License

This project is open-source and available under the MIT License.

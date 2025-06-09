Overview
Legal Guru is a prototype AI-powered system designed to help legal professionals predict case outcomes. The system analyzes case documents or manually entered case details, compares them with historical cases, and provides predictions, evidence trails, and strategic recommendations. This enhanced version integrates the European Court of Human Rights (ECHR) dataset for improved predictions and specialized handling of human rights cases.

Features
Document Upload: Upload legal case documents (PDF, DOCX, TXT) for analysis
Manual Case Entry: Enter case details through a structured form
Case Analysis: AI-powered analysis of case details
Outcome Prediction: Prediction of case outcomes with confidence levels
Similar Case Identification: Finding and displaying similar historical cases
Strategic Recommendations: AI-generated strategic suggestions
Risk Assessment: Identification of potential risk factors
ECHR Dataset Integration: Access to European Court of Human Rights cases
Machine Learning Model: Trained model for predicting case outcomes based on ECHR data
Human Rights Specialization: Special handling for human rights cases with ECHR article references
Project Structure
Legal_guruV2/
├── backend/            # Flask backend API
│   └── app.py          # Main backend application
├── frontend/           # React frontend application
│   ├── public/         # Public assets
│   └── src/            # React source code
│       ├── components/ # Reusable UI components
│       └── pages/      # Application pages
├── data/               # Data storage
│   ├── uploads/        # Uploaded documents
│   ├── processed/      # Processed case data
│   └── sample_documents/ # Sample documents for testing
├── models/             # Machine learning models
│   ├── echr_dataset.py # ECHR dataset loader and processor
│   ├── prediction_model.py # ML model for case prediction
│   └── __init__.py     # Package initialization
└── run.bat             # Script to run both frontend and backend
Technologies Used
Frontend: React, Material-UI, Chart.js
Backend: Flask, NLTK, scikit-learn
Document Processing: PyPDF2, python-docx
Data Storage: Local file system (JSON)
Machine Learning: Random Forest, TF-IDF Vectorization
Dataset: Hugging Face ECHR dataset (AUEB-NLP/ecthr_cases)
Setup Instructions
Prerequisites
Python 3.8+ installed
Node.js and npm installed
Git (optional)
Backend Setup
Navigate to the project directory:

cd Legal_guruV2
Install Python dependencies:

pip install -r requirements.txt
Frontend Setup
Navigate to the frontend directory:

cd Legal_guruV2/frontend
Install Node.js dependencies:

npm install
Running the Application
Option 1: Using the run script
Simply double-click the run.bat file or run it from the command line:

run.bat
This will start both the backend and frontend servers.

Option 2: Manual startup
Start the backend server:

cd backend
python app.py
In a separate terminal, start the frontend server:

cd frontend
npm start
Access the application at http://localhost:3000

Usage Guide
Uploading a Document
Click on "Upload Case" in the navigation menu
Drag and drop your document or click to browse files
Select a PDF, DOCX, or TXT file
Click "Upload and Analyze"
Wait for the analysis to complete
View the prediction results on the dashboard
Entering Case Details Manually
Click on "Enter Case Details" in the navigation menu
Fill in the required fields in the form
For human rights cases, select "Human Rights" as the case type or "ECHR (European Court of Human Rights)" as the jurisdiction
When ECHR is selected, enter the relevant ECHR articles in the additional field that appears
Click "Submit and Analyze"
Wait for the analysis to complete
View the prediction results on the dashboard
Interpreting Results
Outcome Prediction: Shows the predicted outcome with win probability
Key Factors: Displays factors that influence the case outcome
Similar Cases: Shows historical cases similar to yours, including ECHR cases when relevant
ECHR Articles: For human rights cases, displays the relevant ECHR articles
Violation Status: For ECHR cases, shows whether a violation was found or not
Strategic Recommendations: Provides suggestions for case strategy
Risk Factors: Highlights potential risks to be aware of
Sample Documents
A sample case document is included in the data/sample_documents directory for testing purposes.

Notes
This is a prototype system for demonstration purposes only
All data is stored locally on your PC
No real machine learning model is implemented; predictions are based on simplified similarity algorithms
Hackathon Project
This project was created as a prototype for a hackathon and is not intended for production use.

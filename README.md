# Insurance Cross Sell Prediction 🏠🏥
[![GitHub](https://img.shields.io/badge/GitHub-code-blue?style=flat&logo=github&logoColor=white&color=red)](https://github.com/prsdm/mlops-project) [![Medium](https://img.shields.io/badge/Medium-view_article-green?style=flat&logo=medium&logoColor=white&color=green)](https://medium.com/@prasadmahamulkar/machine-learning-operations-mlops-for-beginners-a5686bfe02b2)

Welcome to the Insurance Cross-Selling Prediction project! The goal of this project is to predict which customers are most likely to purchase additional insurance products using a machine learning model.

---

## 📊 Diagram
Below is the architecture diagram that illustrates the flow of the project from data ingestion to model deployment:

![Image](docs/mlops.jpg)

---

## 🚀 Get Started
To get started with the project, follow the steps below:

---

### 🔧 1. Clone the Repository
Clone the project repository from GitHub:
\`\`\`bash
git clone https://github.com/Hari927/Insurance-Cross-Sell-Prediction-mlops-project.git
cd ml-project
\`\`\`

---

### 📦 2. Set Up the Environment
Ensure you have Python 3.8+ installed. Create a virtual environment and install the necessary dependencies:
\`\`\`bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt
\`\`\`

Alternatively, use the Makefile command:
\`\`\`bash
make setup
\`\`\`

---

### 📁 3. Data Preparation
Pull the data using DVC. If DVC doesn't work, training and testing data should already be present in the \`data\` folder:
\`\`\`bash
dvc pull
\`\`\`

---

### 🧠 4. Train the Model
To train the machine learning model, execute:
\`\`\`bash
python main.py
\`\`\`

Or use:
\`\`\`bash
make run
\`\`\`

This script will load, preprocess, train, and save the model in the \`models/\` directory.

---

### ⚙️ 5. Start FastAPI
To run the FastAPI server:
\`\`\`bash
uvicorn app:app --reload
\`\`\`

---

### 🐳 6. Docker Deployment
To build and deploy using Docker:
\`\`\`bash
docker build -t my_fastapi .
docker run -p 80:80 my_fastapi
\`\`\`

Once built, you can push the image to Docker Hub for cloud deployment.

---

### 📈 7. Monitor the Model
Use Evidently AI to monitor model performance and data drift:

\`\`\`bash
jupyter notebook monitor.ipynb
\`\`\`

---

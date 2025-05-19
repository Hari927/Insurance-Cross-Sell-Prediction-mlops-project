# Insurance Cross Sell Prediction 🏠🏥
[![GitHub](https://img.shields.io/badge/GitHub-code-blue?style=flat&logo=github&logoColor=white&color=red)](https://github.com/Hari927/Insurance-Cross-Sell-Prediction-mlops-project)  


Welcome to the **Insurance Cross-Selling Prediction** project!  
This project aims to identify customers most likely to purchase additional insurance products using a machine learning pipeline and modern MLOps practices.

---

## 📊 Architecture Diagram

The diagram below represents the flow from data ingestion to model deployment and monitoring:

![image](https://github.com/user-attachments/assets/6a371204-abe4-4290-9637-f1f874406403)


---

## 🚀 Get Started

Follow these steps to set up and run the project locally:

---

### 🔧 1. Clone the Repository

```bash
git clone https://github.com/Hari927/Insurance-Cross-Sell-Prediction-mlops-project.git
cd Insurance-Cross-Sell-Prediction-mlops-project
```

---

### 📦 2. Set Up the Environment

Ensure Python 3.8+ is installed. Then run:

```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt
```

Or use Makefile:

```bash
make setup
```

---

### 📁 3. Data Preparation

If DVC is configured, pull the data:

```bash
dvc pull
```

> ✅ If DVC is not set up, data files should already exist in the `data/` folder.

---

### 🧠 4. Train the Model

Run the training script:

```bash
python main.py
```

Or use:

```bash
make run
```

The trained model will be saved in the `models/` directory.

---

### ⚙️ 5. Start FastAPI

To serve the model using FastAPI:

```bash
uvicorn app:app --reload
```

Visit: [http://127.0.0.1:8000/docs](http://127.0.0.1:8000/docs)

---

### 🐳 6. Docker Deployment

Build and run using Docker:

```bash
docker build -t my_fastapi .
docker run -p 80:80 my_fastapi
```

> ☁️ You can optionally push your image to Docker Hub for deployment.

---

### 📈 7. Monitor the Model

Monitor model performance and data drift with **Evidently AI**:

```bash
jupyter notebook monitor.ipynb
```

---

## 🧰 Tech Stack

- Python 3.8+
- Scikit-learn
- FastAPI
- Docker
- DVC
- Evidently AI
- Uvicorn

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

## 👤 Contact

Created by [**@Hari927**](https://github.com/Hari927) – feel free to connect or open issues!

---

⭐ Star this repo if you found it helpful!

# CyberSentryML — AI-Powered Phishing URL Detection System

CyberSentryML is a cutting-edge AI-based phishing website detection system designed to protect users from fraudulent online attacks. Leveraging advanced deep learning models, including Convolutional Neural Networks (CNNs), this project achieves **99.2% accuracy** in distinguishing phishing URLs from legitimate ones.

---

##  Project Goal

Phishing attacks are a rapidly evolving cybersecurity threat that bypass traditional rule-based detection. CyberSentryML aims to provide a robust, scalable AI solution to identify phishing websites through intelligent feature extraction and deep learning classification.

---

##  Data Collection & Preparation

- **Phishing URLs:** Collected from [PhishTank](https://www.phishtank.com/developer_info.php), a community-driven platform providing up-to-date phishing data.
- **Legitimate URLs:** Sourced from a balanced Kaggle dataset and supplemented by research datasets (CyberSA 2021).
- Extensive feature engineering extracted URL components such as domain info, address bar features, HTML tags, and JavaScript behavior indicators.
- Features are encoded for classification as phishing or legitimate, detailed in `Phishing Website Features.docx`.
- Data exploration and visualization performed using Python libraries like matplotlib and scikit-learn, with results documented in `Phishing Website Detection Deep Learning.ipynb`.

---

## ⚙ Model Development

- Explored multiple models: SVM, Multilayer Perceptron (MLP), Autoencoder, CNN, and RNN.
- The **MLP model** delivered the best balance of accuracy and inference speed.
- Trained using PyTorch and TensorFlow frameworks.
- Model persistence handled via Python’s pickle module (`phish_classifier.pkl`).

---

##  Results

- Achieved **99.2% classification accuracy** on the test dataset.
- Demonstrated strong generalization in identifying previously unseen phishing URLs.
- Validated effectiveness via performance metrics and confusion matrix visualizations.

---

##  Technologies Used

- **Programming Languages:** Python, JavaScript, HTML/CSS  
- **ML Frameworks:** PyTorch, TensorFlow  
- **Data Processing:** pandas, numpy, scikit-learn  
- **Web & API:** FastAPI for backend serving  
- **Other Libraries:** BeautifulSoup4, python-whois, googlesearch  

---
## Demo: User Interface & URL Detection

### 1. Landing Page - URL Input

This is the index.html interface where users can enter any URL they want to check for phishing.

![Landing Page - URL Input]<img width="937" alt="image" src="https://github.com/user-attachments/assets/d4156f33-57b7-4164-93b5-e297e7a8c2d2" />


---

### 2. Detection Result

After entering a URL, the system analyzes and shows whether the URL is **Legitimate** or **Phishing**.

![URL Detection Result]![WhatsApp Image 2025-07-08 at 18 06 32_4bf339fe](https://github.com/user-attachments/assets/811383ba-a81e-4940-b4c8-3df5b2b0c4ee)


---

## Future Directions

- Develop a browser extension for real-time phishing alerts.
- Integrate with internet security tools for broader user protection.
- Explore deployment on cloud platforms for public access and scalability.

---

## How to Run

1. Clone the repo:
git clone https://github.com/yourusername/CyberSentryML.git
2. Install dependencies:
pip install -r requirements.txt
3. Explore the Jupyter Notebook for model insights:
Phishing Website Detection Deep Learning.ipynb
4. Run the FastAPI server to test the detection UI locally:
uvicorn app:app --reload

---

## About Me

Sravani Elavarthi
-


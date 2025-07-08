# CyberSentry

CyberSentryML is an AI-powered phishing detection system leveraging deep learning to identify fraudulent websites with 99.2% accuracy. By combining cybersecurity and artificial intelligence, this project aims to protect users from online fraud and phishing attacks through advanced pattern recognition and feature analysis.

## Objective
Phishing websites pose a significant cybersecurity threat, evolving rapidly to evade traditional detection methods. CyberSentryML uses deep learning techniques, including Convolutional Neural Networks (CNNs), to detect phishing sites effectively. This project merges Python, JavaScript, HTML/CSS, and AI to deliver a practical solution for enhancing online security.

## Key Achievement
- Designed an AI-powered phishing detection system using Machine Learning, PyTorch, TensorFlow, and FastAPI, resulting in a 99.2% accuracy in identifying phishing attempts.

## Data Collection
To train the deep learning model, we curated a balanced dataset of legitimate and phishing URLs:

- **Phishing URLs**: Sourced from [PhishTank](https://www.phishtank.com/developer_info.php), providing periodically updated phishing URLs in CSV, XML, JSON, and PHP formats.
- **Legitimate URLs**: Obtained from a balanced Kaggle dataset ([Web Page Phishing Detection Dataset](https://www.kaggle.com/datasets/shashwatwork/web-page-phishing-detection-dataset)) and supplemented by the dataset from P. Mowar and M. Jain's paper, ["Fishing out the Phishing Websites"](https://zenodo.org/records/5807622#.Ycsbzy0RpQJ), published in CyberSA 2021.

## Feature Engineering
We extracted domain-based, address bar, HTML, and JavaScript features from the URLs, as detailed in `Phishing Website Features.docx`. Features were encoded as -1 (legitimate) or 1 (phishing) using the `Feature_Extraction.py` script. The resulting dataset is available in `url_features.csv`.

Visualizations to explore data relationships and correlations were implemented using Python's sklearn and matplotlib libraries, available in `Phishing Website Detection Deep Learning.ipynb`.

## Model Development
The following deep learning algorithms were evaluated:

- Support Vector Machines
- Multilayer Perceptrons (MLP)
- Autoencoder Neural Network
- Convolutional Neural Network (CNN)
- Recurrent Neural Network (RNN)

The Multilayer Perceptrons (MLP) model outperformed others in accuracy and testing speed. The complete training and analysis code is in `Phishing Website Detection Deep Learning.ipynb`.

## Results
The final MLP classifier achieved a 99.2% accuracy and was saved using Python's pickle module as `phish_classifier.pkl`.

## Future Work
The model holds potential for real-world applications, such as:
- Developing a browser extension using JavaScript and HTML/CSS.
- Integrating with internet security providers to proactively alert users against phishing threats.



**Python Packages**:
- sklearn
- numpy
- pandas
- pickle
- matplotlib
- python-whois
- tensorflow
- BeautifulSoup4
- googlesearch

## Technologies
- **Python**: Core development and model training.
- **JavaScript & HTML/CSS**: Browser extension prototype (`popup.js`, `popup.html`, `popup.css`).
- **Deep Learning & CNNs**: Model development using TensorFlow and PyTorch.
- **Artificial Intelligence**: Powers phishing detection logic.
- **Security**: Focus on cybersecurity threat mitigation.

## Getting Started
1. Clone the repository:
Install dependencies:pip install -r requirements.txt


Explore the Jupyter notebook (Phishing Website Detection Deep Learning.ipynb) for model training and analysis.
Test the browser extension by loading the manifest.json and related files in a browser.

About
CyberSentryML combines AI and cybersecurity to combat phishing attacks, showcasing the power of deep learning in real-world security applications.

Topics: python, javascript, html, css, deep-learning, cnns, artificial-intelligence, security```

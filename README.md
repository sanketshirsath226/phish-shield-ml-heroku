# Phish-Shield - Machine Learning

Phish-Shield is a backend project that aims to provide protection against phishing attacks. It utilizes various methods, including blacklisting, a famous website dataset, an API, and feature extraction with an SVM (Support Vector Machine) model, to identify and prevent phishing attempts.


## Features

* Blacklisting: Phish-Shield maintains a blacklist of known phishing websites. When a user accesses a URL, it checks against the blacklist to determine if it is a known phishing site.
* Famous Website Dataset: Phish-Shield also leverages a dataset of famous websites to compare and validate the authenticity of a given URL.
* API Integration: The project integrates with an API service that provides additional information about a website, such as its reputation, domain age, and SSL certificate status. This helps in determining the likelihood of the website being legitimate or phishing.
* Feature Extraction with SVM Model: Phish-Shield extracts relevant features from a URL and utilizes a trained SVM model to classify the URL as either legitimate or phishing. The SVM model uses machine learning techniques to identify patterns and make accurate predictions.

## Technologies Used
1. Python: The programming language used for the backend development of Phish-Shield.
2. Flask: A lightweight web framework for Python used to create the backend API endpoints and handle HTTP requests.
3. Scikit-learn: A machine learning library in Python that includes the SVM model for classification tasks.
4. SQLite: A relational database used to store the blacklist of known phishing websites.
5. API: Integration with an external API service for retrieving additional information about a website.
6. Feature Extraction: Techniques such as analyzing URL structure, domain age, SSL certificate status, and other relevant features to classify URLs.

## Installation
To set up and run the Phish-Shield backend locally, follow these steps:

1. Clone the repository: git clone https://github.com/sanketshirsath226/phish-shield-ml-heroku.git
2. Navigate to the project directory: cd phish-shield
3. Create a virtual environment (optional but recommended): python3 -m venv env (replace env with your desired environment name).
4. Activate the virtual environment:
= For Windows: .\env\Scripts\activate
- For macOS/Linux: source env/bin/activate
5. Install the dependencies: pip install -r requirements.txt
6. Set up the required configuration:
- Rename .env.example to .env.
- Update the necessary configuration variables in the .env file, such as API keys or database information.
7. Run the application: python app.py
8. The Phish-Shield backend will start running on http://localhost:5000.

## License
This project is licensed under the MIT License. You can find the details in the LICENSE file.

## Acknowledgments
Phish-Shield is developed with the goal of enhancing online security and protecting users from phishing attacks. It leverages various techniques and technologies to provide accurate phishing detection. Contributions from the open-source community are crucial in improving the project's effectiveness and ensuring the safety of users online.

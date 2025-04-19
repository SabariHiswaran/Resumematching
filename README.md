# 🧠 Resume Matcher Web App

This is a smart **Resume vs Job Description Matcher** web application built with **Flask**, **spaCy**, **scikit-learn**, and **NLTK**. The app analyzes a `.docx` resume against a pasted job description, extracts and compares technical keywords, and calculates a **match score** using **cosine similarity**. It also highlights matched and unmatched keywords for better clarity.

---

## 🚀 Features

- 🔍 Extracts key **technical terms** from job descriptions and resumes
- 🤖 Uses **NLP (spaCy)** for chunking & named entity recognition
- 📊 Calculates a **match percentage** using cosine similarity
- ✨ Highlights **matched** and **unmatched** terms visually
- 🌗 Includes **Dark Mode** for better UX
- 📄 Accepts `.docx` resume file uploads

---

## 🛠️ Tech Stack

- Backend: [Python](https://www.python.org/), [Flask](https://flask.palletsprojects.com/)
- NLP: [spaCy](https://spacy.io/), [NLTK](https://www.nltk.org/)
- ML: [scikit-learn](https://scikit-learn.org/)
- Frontend: [HTML5](https://developer.mozilla.org/en-US/docs/Web/Guide/HTML/HTML5), [Bootstrap 5](https://getbootstrap.com/)

---

## 📸 Screenshots

| Upload & Paste JD | Results Page |
|-------------------|--------------|
| ![Upload Screenshot](screenshots/upload.png) | ![Result Screenshot](screenshots/result.png) |

---

## ⚙️ Installation

1. **Clone the repository**
git clone https://github.com/yourusername/resume-matcher.git
cd resume-matcher

2. **Create a virtual environment**

python -m venv venv
source venv/bin/activate   # On Windows use: venv\Scripts\activate

3. **Install dependencies**
pip install -r requirements.txt


4. **Download spacy model**
python -m spacy download en_core_web_sm


5. **Run the app**
python app.py

6. **Visit the browser**
http://127.0.0.1:5000/

## 📂 Project Structure
resume-matcher/
│
├── app.py                  # Flask app
├── requirements.txt        # Dependencies
├── templates/
│   ├── index.html
│   └── result.html
├── static/                 # Optional: CSS or JS files
├── screenshots/            # Optional: Add images for README
└── README.md

## 🧠 How It Works
User uploads a .docx resume and pastes a job description.

App uses NLP and a custom tech keyword list to extract meaningful keywords.

Cosine similarity is calculated between resume and JD keyword vector.

Score is shown with highlighted matches and misses.


## 📌 Customization
You can update the core technical keyword list in app.py under:

python:

TECH_KEYWORDS = {
    'python', 'etl', 'ab initio', 'data modeling', ...
}
You can also tweak logic to include or exclude specific roles, phrases, or technologies.

## 🤝 Contributing
Contributions, issues and feature requests are welcome! Feel free to fork this project and submit a PR.

## 📄 License
This project is licensed under the MIT License.

## 🙌 Acknowledgements
spaCy

NLTK

scikit-learn

Bootstrap

docx2txt

## 💡 Future Enhancements
PDF resume support

Keyword category breakdown

Multi-language support

Upload JD as a file





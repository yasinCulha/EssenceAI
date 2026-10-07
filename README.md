# EssenceAI

EssenceAI is a Django-based perfume recommendation web application. It uses perfume note data to suggest similar fragrances with a content-based recommendation approach.

The project combines a Python data processing workflow with a simple web interface. Perfume notes are prepared as text data, converted into numerical vectors with TF-IDF, and compared with cosine similarity to find close alternatives.

## Features

- Recommends similar perfumes based on selected fragrance data
- Uses perfume notes and character information as recommendation input
- Processes Excel-based perfume datasets with Pandas
- Builds a similarity model with Scikit-learn
- Serves recommendations through a Django web application
- Provides a simple user interface for selecting a perfume and viewing suggestions

## Technologies Used

- Python
- Django
- Pandas
- NumPy
- Scikit-learn
- TF-IDF Vectorizer
- Cosine Similarity
- OpenPyXL
- HTML and CSS

## How It Works

1. Perfume data is read from an Excel file.
2. Top notes, middle notes, base notes, and general character values are combined into one text field.
3. TF-IDF converts the text data into numerical vectors.
4. Cosine similarity compares perfumes based on those vectors.
5. The generated similarity model is saved and used by the Django application.
6. When the user selects a perfume, the application returns the closest recommendations.

## Project Structure

```text
EssenceAI/
├── ai_engine/
│   ├── data/
│   │   └── egitim.xlsx
│   └── notebooks/
│       └── train.py
├── web_app/
│   ├── EssenceAI/
│   ├── recommender/
│   ├── data/
│   │   └── database.xlsx
│   └── manage.py
├── requirements.txt
└── README.md
```

## Installation

Clone the repository:

```bash
git clone https://github.com/yasinCulha/EssenceAI.git
cd EssenceAI
```

Create and activate a virtual environment:

```bash
python -m venv .venv
```

Windows:

```bash
.venv\Scripts\activate
```

macOS / Linux:

```bash
source .venv/bin/activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

## Running the Project

Go to the Django application folder:

```bash
cd web_app
```

Run database migrations:

```bash
python manage.py migrate
```

Start the development server:

```bash
python manage.py runserver
```

Then open the local development address shown in the terminal, usually:

```text
http://127.0.0.1:8000/
```

## Model Training

The recommendation model is created in:

```text
ai_engine/notebooks/train.py
```

This script reads the training data, creates a similarity matrix, and exports the model files. The Django application then uses the saved model and perfume list to generate recommendations.

## Portfolio Notes

This project is useful as a portfolio example because it shows:

- Python data processing
- Use of external libraries
- A basic machine learning recommendation approach
- Integration between a trained model and a web application
- Django views, URLs, templates, and project structure

## Disclaimer

This project is intended for educational and portfolio purposes. The recommendations are based on similarity between available perfume note data and should not be treated as professional fragrance advice.

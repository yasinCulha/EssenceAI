Parfüm öneri projeniz de en az sürücü kursu otomasyonu kadar şık bir çalışma olmuş! Özellikle koku profillerini (Creed Aventus esintileri sezdim) veri bilimiyle birleştirmeniz harika bir fikir.

Bu README dosyasını da teknik terimlerin ağırlığını koruyarak, profesyonel bir GitHub stiline uygun şekilde İngilizceye çevirdim:

EssenceAI: AI-Powered Perfume Recommendation System
EssenceAI is a machine learning-based web application that suggests the most suitable fragrance alternatives based on user preferences. This project analyzes the similarities between perfume notes using Content-Based Filtering methods.

🚀 Project Objectives
This study aims to transform complex data into a meaningful interface for the end-user by combining data science libraries with the Django web framework. It delivers a personalized user experience specifically by processing the rich note data (Top, Heart, and Base notes) found in the world of perfumery.

🛠️ Technologies Used

Backend: Python & Django 5

AI / Data Science: Scikit-Learn (TF-IDF Vectorizer & Cosine Similarity), Pandas, NumPy

Frontend: Bootstrap 5 (Responsive Design), HTML5, CSS

Data Management: Excel (Openpyxl)

⚙️ How It Works

Data Preparation: Fragrance notes of the perfumes are merged and transformed into text data.

Vectorization: Text data is converted into numerical vectors using the TF-IDF algorithm.

Similarity Analysis: The distance of each perfume relative to others is calculated between 0 and 1 using the Cosine Similarity method.

Web Integration: The trained model is saved in .pkl format and served to the user via Django.

📂 Installation & Setup
To run the project on your local machine:

Clone the repository:

Bash
git clone https://github.com/yourusername/EssenceAI.git
Install the required dependencies:

Bash
pip install -r requirements.txt
Start the development server:

Bash
python manage.py runserver 

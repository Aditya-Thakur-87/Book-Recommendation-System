📚 Book Recommendation System

A Flask-based web application that recommends books to users based on their input.
It uses a collaborative filtering approach with similarity scores precomputed from user-book interactions.

🚀 Features

Homepage shows popular books (based on number of ratings & average rating).

Enter a book title to get Top-4 similar book recommendations.

Displays:

Book Title

Author

Cover Image

📂 Project Structure
.
├── app.py                        # Flask web app
├── Book Recommendation.ipynb     # Notebook for preprocessing & model building
├── popular.pkl                   # Pickled dataframe of popular books
├── pt.pkl                        # Pickled pivot table (user-book matrix)
├── books.pkl                     # Pickled dataframe with book metadata
├── similarity_scores.pkl         # Pickled similarity matrix

⚙️ Installation & Setup
1. Clone the Repository
git clone https://github.com/your-username/book-recommender.git
cd book-recommender

2. Install Dependencies
pip install flask numpy pandas scikit-learn

3. Run Flask App
python app.py


Go to 👉 http://127.0.0.1:5000/ in your browser.

🧑‍💻 Workflow
Notebook (Book Recommendation.ipynb)

Perform data cleaning & preprocessing.

Create a user-item pivot table.

Compute similarity scores between books.

Identify popular books based on ratings.

Save results as .pkl files for the Flask app.

Flask App (app.py)

Loads .pkl files.

/ → Homepage displaying popular books.

/recommend → Page where user can search a book.

/recommend_books → Backend route returning Top-4 recommended books.

📸 Example

Homepage – Displays top popular books.

Search "Harry Potter"
→ Recommends other fantasy novels.

🌐 Deployment

You can deploy this app.

Push to GitHub.

Connect Heroku app → Deploy.

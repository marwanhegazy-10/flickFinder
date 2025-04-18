# FlickFinder: Movie Recommendation System

This repository contains a movie recommendation system built using the [MovieLens](https://grouplens.org/datasets/movielens/) dataset. The system allows users to search for movies and receive recommendations based on similar users' preferences and content-based similarity.

## Features

- **Search for Movies**: Use an interactive interface to find movies by their titles.
- **Content-Based Recommendations**: Find movies with similar titles using TF-IDF vectorization and cosine similarity.
- **Collaborative Filtering**: Recommend movies based on ratings from similar users.
- **Interactive Notebook**: Explore the recommendation system interactively using Jupyter Notebook.

## Dataset

The project uses the **MovieLens 25M Dataset**, which contains:
- 25 million ratings for 62,000 movies by 162,000 users.
- Metadata about movies, including genres and release years.

You can download the dataset [here](https://files.grouplens.org/datasets/movielens/ml-25m.zip).

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/marwanhegazy-10/movie-recommendations.git
   cd movie-recommendations
   ```

2. Ensure Jupyter Notebook is installed:
   ```bash
   pip install notebook
   ```

3. Download and extract the MovieLens dataset into the project directory.

## Usage

1. Open the Jupyter Notebook:
   ```bash
   jupyter notebook movie_recommendations.ipynb
   ```

2. Follow the instructions in the notebook to:
   - Search for movies by title.
   - View content-based recommendations.
   - Explore collaborative filtering recommendations.

3. Enter a movie title (e.g., "Toy Story") in the interactive search box to get recommendations.

## Example Workflow

1. **Search for a Movie**:
   Enter a movie title in the search bar (e.g., "Toy Story").

2. **View Recommendations**:
   - Content-based recommendations: Movies with similar titles or genres.
   - Collaborative filtering recommendations: Movies liked by users with similar preferences.

3. **Example Output**:
   Searching for **"Toy Story"** might recommend:
   - **Finding Nemo** (Animation|Adventure|Comedy)
   - **Shrek** (Animation|Comedy|Family)
   - **The Lion King** (Adventure|Children|Animation)

## File Structure

```
.
├── README.md                       # Project documentation
├── movie_recommendations.ipynb     # Jupyter Notebook with the recommendation system code
```

## Key Functions in `movie_recommendations.ipynb`

- `clean_title(title)`: Cleans movie titles by removing special characters.
- `search(title)`: Searches for movies with similar titles using TF-IDF.
- `find_similar_movies(movie_id)`: Recommends movies based on collaborative filtering.

## Dependencies

- Python 3.8+
- Pandas
- scikit-learn
- Jupyter Notebook
- ipywidgets

## Acknowledgments

- Dataset provided by [GroupLens Research](https://grouplens.org/).
- Recommendation algorithms inspired by classic machine learning techniques.
- This project was developed with guidance and resources from Dataquest.

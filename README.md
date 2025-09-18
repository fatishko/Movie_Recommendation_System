# Movie Recommendation System

A content-based movie recommendation system that suggests movies based on similarity to your favorite movie.

## Features

- Recommends movies based on genres, keywords, tagline, cast, and director
- Uses TF-IDF vectorization and cosine similarity for recommendations
- Fuzzy string matching to handle minor spelling errors in movie titles
- Returns top 30 similar movies

## Requirements

```bash
pip install numpy pandas scikit-learn
```

## Dataset

The system expects a CSV file named `movies.csv` with the following columns:
- `title`: Movie title
- `genres`: Movie genres
- `keywords`: Keywords associated with the movie
- `tagline`: Movie tagline
- `cast`: Main cast members
- `director`: Movie director
- `index`: Unique identifier for each movie

## Usage

1. Place your `movies.csv` file in the project directory
2. Update the file path in the code if necessary
3. Run the script
4. Enter your favorite movie name when prompted
5. Get personalized movie recommendations

## How It Works

1. **Data Processing**: Combines multiple movie features into a single text representation
2. **Vectorization**: Converts text data into numerical vectors using TF-IDF
3. **Similarity Calculation**: Computes cosine similarity between all movies
4. **Recommendation**: Finds and ranks movies most similar to your input
5. **Output**: Displays top 30 recommended movies

## Example

```
Enter your favourite movie name: The Dark Knight
Movies suggested for you:

1. The Dark Knight
2. Batman Begins
3. The Dark Knight Rises
...
```

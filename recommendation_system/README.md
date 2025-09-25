# Movie recommendation system movieLens

This project demonstrates a **movie recommendation system** using the [MovieLens dataset](https://grouplens.org/datasets/movielens/). The project covers data loading, exploration, visualization and basic recommendation strategies.

## Dataset

The MovieLens dataset is provided by [GroupLens](https://grouplens.org/datasets/movielens/) and contains movie ratings from users, along with movie metadata including titles and genres.

Files used in this project:
- `movies.csv`: movie metadata (MovieId, Title, Genres)
- `ratings.csv`: user ratings (UserId, MovieId, Rating, Timestamp)

## Features

- **Data loading and cleaning**
  - Load movies and ratings CSV files using `pandas`.
  - Preprocess columns and set indexes as needed.

- **Exploratory data analysis (EDA)**
  - Visualize movie and user statistics.
  - Examine rating distributions, timestamps, and popular genres.

- **Visualization**
  - Use `matplotlib` and `seaborn` to generate bar charts, line plots, scatter plots, and histograms.
  - Explore trends in ratings over time and across movies.

- **Recommendation**
  - Compute total votes per movie.
  - Compute average ratings per movie.
  - Filter movies with enough votes for more reliable recommendations.
  - Sort movies to recommend top-rated films to users.

## Installation

Run the project in a **local python environment** or **Google Colab**. The following libraries are required:

```python
import pandas as pd
import seaborn as sns
from matplotlib import pyplot as plt
```

## Usage

- Load the `MovieLens` dataset.
- Explore and visualize user ratings and movie metadata.
- Compute total votes and average ratings per movie.
- Filter and rank movies to generate recommendations.

## Notes

- Each project is designed as a prototype for learning and experimentation.
- Large datasets may require sufficient memory and computation resources.
- The code is written in python 3 and uses standard data science libraries.

## License

This project is licensed under the MIT License. You are free to use, modify, and distribute the code as needed.
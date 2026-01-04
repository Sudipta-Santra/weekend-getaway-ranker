# Weekend Getaway Ranker
## Project Title

Weekend Getaway Ranker – Data Engineering Project


## Project Objective

he objective of this project is to recommend the best weekend travel destinations in India based on a user’s source city.

- The system ranks tourist places using:

- Distance from the source city

- Google review rating

- Popularity (number of Google reviews)


## Dataset Used

### Top Indian Places to Visit

## Important Columns Used:

- Name – Tourist place name

- City – Destination city

- Google review rating – Quality of the place

- Number of google review in lakhs – Popularity of the place

- Other columns are available in the dataset but are not used to keep the project simple.

## Technologies Used

- Python
- Pandas

## How the Project Works

1. User enters a source city

2. Source city coordinates are fetched from an offline city database

3. Distance to each tourist place is calculated using the Haversine formula

4. Rating, popularity, and distance are normalized

5. A final score is calculated using weighted ranking

6. Top weekend destinations are displayed


### Ranking Formula

    Each place is ranked using:

        Final Score = (0.5 × Rating) + (0.3 × Popularity) + (0.2 × Distance)
    
    Higher score means a better recommendation.


## Project Structure

        weekend-getaway-ranker/
        │
        ├── weekend_getaway_ranker.py
        ├── Top Indian Places to Visit.csv
        └── README.md

### Learning Outcomes

- Understanding of data preprocessing
- Distance calculation using latitude and longitude
- Feature normalization
- Rule-based recommendation systems
- Practical data engineering concepts  

## Conclusion

This project presents a simple and effective weekend travel recommendation system built using data engineering principles. By combining distance calculation, user ratings, and popularity through a weighted ranking approach, the system generates meaningful and practical travel recommendations. The solution avoids machine learning and external APIs, focusing instead on clear logic and reliable results, making it easy to understand, evaluate, and extend in the future.
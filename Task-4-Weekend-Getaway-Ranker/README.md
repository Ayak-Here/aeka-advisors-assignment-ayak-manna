# Task 4 – Weekend Getaway Ranker

## Overview
This project implements a simple recommendation system that ranks suitable weekend travel destinations in India based on a given source city.

The goal is to help users identify nearby and popular places that are practical for short weekend trips.

---

## Dataset
The project uses a travel dataset containing information about India’s must-see tourist places.  
Important fields used from the dataset include:

- City  
- State  
- Zone  
- Tourist Place Name  
- Google Review Rating  
- Number of Google Reviews  

The dataset provides sufficient information to rank destinations logically without using external APIs.

---

## Approach
The ranking algorithm is based on three main factors:

1. **Distance Proximity**  
   Since exact geographical distances were not available, distance was estimated logically using:
   - Same city  
   - Same state  
   - Same zone  
   - Different zone  

   Strong penalties were applied to far-away destinations to ensure realistic weekend recommendations.

2. **Rating**  
   Google review ratings were normalized and used to reflect user satisfaction.

3. **Popularity**  
   Popularity was derived from the number of Google reviews and normalized.

A weighted scoring formula was applied:
- Distance score: 45%
- Rating score: 35%
- Popularity score: 20%

Destinations are ranked based on the final combined score.

---

## Files Included
- `weekend_getaway_ranker.py` – Python script implementing the ranking algorithm  
- `requirements.txt` – Required Python dependency  
- `sample_output.txt` – Sample ranked outputs for three different source cities  

---

## How to Run
1. Ensure the dataset CSV file is present in the same directory as the script
2. Install the required dependency using `requirements.txt`
3. Run the Python script
4. Enter a source city when prompted
5. View the ranked list of recommended weekend destinations

---

## Sample Cities Tested
- Delhi  
- Mumbai  
- Kolkata  

The outputs for these cities are provided in the `sample_output.txt` file.

---

## Notes
- This project focuses on data engineering and ranking logic, not machine learning
- The solution is designed to be simple, explainable, and realistic
- All work is original and follows the no-plagiarism policy

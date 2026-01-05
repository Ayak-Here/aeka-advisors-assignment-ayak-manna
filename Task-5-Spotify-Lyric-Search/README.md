# Task 5 – Spotify Lyric Search

## Project Overview
This project implements a text identification model that predicts the **song title** and **artist name** when a small snippet of song lyrics is provided as input.

The objective of this task is to demonstrate the use of text preprocessing techniques and a similarity-based model for lyric identification.

---

## Dataset Information
- Dataset Name: Spotify Million Song Dataset
- Total records: 57,651
- Columns used:
  - artist
  - song
  - text (lyrics)

The dataset was downloaded from Kaggle and contains song lyrics along with corresponding artist and song names.

Due to GitHub file size limitations, the complete dataset is **not uploaded** to this repository.

---

## Dataset Access
The full dataset can be downloaded from Kaggle using the link below:

https://www.kaggle.com/datasets/joebeachcapital/57651-spotify-songs

A small sample dataset (`spotify_sample.csv`) is included in this repository for reference and testing purposes.

---

## Technologies Used
- Python
- Pandas
- Natural Language Processing (NLP)
- Scikit-learn
- Jupyter Notebook

---

## Methodology
1. Lyrics text is preprocessed using:
   - Lowercasing
   - Tokenization
   - Stop-word removal
   - Removal of punctuation and unwanted characters
2. TF-IDF Vectorization is applied to convert text into numerical features.
3. Cosine similarity is used to compare lyric similarity.
4. The most similar song lyrics are selected to predict the song title and artist.

This approach is suitable for lyric-based search and text identification problems.

---

## Model Usage
The model accepts a short lyric snippet as input and returns:
- Predicted Song Title
- Predicted Artist

---

##Example input:
she makes me feel fine who could ever believe

##Example output:
Predicted Song Title: Ahe's My Kind Of Girl
Predicted Artist: ABBA

---

## Model Evaluation
Prediction accuracy is demonstrated within the Jupyter Notebook by comparing predicted song titles against the actual song titles from a test dataset.

---

## Installation & Execution
1. Open the Jupyter Notebook file:
2. Ensure the dataset file is available:
- Either download the full dataset from Kaggle
- Or use the provided `spotify_sample.csv`
3. Run all cells in sequence
4. Enter a lyric snippet in the final input cell to test the model

No additional setup is required.

---

## Notes
- This project uses a similarity-based text identification approach.
- The implementation focuses on clarity, correctness, and ease of evaluation.
- All work is original and follows the no-plagiarism policy.

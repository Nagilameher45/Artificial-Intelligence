**Project 2 : Spotify Song's Genre Segmentation**

The music recommendations made by Spotify, a music app, are excellent. It recommends music based on the songs and artists you usually listen to. The algorithm groups comparable features into clusters, and these clusters aid in comprehending the auditory properties of diverse songs. 
This project uses K-Means clustering to group Spotify songs based on their audio features such as danceability, energy, valence, loudness, tempo, etc.
After clustering, a simple recommendation system is implemented that suggests songs from the same cluster, meaning they have similar musical characteristics.

**Project Overview**

Load Spotify dataset
Handle missing values
Select important numerical audio features
Scale the features using StandardScaler
Determine the optimal number of clusters using the Elbow Method
Apply K-Means clustering
Visualize clusters (Energy vs Danceability)
Display cluster summary
Provide recommendations based on cluster similarity

**Technologies Used**

Python
Pandas
NumPy
Scikit-Learn
Matplotlib
Seaborn
Google Colab

**Project Structure**
├── Spotify_dataset.csv
├── project2.ipynb      # Google Colab Notebook
├── project2(1).py         # Python Script
└── README.md

**How to Run the Project**
1. Clone this repository:
git clone https://github.com/Nagilameher45/Artificial-Intelligence.git

2. Open the notebook in Google Colab or Jupyter:
Project2.ipynb

3. Or run the Python script:
python project2(1).py

**Main Features**
✔ 1. Missing Value Handling
All NULL values in numeric columns are filled using the mean.

✔ 2. Feature Selection
Attributes used for clustering:
danceability
energy
loudness
speechiness
acousticness
instrumentalness
liveness
valence
tempo

✔ 3. Feature Scaling

Standardization using:
StandardScaler()

✔ 4. K-Means Clustering
Used Elbow Method to find optimal k
Final model uses k = 4

✔ 5. Visualization
Scatter plot:
x-axis → energy
y-axis → danceability
colored by cluster

✔ 6. Recommendation System
Given a song index:
Find its cluster
Recommend other songs from the same cluster

**Example Recommendation Output**
Selected Song: Memories - Dillon Francis Remix
Cluster: 2

Recommended Songs:
- Song A by Artist A
- Song B by Artist B
- Song C by Artist C
...

**Future Enhancements**

Add cosine similarity for more accurate recommendations
Visualize clusters using PCA or t-SNE
Build a Streamlit web app interface
Integrate live Spotify API data


Nagila Meher A
Machine Learning Intern

# Content Based Movie Recommendation System using Streamlit

#### 🔗 *[Movie Recommendation Website](https://mrs-sd.streamlit.app/)*

(https://img.shields.io/badge/Python-3.10-fcba03) ![Frontend](https://img.shields.io/badge/Frontend-Streamlit-red) ![API](https://img.shields.io/badge/API-TMDB-237a3b) ![API](https://img.shields.io/badge/ML-Numpy_|_Pandas_|_NLTK_|_Scikit_learn_|_Count_Vectorizer_|_Cosine_Similarity-blue)

A content-based movie recommendation system that suggests films according to user preferences using cosine similarity.

The model was extensively trained on a diverse dataset of over 5000+ movies.

Recommendations are generated by calculating similarity scores for movies using cosine similarity. Tags for each movie are created by combining various details such as genre, title, top cast, and director. These tags are then converted into vectors to form a similarity matrix. When a movie is searched, movies with the highest similarity scores are sorted and recommended.


## How Cosine Similarity works?

Cosine similarity is a metric used to measure how similar two vectors are by calculating the cosine of the angle between them. In the context of a recommendation system, it quantifies the similarity between two items (such as movies) based on their attributes (like genre, title, cast, etc.). The cosine similarity ranges from -1 to 1, where 1 indicates perfect similarity, 0 indicates no similarity, and -1 indicates perfect dissimilarity. This method is particularly effective for high-dimensional data and is widely used in text analysis and recommendation systems.

  ![image][(https://www.google.com/url?sa=i&url=https%3A%2F%2Fmedium.com%2Fgeekculture%2Fcosine-similarity-and-cosine-distance-48eed889a5c4&psig=AOvVaw2G9732hCZvKwuVEx89Bkcw&ust=1721994289459000&source=images&cd=vfe&opi=89978449&ved=0CBEQjRxqFwoTCJic_96OwocDFQAAAAAdAAAAABAE)].

Understanding Similarity Scores
How does the system decide which item is most similar to the one the user likes? This is where similarity scores come in.

A similarity score is a numerical value ranging between zero and one, indicating the degree of similarity between two items on this scale. The score is derived by measuring the similarity between the text details of both items. Essentially, the similarity score quantifies the resemblance between the given text details of two items. This is typically calculated using cosine similarity.

More about Cosine Similarity : [Understanding the Math behind Cosine Similarity](https://www.machinelearningplus.com/nlp/cosine-similarity/)

## How to run the project locally?

1. Clone or download this repository to your local machine.
2. `cd` into the cloned folder.
3. Install virtual environment python package using command:

   ```
   pip install virtualenv
   ```
4. Create a virtual environment using command:

   ```
   python3 -m venv [Enter Folder name]
   ```
5. Activate virtual environment using command:

   ```
   source [virtual environment name]/bin/activate
   ```
6. Install all the libraries mentioned in the [requirements.txt](https://github.com/soumadeep-dey/Movie-Recommendation-System/blob/main/requirements.txt) file with the command:

   ```
    pip install -r requirements.txt
   ```
7. Install ipykernel using command:

   ```
   pip install ipykernel
   ```
8. Create a kernel user using command:

   ```
   ipython kernel install --user --name=[Enter kernel_name]
   ```
9. Get your API key from [themoviedb.org](https://www.themoviedb.org/settings/api)
10. Create a `.env` file and paste the API key insde the file as follows:

    ```
    API_KEY = YOUR_API_KEY
    ```
11. Run the file `app.py` by executing the command:

    ```
    streamlit run app.py
    ```
12. The streamlit app will locally run on your browser using your default browser or run it manually in any browser using  the local url provided in your terminal as follows:

    ```
     You can now view your Streamlit app in your browser.

      Local URL: http://localhost:8501 (port number can be different) [copy and paste in any browser]
      Network URL: http://192.168.0.103:8501

    ```


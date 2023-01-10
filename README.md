# Rick & Morty Scripts | NLP Analysis | KNN Clustering 📄📚📊

![Captura de pantalla_20230110_202823](https://user-images.githubusercontent.com/119113483/211643725-bfbf6570-44c9-4110-a34d-2d9ea1a506b9.png)


## Technologies 💻
* Python
* Jupyter

## Python Libraries 🗃️
* Numpy
* Pandas
* Matpoltlib
* Scikit-learn
* Re
* Nltk
* WorkCloud
* Tfidf
* PCA

## Objectives 📋

The main objective of this project is to differentiate topics in a set of scripts of the famous tv serie Rick & Morty. To achieve this we will use text mining and clustering.

## Data 📁

The dataset contains 1905 scripts of the chapters, with several columns like: episode name, character, season...

## Text mining 🗒️⛏️

* First of all, we eliminate the "stopwords" from the abstract column, discarding irrelevant words to reduce the dimension later, facilitating the training of the model.
* We convert each word of the abstract to tokens in order to work with them.
* We eliminate the words that only appear once and the numbers, since when creating clusters they do not give us anything.
* We convert each word to its stem to be able to group them later in clusters.
* We get the TF-IDF array and convert it to a dataframe to work with.

## Clustering 🟡🔴🟢

Now that we have done the preprocessing of the text we can start working with the dataset that we have created and use clustering techniques to try to identify topics and group the articles.

* The first thing we do is use PCA to reduce the dimensionality of our dataset. In this case we chose 500 components with explained variance of 80%.

![Captura de pantalla_20230110_203427](https://user-images.githubusercontent.com/119113483/211644895-0e8e9344-5d81-4850-8ee0-ea4631adf8c8.png)

* Then we calculate the inertia 

![Captura de pantalla_20230110_203453](https://user-images.githubusercontent.com/119113483/211645036-30d52ac4-a6b0-462c-aa6a-0bc3107397eb.png)

Afterwards, we used different techniques to try to obtain the optimal number of clusters and we carried out different tests and post-analysis of the results obtained with metrics and visualization tools.

![Captura de pantalla_20230110_203603](https://user-images.githubusercontent.com/119113483/211645235-89072aa1-0929-40e5-8d1b-99e951c7fb99.png)

![Captura de pantalla_20230110_203550](https://user-images.githubusercontent.com/119113483/211645245-e1b81a51-deab-4baa-a8f7-1ceb150b884d.png)

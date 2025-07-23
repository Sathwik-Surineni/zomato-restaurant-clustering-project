

# Zomato Clustering: From Messy Data to Foodie Groups 

This project is a fun dive into the Zomato restaurant dataset for Hyderabad. We use a bit of data science magic (a.k.a. machine learning) to find out what the city's food scene *really* looks like,how we turned a confusing spreadsheet into simple, understandable segments.

---

###  The Problem
There are thousands of restaurants on Zomato, and it's impossible to manually sort them into clear groups. Our goal is to use **clustering** to automatically find these groups based on data like their price and the type of food they serve. This helps us see the bigger picture of the city's market.

---

###  Key Features We Looked At
* **Cost**: The average cost for two people.
* **Cuisines**: The types of food served (e.g., North Indian, Italian, etc.).
* **Collections**: Special curated lists from Zomato (e.g., "Trending This Week").

---

###  How It's Done: Our Project Workflow

1.  **Data Cleanup**: The first step was a major cleanup. The raw data was a bit of a mess, so we had to fix columns, handle missing values, and get everything into a clean, usable format.

2.  **Data Exploration (EDA)**: We went deep into the data by creating **15 different charts**! This is where we found cool insights, like discovering that `North Indian` and `Chinese` food are the most common and that most restaurants are surprisingly affordable.

3.  **Feature Prep & Scaling**: Before modeling, we had to get our data ready. We converted the text-based 'Cuisines' into numbers (0s and 1s) using One-Hot Encoding and then **scaled** all the data so our model would treat every feature fairly.

4.  **Clustering Magic**: We experimented with three different clustering models: K-Means, Hierarchical, and DBSCAN. After evaluating them, we found that **K-Means** with **5 clusters** gave us the most logical and useful groups.

---

###  The Results: Our 5 Restaurant Clusters

Our final K-Means model sorted the restaurants into these five distinct "vibes":

* **Cluster 0: The Budget Bistros** 
    * *Profile*: Low-cost spots serving the most popular cuisines like North Indian and Chinese. This is the biggest and most competitive group.

* **Cluster 1: The Mid-Range Eateries** 
    * *Profile*: Moderately priced restaurants, often specializing in cuisines like Mughlai and Biryani. Perfect for family dinners.

* **Cluster 2: The Premium Dining Spots** 
    * *Profile*: A small, exclusive group of high-cost restaurants, usually serving Continental or Italian food.

* **Cluster 3: The Quick Bites & Cafes** 
    * *Profile*: Very low-cost places focused on Fast Food, Desserts, and Beverages. Very popular with a younger crowd.

* **Cluster 4: The Specialty Hubs** 
    * *Profile*: A unique group of restaurants that specialize in less common but popular niches, like authentic local cuisines.

---

###  Tech Stack
* **Python**
* **Pandas** & **NumPy** for data manipulation
* **Matplotlib** & **Seaborn** for visualizations
* **Scikit-learn** for machine learning (K-Means, DBSCAN, etc.)
* **Google Colab** as our workspace

---

###  How to Use This
1.  Clone this repository to your local machine.
2.  Make sure you have the required Python libraries installed.
3.  Open the `.ipynb` notebook file in Google Colab or Jupyter Notebook.
4.  Run the cells from top to bottom to see the magic happen!

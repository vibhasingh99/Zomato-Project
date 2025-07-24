
# 🍽️ Zomato Sentiment-Based Restaurant Recommendation System

This project is a Natural Language Processing (NLP) powered recommendation system that suggests similar restaurants based on customer reviews and sentiments extracted from Zomato data.

---

## 📌 Objective

To build a system that:
- Cleans and analyzes real restaurant reviews
- Performs sentiment analysis (positive, neutral, negative)
- Recommends restaurants based on review similarity using cosine similarity
- Visualizes recommendations for better interpretation

---

## 📂 Dataset Description

We used two datasets:
1. **Zomato Restaurant Metadata**
   - Name, Cost, Cuisine, Timings, etc.
2. **Zomato Restaurant Reviews**
   - Restaurant name, Reviewer, Review, Rating, Time, etc.

These were merged using the restaurant name for unified analysis.

---

## 🔧 Key Steps Performed

1. **Data Loading & Merging**  
   Loaded both datasets using Pandas and merged them into a single frame for analysis.

2. **Text Preprocessing**  
   - Lowercased reviews  
   - Removed punctuation, stopwords, special characters  
   - Cleaned empty or missing reviews  

3. **Sentiment Analysis**  
   - Used TextBlob to calculate polarity  
   - Classified each review as Positive, Negative, or Neutral  

4. **TF-IDF Vectorization**  
   - Converted cleaned text into numerical vectors  
   - Used `TfidfVectorizer` from `sklearn`  

5. **Cosine Similarity-Based Recommendation**  
   - Built a `recommend()` function  
   - Takes a restaurant name input  
   - Finds top 5 most similar restaurants based on review content  

6. **Visualization**  
   - Used Seaborn to display the sentiment and cost of similar restaurants  
   - Displayed results in a clean vertical bar chart

---

## 📊 Output Example

For input: `"Barbeque Nation"`, the model returns 5 similar restaurants with:
- Cuisine type  
- Cost for two  
- Overall sentiment  
- And a visual bar plot for comparison

---

## 💡 Tools & Libraries Used

- Python
- Pandas
- Numpy
- NLTK
- TextBlob
- Scikit-learn
- Matplotlib
- Seaborn

---

## 📈 Skills Demonstrated

- Text Cleaning & NLP
- Sentiment Analysis
- TF-IDF Vectorization
- Cosine Similarity
- Recommendation Engine
- Data Visualization
- Real-world Data Handling

---

## 📌 How to Run

1. Clone the repository or download the `.ipynb` notebook.
2. Ensure required libraries are installed (`pip install -r requirements.txt`).
3. Run each cell in sequence on Jupyter Notebook or Google Colab.
4. Call the `recommend()` function with any valid restaurant name.

---

## 🎓 Conclusion

This project demonstrates how NLP techniques can enhance recommendation systems by incorporating real user sentiments, making suggestions more personalized and intuitive.

---

## 🧑‍💻 Author

**Vibha Singh Chauhan**   
Email: vibhachauhan85@gmail.com

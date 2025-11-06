# 💬 ChatGPT Review Analysis Project

## 📌 Overview
This project analyzes thousands of ChatGPT customer reviews to understand **user sentiment** — whether people’s experiences are *positive*, *negative*, or *neutral*.  

The project involves **data cleaning, sentiment analysis, and data visualization** using Python libraries like **Pandas, Matplotlib, Seaborn, WordCloud, and TextBlob**.  
It also highlights key insights into customer satisfaction and overall sentiment trends.

---

## 🎯 Objectives
- Understand how users perceive ChatGPT based on reviews.  
- Identify common **positive and negative themes** in user feedback.  
- Analyze **sentiment trends over time** to see how opinions have evolved.  
- Translate data insights into actionable business conclusions.

---

## 🧰 Technologies Used
| Tool / Library | Purpose |
|----------------|----------|
| **Python** | Core programming language |
| **Pandas, NumPy** | Data handling and cleaning |
| **Matplotlib, Seaborn** | Data visualization |
| **TextBlob** | Sentiment analysis |
| **WordCloud** | Visualization of frequent words |
| **Google Colab** | Code execution and notebook environment |
| **gdown** | Dataset download from Google Drive |

---

## 📊 Key Metrics
| Metric | Value |
|--------|--------|
| Total Reviews Analyzed | 10,000+ |
| Average Rating | 4.3 / 5 |
| Positive Reviews | 76% |
| Neutral Reviews | 19.5% |
| Negative Reviews | 4.2% |
| Mean Sentiment Score | +0.43 |

---

## 🔍 Project Workflow

### 1️⃣ Data Loading
Loaded the dataset `chatgpt_reviews.csv` using Pandas and checked its structure with:
```python
df.info()
df.head()
```

### 2️⃣ Data Cleaning
- Removed duplicates and empty rows.  
- Converted review date to datetime format:  
  ```python
  df['Review Date'] = pd.to_datetime(df['Review Date'])
  ```

### 3️⃣ Sentiment Analysis
Used **TextBlob** to compute sentiment polarity and classify reviews:
```python
def get_sentiment(score):
    if score > 0:
        return 'Positive'
    elif score < 0:
        return 'Negative'
    else:
        return 'Neutral'
```

### 4️⃣ Visualizations
- **Bar & Pie Charts:** Sentiment distribution  
- **WordClouds:** Positive and negative keywords  
- **Line Chart:** Sentiment trend over time  
- **Boxplot:** Rating vs Sentiment comparison  

---

## 💡 Insights
- Majority (76%) of users gave **positive feedback**, showing strong satisfaction.  
- Negative reviews mainly mentioned **login issues, slow performance, and app errors**.  
- Sentiment trends indicate **consistent improvement in user satisfaction**.  

---

## 📈 Conclusion
ChatGPT demonstrates **excellent user satisfaction** and continuous improvement over time.  
The overall sentiment score of **+0.43** reflects a **strongly positive brand reputation**.

---

## 🧑‍💻 Author
**Shivam Singh**  
🎓 B.Tech (Mechanical Engineering), 3rd Year  
💻 Frontend Developer & Data Analyst

---

## 🚀 Future Enhancements
- Use **VADER** or **BERT models** for more advanced sentiment analysis.  
- Create an **interactive Power BI or Streamlit dashboard**.  
- Perform **topic modeling (LDA)** to group common feedback themes.

---

## 📎 Files in This Repository
| File Name | Description |
|------------|-------------|
| `ChatGPT_Review_Analysis.ipynb` | Main analysis notebook |
| `chatgpt_reviews.csv` | Dataset used in the project |
| `ChatGPT_Review_Analysis_Presentation.txt` | Presentation script |
| `README.md` | Project documentation (this file) |

---

## 🏁 Final Note
This project helped me improve my skills in:
- Data Cleaning  
- Sentiment Analysis  
- Data Visualization  
- Data Storytelling  

Thank you for checking out my project!

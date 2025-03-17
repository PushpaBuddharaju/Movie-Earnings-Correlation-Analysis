# 🎬 Movie Earnings Correlation Analysis using Python  

## 📌 Project Overview  
This project explores the **factors affecting movie gross earnings** using the **Movies.csv dataset** from Kaggle.  
The initial hypothesis was that **company name** would be highly correlated with revenue.  
However, through **data analysis and visualization in Python**, it was discovered that **budget and votes** had the highest correlation with gross earnings.  

## 📁 Dataset  
Dataset: [Movies.csv](https://www.kaggle.com/datasets/danielgrijalvas/movies) (Downloaded from Kaggle)  
### 📜 Column Names in the Dataset  
| Column Name     | Description |
|----------------|------------|
| `name`         | Movie title |
| `rating`       | Movie rating (e.g., PG-13, R) |
| `genre`        | Movie genre (e.g., Action, Comedy) |
| `year`         | Incorrect release year (Dropped) |
| `released`     | Release date (Used to extract `released_year`) |
| `score`        | IMDb rating score |
| `votes`        | Number of votes on IMDb |
| `director`     | Director of the movie |
| `writer`       | Writer of the movie |
| `star`         | Lead actor/actress |
| `country`      | Country of production |
| `budget`       | Budget of the movie |
| `gross`        | Total earnings at the box office |
| `company`      | Production company |
| `runtime`      | Duration of the movie in minutes |
| `released_year` | Extracted from `released` column |

## 🛠️ Technologies & Tools
- **Google Colab**
- **Python**   
- **Pandas** for data manipulation  
- **NumPy** for numerical operations  
- **Matplotlib & Seaborn** for data visualization 

## 📊 Key Steps  
1️⃣ **Data Preprocessing:**  
   - Imported dataset using Pandas.  
   - Checked for missing values and dropped them as they didn’t impact analysis.  
   - Converted `Budget` and `Gross` columns to integer type for better readability.  

2️⃣ **Feature Engineering:**  
   - Extracted Released Year from the `Released` column and created a new column **Relesed_Year** since the `Year` column contained incorrect values.  
   - Removed the incorrect `Year` column for data accuracy.

3️⃣ **Data Cleaning:**  
   - Dropped duplicate records to maintain data integrity.  

4️⃣ **Data Visualization & Correlation Analysis:**  
   - **Regression Plot**: Visualized the relationship between **budget and gross earnings** using Seaborn.  
   - **Heatmap**: Displayed correlations between numeric columns to identify key factors influencing revenue.  
   - **Categorical Encoding**: Converted categorical columns to numeric ones for a deeper correlation analysis.  
   - **Correlation Sorting**: Unstacked and sorted correlation pairs to highlight the strongest relationships.  

## 🔍 Findings  
✅ **Budget and Votes are highly correlated with Gross Earnings** 📈  
❌ **Company name has little to no impact on revenue**  

## 📜 Code  
Check out the full project code in the **Google Colab file** in this repository.  

## 🌍 Real-World Applications  
This project can be useful in various domains:  
- **🎥 Film Production:** Helps studios optimize budgets by understanding how spending impacts revenue.  
- **💰 Investment Decision-Making:** Investors can assess which factors contribute most to a movie’s financial success.  
- **📊 Data-Driven Marketing:** Provides insights on audience engagement (votes) and how it correlates with revenue.  
- **🎬 Streaming Services:** Platforms like Netflix or Amazon Prime can analyze trends to make data-backed content acquisition decisions.  

🚀 **If you find this project useful, feel free to fork and star ⭐ the repository!**  

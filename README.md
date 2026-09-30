\# 📊 Udemy Courses — End-to-End Data Analysis



An end-to-end portfolio project that cleans, explores and visualises the

\[Udemy Courses Dataset](https://www.kaggle.com/) to uncover \*\*pricing,

popularity, and subject-level trends\*\* across \~3,700 online courses.



!\[Subject Distribution](images/subject\_distribution.png)



\## 🎯 Objectives

\- Clean 12 data-quality issues (mixed types, shifted columns, duplicates).

\- Explore how \*\*price, subject, level, duration, and publishing year\*\* affect enrolment.

\- Produce publication-ready visualisations and a PDF report.



\## 🗂️ Project Structure

\\`\\`\\`

udemy-analysis/

├── data/UdemyCoursesDataset.csv

├── notebooks/udemy\_analysis.ipynb

├── report/udemy\_analysis\_report.html

├── images/

├── README.md

└── requirements.txt

\\`\\`\\`



\## 🧹 Data Cleaning Highlights

| Issue | Resolution |

|---|---|

| `price = "Free"` | Converted to `0`, added boolean `is\_paid` |

| Column-shift rows | Dropped |

| `content\_duration` mixed units | Regex → `duration\_minutes` |

| String timestamps | `pd.to\_datetime` + `year`, `month` |

| Duplicate `course\_id` | Kept first occurrence |



\## 📈 Key Insights

1\. \*\*Web Development\*\* is the most supplied subject (\~34 %).

2\. \*\*92 % of courses are paid\*\*, but a handful of free courses top 200 k subscribers.

3\. Price and popularity are \*\*uncorrelated\*\* (r ≈ −0.02).

4\. \*\*Reviews ≈ Subscribers\*\* (r = 0.87) → reviews are the best popularity proxy.

5\. Publishing exploded \*\*2015–2016\*\* while average price fell.



\## 🛠️ Tech Stack

`Python` · `Pandas` · `NumPy` · `Matplotlib` · `Seaborn` · `Jupyter`



\## 🚀 How to Run

\\`\\`\\`bash

git clone https://github.com/yourhandle/udemy-analysis.git

cd udemy-analysis

pip install -r requirements.txt

jupyter notebook notebooks/udemy\_analysis.ipynb

\\`\\`\\`



\## 📄 Report

Open `report/udemy\_analysis\_report.html` in Chrome → \*\*Print → Save as PDF\*\*.



\## 🔮 Future Work

\- Subscriber prediction (XGBoost / linear regression)

\- NLP on course titles

\- Revenue estimation (price × subscribers)

\- Recommendation engine (TF-IDF course similarity)



\## 📬 Connect

\- LinkedIn: \[your profile](https://linkedin.com/in/yourhandle)

\- GitHub: \[@yourhandle](https://github.com/yourhandle)


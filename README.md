
# 🎬 IMDb 2024 Movie Insights Dashboard

Welcome to the **IMDb 2024 Movie Insights Dashboard**, a comprehensive, interactive web application built using **Streamlit** that connects to a **MySQL** database and visualizes curated data from the 2024 IMDb movie dataset.

This project is aimed at providing deep insights into movie ratings, genres, voting trends, durations, and statistical relationships through rich, interactive, and aesthetically designed visualizations.

![Banner](https://img.icons8.com/ios/452/movie-projector.png)

---

## 📌 Table of Contents

- [🎯 Project Overview](#-project-overview)
- [✨ Features](#-features)
- [🖼️ Dashboard Screens](#️-dashboard-screens)
- [📊 Tech Stack](#-tech-stack)
- [🔧 Setup Instructions](#-setup-instructions)
- [🛠️ Project Structure](#️-project-structure)
- [🗃️ Database Schema](#️-database-schema)
- [🚀 Future Improvements](#-future-improvements)

---

## 🎯 Project Overview

This dashboard helps users explore IMDb 2024 movie data through:

- **Real-time MySQL querying**
- **Genre-based filtering and comparison**
- **Statistical correlations between Ratings and Votes**
- **Trends analysis via interactive charts**

Whether you're a data enthusiast, film buff, or developer, this app offers a seamless and engaging way to visualize current movie trends.

---

## ✨ Features

✔️ **Real-Time MySQL Integration**  
✔️ **Custom CSS Theming**  
✔️ **Genre-Based Filtering**  
✔️ **Responsive & Interactive UI**  
✔️ **Data Insights Tabs**  
✔️ **Scatterplots, Pie Charts, Heatmaps, Histograms**  
✔️ **Streamlit Option Menu for Navigation**

---

## 🖼️ Dashboard Screens

| Tab              | Description                                                                 |
|------------------|-----------------------------------------------------------------------------|
| **Overview**     | View Top 10 movies, rating distribution                                     |
| **Genre Analysis**| Genre counts, average durations, top-rated per genre, heatmap ratings     |
| **Voting**       | Average votes by genre, popular genres (pie chart)                         |
| **Durations**    | Highlights shortest and longest movies                                     |
| **Correlations** | Rating vs Vote scatterplot for deeper analysis                             |

---

## 📊 Tech Stack

**Frontend / Dashboard**:  
- Streamlit  
- Plotly  
- Matplotlib  
- Seaborn  

**Backend / Database**:  
- MySQL  
- SQLAlchemy  
- pymysql  

**Data Manipulation**:  
- Pandas  
- NumPy  

---

## 🔧 Setup Instructions

### 1. Clone this Repository

```bash
git clone https://github.com/yourusername/imdb-2024-dashboard.git
cd imdb-2024-dashboard
```

### 2. Create and Activate Virtual Environment (Optional)

```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

### 3. Install Requirements

```bash
pip install -r requirements.txt
```

Or manually:

```bash
pip install streamlit pandas plotly matplotlib seaborn pymysql sqlalchemy streamlit-option-menu
```

### 4. Configure Database Credentials

In `streamlit.py`, update the `get_connection()` function with your actual credentials:

```python
user = 'YOUR_USERNAME'
password = 'YOUR_PASSWORD'
host = 'YOUR_HOST'
port = 'YOUR_PORT'
database = 'YOUR_DATABASE'
```

The default table used is `imdb_2024`.

### 5. Run the Dashboard

```bash
streamlit run streamlit.py
```

The app will open in your browser at `http://localhost:8501`.

---

## 🛠️ Project Structure

```
.
├── streamlit.py                # Main Streamlit dashboard script
├── imdballgenre.ipynb          # (Optional) Jupyter notebook for EDA
├── requirements.txt            # Python dependencies
├── README.md                   # This file
```

---

## 🗃️ Database Schema

The dashboard expects a table called `imdb_2024` with the following columns:

| Column Name   | Data Type    | Description                          |
|---------------|--------------|--------------------------------------|
| `Title`       | VARCHAR       | Movie title                          |
| `Genre`       | VARCHAR       | Primary genre                        |
| `Rating`      | FLOAT         | IMDb rating                          |
| `Votes`       | INT           | Number of votes                      |
| `Duration`    | INT (minutes) | Duration of the movie in minutes     |

---

## 🚀 Future Improvements

- 🎥 Add poster/image previews
- 🧠 NLP-based sentiment analysis from reviews
- 🌍 Map-based country-wise production breakdown
- 📱 Mobile responsiveness improvements
- ☁️ Deploy to Streamlit Cloud or Docker

---

🙌 Acknowledgements IMDb for public movie data.

Open-source contributors and libraries used in this project.

📬 Contact For queries, feel free to reach out via GitHub Issues or connect with me on https://www.linkedin.com/in/suhasan-i-91734324a/
Made with ❤️ by **[Suhasan]**


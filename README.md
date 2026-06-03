# 📊 YouTube Channel & Video Intelligence Suite

This project leverages the **Google YouTube Data API v3** to perform deep-dive analytics on prominent educational and entertainment channels. The analysis is split into two primary layers:

* **Macro-level Channel Benchmarking**
* **Micro-level Video Performance Analysis**

---

## 🚀 Project Overview

The goal of this project is to move beyond surface-level metrics (like total subscribers) to understand the underlying drivers of **growth, engagement, and production efficiency**.

By analyzing channels like:

* Alex The Analyst
* 3Blue1Brown
* GothamChess

we identify patterns that lead to **viral success** and **sustainable audience retention**.

---

## 🛠️ Tech Stack

* **Language:** Python 3.x
* **Data Extraction:** Google API Client Library (`googleapiclient`)
* **Data Manipulation:** Pandas, NumPy
* **Visualization:** Seaborn, Matplotlib
* **Storage:** CSV (raw and processed data)

---

## 📈 Phase 1: Channel Analytics (Macro View)

In this phase, we benchmarked multiple channels to understand their positioning in the ecosystem.

### 🔑 Core Metrics Defined

#### 1. Subscriber Acquisition Rate (SAR)

```
SAR = Total Subscribers / Total Videos
```

* **Concept:** Measures how "hard" each video works to earn a subscriber.

#### 2. Viewer Retention / Loyalty Metric

```
Viewer Retention = Total Views / Total Subscribers
```

* **Concept:** Indicates how often the audience returns or how viral content is relative to subscriber base.

#### 3. Production Efficiency

```
Production Efficiency = Total Views / Total Videos
```

* **Concept:** Average ROI (views) per video.

---

### 📊 Visualizations & Insights

#### Subscriber vs. View Count (Bar Charts)
<img width="690" height="300" alt="image" src="https://github.com/user-attachments/assets/3a700566-d6ba-4e03-a736-bb36b75ee72d" />

* Compares raw reach.
* **Insight:** High subscriber count ≠ high efficiency.
  Some channels grow through fewer, high-quality uploads.

#### Subscriber Acquisition Chart
<img width="690" height="300" alt="image" src="https://github.com/user-attachments/assets/43313355-35b6-494d-b12e-2ad4a99658e0" />


* **Insight:** High SAR (e.g., 3Blue1Brown) → strong **conversion power** and evergreen content.

---

## 🎥 Phase 2: Video-Level Deep Dive

Focused on the **Alex The Analyst** channel with **440+ videos** to uncover the *anatomy of a successful video*.

---

### 🔍 Advanced Metrics & Features

#### Engagement Rates

```
Like Rate = (Likes / Views) * 100
Comment Rate = (Comments / Views) * 100
```

#### Temporal Features

* Year
* Month
* Day of Week
* Hour

#### Title Optimization

Categorized titles into:

* Short
* Medium
* Long
* Very Long

---

## 📊 Key Visualizations

### 1. 🔥 Heatmap: Upload Schedule Strategy
<img width="721" height="400" alt="image" src="https://github.com/user-attachments/assets/b3f16f79-7822-4683-93a4-2be58e21d424" />

* **Chart:** Day of Week vs Hour (Seaborn Heatmap)
* **Insight:**
  Mid-week uploads (Tuesday/Thursday) during peak UTC hours → higher initial traction.

---

### 2. 📦 Boxplot: Views Distribution Over Years
<img width="592" height="484" alt="image" src="https://github.com/user-attachments/assets/12893838-d747-4d98-a97b-1326fb18113d" />

* **Chart:** Log-scaled boxplot of views
* **Insight:**
  Shows **Long Tail Effect**:

  * Evergreen videos continue gaining views
  * Some channels depend heavily on new uploads

---

### 3. 📉 Scatterplot: Engagement Correlation
<img width="721" height="400" alt="image" src="https://github.com/user-attachments/assets/787d8776-23d5-4b54-9a71-02885c101ef0" />

* **Chart:** Views vs Like Rate (size = Comment Rate)
* **Insight:**

  * High views + low likes → possible **clickbait**
  * Balanced metrics → **healthy audience satisfaction**

---

### 4. 📊 Bar Chart: Title Length vs Performance
<img width="471" height="349" alt="image" src="https://github.com/user-attachments/assets/45919473-3974-4a86-a7ab-0392f3d710ff" />

* **Chart:** Total views grouped by title length
* **Insight:**

  * **Medium–Long titles perform best**
  * Short titles lack keywords
  * Very long titles get truncated (especially on mobile)

---

## 📂 Project Structure

```
├── Yt-analysis.ipynb          # Channel benchmarking and macro-ratios
├── YT-video_analysis.ipynb    # Video-level analysis & visualization
├── raw_video_data.csv         # Raw API data
├── YT_videodata.csv           # Processed dataset
└── README.md                  # Documentation
```

---

## 🛠️ Setup & Installation

### 1. Get YouTube API Key

* Visit [Google Cloud Console](https://console.cloud.google.com/)
* Create a project
* Enable **YouTube Data API v3**
* Check its [documentation](https://developers.google.com/youtube/v3)
* *Pro Tip:* Use Online JSON Parser while extracting data

---

### 2. Clone the Repository

```bash
git clone https://github.com/yourusername/youtube-analysis.git
```

---

### 3. Install Dependencies

```bash
pip install pandas seaborn matplotlib google-api-python-client
```

---

### 4. Run the Project

* Open Jupyter notebooks
* Replace `api_key` with your own key

---

## 💡 Summary of Insights

* **Quality > Quantity**
  Fewer high-quality videos → higher Subscriber Acquisition Rate

* **Engagement Lag**

  * High-view videos → lower engagement %
  * Niche videos → higher engagement

* **SEO Matters**

  * Optimal title length exists
  * Balance between keywords & readability

---

## Developed By

**[Yuvaraj Satvik]**
*Created with ❤️ by a Data Enthusiast.*

This project and the analytical approach were inspired and learned from the [techTFQ](https://www.youtube.com/@techTFQ) YouTube channel.

# 🏠 Airbnb Market Analysis (NYC 2024)— Data Cleaning, EDA, Visualizations.  

📊 **An in-depth EDA of Airbnb listings in New York City (2024)**.  
This project explores pricing dynamics, availability trends, neighbourhood patterns, and correlations across multiple features.  

---

## 📂 Project Steps  

### 1️⃣ Data Collection & Setup  
- 📑 Imported dataset: `Airbnb_dataset.csv` (NYC listings, 2024).  
- 🐍 Libraries used: `pandas`, `numpy`, `matplotlib`, `seaborn`.  
- 🔍 Initial inspection of shape, columns, and data types.  

---

### 2️⃣ Data Cleaning & Preprocessing  
- ✅ Checked and handled null values (e.g., reviews/month, host fields).  
- ✂️ Outliers Filetered at that Price<1500.  
- 🔄 Converted data types (e.g., price → numeric, neighbourhood → categorical).  

---

### 3️⃣ Feature Engineering  
- 🆕 Created **`price_per_bed = price / beds`** to normalize pricing across room capacity.  
- 📊 Added group-level summaries:  
  - Average price per borough.  
  - Price per bed per borough.  
  - Top 15 neighbourhoods by listing counts.  

---

### 4️⃣ Exploratory Data Analysis (EDA)  

#### 📈 Univariate Analysis  
- Price distribution → skewed, **mean $187.71**, long luxury tail.  
- Minimum nights → **mean 28.56**, mostly 1–2 nights.  
- Availability → **~206 days** average.  

#### 📊 Bivariate Analysis  
- **Price vs Room Type** → Entire home/apt most expensive.  
- **Price vs Borough** → Manhattan highest.  
- **Price per bed** → Manhattan = $138.7/bed vs Staten Island = $67.7/bed.  
- Count plots → Manhattan & Brooklyn dominate listing counts.  

#### 📉 Visualizations Used  
📊 Histograms | 📦 Boxplots (log scale) | 📌 Barplots | 🎻 Violin Plots | 🔍 Scatterplots (with regression) | 🌡️ Heatmap  

---

### 5️⃣ Correlation Analysis  
- 🛏️ **Price vs Beds → 0.415 (positive correlation)**  
- ✍️ **Reviews/Month vs Total Reviews → 0.631 (strong positive)**  
- 💵 **Price vs Reviews → −0.044 (weak negative)**  
- 📆 **Price vs Availability → 0.048 (almost no correlation)**  

📌 **Interpretation:** Room capacity (beds, bedrooms, baths) is the best predictor of price.  

---

### 6️⃣ Key Quantitative Insights  
- 💰 **Average Price by Borough**:  
  - Manhattan → **$204**  
  - Brooklyn → **$155**  
  - Queens → **$122**  
  - Bronx → **$108**  
  - Staten Island → **$119**  

- 🛏️ **Price per Bed by Borough**:  
  - Manhattan → **$138.7/bed** (highest)  
  - Staten Island → **$67.7/bed** (lowest)  

- 📅 **Availability** → Listings available on average **~206 days/year**.  
- ⭐ **Reviews** → Cheaper listings attract more reviews (inverse price relation).  

---

### 7️⃣ Conclusions & Next Steps  
✅ **Conclusions:**  
- Prices highly variable, driven by **location (borough)** and **room capacity**.  
- Manhattan & Brooklyn dominate both supply and pricing.  
- Reviews reflect demand but are **not a strong predictor of price**.  

---

## 📌 Tech Stack  
- **Language:** Python 🐍  
- **Libraries:** pandas | numpy | matplotlib | seaborn  

---

## 📊 Sample Visualizations  

- Univariate Analysis:
<img width="520" height="432" alt="image" src="https://github.com/user-attachments/assets/171fa4a4-2fcd-4284-960d-456408161c8c" />

<img width="704" height="470" alt="image" src="https://github.com/user-attachments/assets/9912ee2f-010d-4c79-a715-b0239113274e" />

- Bivariate Analysis:
<img width="571" height="433" alt="image" src="https://github.com/user-attachments/assets/807b2400-7234-47d9-97e6-a5f70bd907ae" />

<img width="704" height="470" alt="image" src="https://github.com/user-attachments/assets/38cd93bd-d032-4b32-97eb-a7116a0bca3a" />

<img width="1156" height="986" alt="image" src="https://github.com/user-attachments/assets/dd5a97d7-ab5a-46bb-a8b7-ae859fbb1da0" />

<img width="858" height="624" alt="image" src="https://github.com/user-attachments/assets/8c0d75e5-d3b1-456b-be64-d06e1f9a4b89" />

<img width="889" height="786" alt="image" src="https://github.com/user-attachments/assets/ce1e0c40-6577-4e21-be05-d7bddc6a27df" />

<img width="704" height="470" alt="image" src="https://github.com/user-attachments/assets/2456b2c8-f658-470a-9c01-9f0819f852df" />

<img width="635" height="470" alt="image" src="https://github.com/user-attachments/assets/45663a9c-b81e-4a57-adb5-c87e1ab04e0a" />

<img width="850" height="547" alt="image" src="https://github.com/user-attachments/assets/0beb4114-2e58-4f63-9255-19d6db6d9a16" />

<img width="977" height="878" alt="image" src="https://github.com/user-attachments/assets/810fc6ae-d38a-4cc5-9780-ee30879bfddd" />

<img width="1004" height="547" alt="image" src="https://github.com/user-attachments/assets/f4d93fbc-6c45-469b-bb1b-2fb8f1d0bb20" />

<img width="1004" height="547" alt="image" src="https://github.com/user-attachments/assets/20ab673f-7be2-496c-81ce-aac41abc4063" />

<img width="1005" height="624" alt="image" src="https://github.com/user-attachments/assets/5cf7358d-f466-4c99-9e41-eb9a7b278339" />

<img width="1189" height="690" alt="image" src="https://github.com/user-attachments/assets/1672c8ee-8ffc-45c1-92bf-402a12b430b1" />

<img width="1005" height="1009" alt="image" src="https://github.com/user-attachments/assets/fbe9ad1d-42b4-4c64-b598-c9cfc5251e66" />

<img width="859" height="624" alt="image" src="https://github.com/user-attachments/assets/73dd2c85-ebe0-43c8-9c8c-0413f7146fb2" />

<img width="1027" height="547" alt="image" src="https://github.com/user-attachments/assets/e4448b66-4e41-4201-b1c9-2588dc366de9" />

<img width="876" height="547" alt="image" src="https://github.com/user-attachments/assets/739af74a-fe44-4f41-b939-05fb8ff0ac9c" />

<img width="997" height="547" alt="image" src="https://github.com/user-attachments/assets/a3f51783-e78f-4923-8fc2-823961a786c2" />

<img width="849" height="624" alt="image" src="https://github.com/user-attachments/assets/f18780e9-82a6-402c-8a90-125d943b1011" />

<img width="1390" height="690" alt="image" src="https://github.com/user-attachments/assets/22ff922e-a8b6-4057-b530-dd90b39d572d" />

---

## 👨‍💻 Author  
👤 **Your Name**  
🔗 [LinkedIn](#) | [GitHub](#) | [Portfolio](#)  

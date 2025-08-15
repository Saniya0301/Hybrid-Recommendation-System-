# 🛍 Hybrid Recommendation System (Content + Collaborative Filtering)



## 📌 Overview
This project implements a **Hybrid Recommendation System** that combines:
1. **Content-Based Filtering** – Recommends products similar to a given product using product metadata (brand, category, color, size, etc.).
2. **Collaborative Filtering** – Suggests products based on user behavior, preferences, and ratings using the **SVD** algorithm from the `Surprise` library.

By merging both approaches, the hybrid model provides more accurate and personalized recommendations for fashion products.

---

## 📂 Dataset
**File:** `fashion_products.csv`  
The dataset contains the following columns:
- **User ID** – Unique identifier for the user
- **Product ID** – Unique identifier for the product
- **Product Name** – Name of the product
- **Brand** – Brand name
- **Category** – Product category (Men's, Women's, Kids' Fashion)
- **Price** – Price in currency units
- **Rating** – User rating (1–5 scale)
- **Color** – Product color
- **Size** – Product size (S, M, L, XL, etc.)

---

## ⚙️ Technologies & Libraries
- **Python 3**
- **Pandas** – Data handling
- **NumPy** – Numerical operations
- **Scikit-learn** – TF-IDF Vectorization & similarity computation
- **Surprise (scikit-surprise)** – Collaborative Filtering with SVD
- **Jupyter Notebook** – Development & testing

---

## 📊 Approach

### 1️⃣ Content-Based Filtering
- Combine product features (`Product Name`, `Brand`, `Category`, `Color`, `Size`) into a single string.
- Use **TF-IDF Vectorization** to convert text data into numerical vectors.
- Compute **cosine similarity** between products to find the most similar items.

### 2️⃣ Collaborative Filtering
- Use the **SVD (Singular Value Decomposition)** algorithm from `Surprise` to predict ratings for products a user hasn’t interacted with.
- Rank predictions to get top recommended products.

### 3️⃣ Hybrid Method
- Merge **content-based** and **collaborative filtering** results.
- Remove duplicates and present the top-N recommendations.

---

## 🚀 How to Run
1. **Install dependencies**  
   ```bash
   pip install pandas numpy scikit-learn scikit-surprise


   ---
  📜 License

This project is open-source and available under the MIT License.

---
Author

---
SANIYA CHHABRA

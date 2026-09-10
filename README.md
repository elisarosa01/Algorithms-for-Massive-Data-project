# 📚 Detecting Similar Book Reviews using MinHash & LSH

Pipeline to efficiently identify near-duplicate book reviews in the **Amazon Books Reviews** dataset using **MinHash** and **Locality-Sensitive Hashing (LSH)**.

### ⚙️ Architecture & Setup
- **Preprocessing:** Text cleaning, contraction handling, and custom stopword removal.
- **Shingling & Signatures:** Word-level 2-shingles, $n=100$ hash functions.
- **LSH Setup:** $b=25$ bands, $r=4$ rows per band | **Target Similarity:** $0.50 \le \text{Jaccard} \le 0.95$.

### 📈 Key Results
- **20k Reviews Sample:** 1,327 LSH candidate pairs $\rightarrow$ 111 confirmed matches within target range.
- **100k Reviews Sample (Scalability):** 11,761 candidate pairs $\rightarrow$ 706 confirmed matches.

### 🚀 Quick Start
1. Install dependencies: `pip install pandas kaggle`
2. Set your Kaggle API credentials and run `project_1.ipynb`.

**Authors:** Elisa Rosa & Mary Jane Reyes | **Course:** Algorithms for Massive Data (September 2025)

# Policy-Tech Mining for EV Battery Recycling

## 🔍 Overview

This project introduces a structured, computational approach to analyze the interaction between public policy and technological innovation, specifically in the context of Electric Vehicle (EV) battery recycling in China. We propose and implement the **Policy–Technology Interaction Matrix (PTIM)**, a seven-step methodology combining patent text mining, policy document analysis, and BM25-based term relevance scoring.

---

## 🧠 Key Contributions

- Development of the **PTIM**, a systematic matrix that maps policies to specific EV battery recycling technologies.
- Integration of patent and policy data using **text mining and similarity-based thresholding**.
- Implementation of **BM25 scoring** to assess term relevance across patents and policies.
- Demonstration of the methodology using Chinese EV battery recycling data (2011–2024).

---

## 📁 Repository Contents

- `EDA_code+TFM_code.ipynb` – Jupyter notebook for exploratory data analysis and term frequency matrix (TFM) generation.
- `sample_dataset_clean.csv` – Cleaned dataset containing sample patent and policy data.
- `T01(electric battery).csv`, `T02(electric motor).csv`, etc. – CSV files representing technology components.
- `F01(transportation).csv`, `F02(reduce emission).csv`, etc. – CSV files representing policy functions.
- `stopwords.csv` – Custom stopword list used for text preprocessing.

---

## ▶️ Running the Code

### 1. Environment Setup  
Make sure you have Python ≥ 3.8 installed. Then install the required packages:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn nltk
```

### 2. Start Jupyter Notebook  
Launch the notebook:

```bash
jupyter notebook EDA_code+TFM_code.ipynb
```

### 3. Execution Flow  
- Load and clean datasets.  
- Construct the technology and policy term libraries.  
- Compute BM25-based similarity scores.  
- Generate the Policy–Technology Interaction Matrix (PTIM).  
- Visualize results and rankings.

---

## 📊 Data Sources

- **Patent Data**: China Intellectual Property Office via IncoPat (2011–2024)
- **Policy Documents**: China National Policy Database & Local Policy Documents (Shenzhen, Beijing, Shanghai)
- Sample data included; full dataset can be licensed via [IncoPat](https://www.incopat.com)

---

## 📜 Citation

If you find this work useful, please cite our paper:

```bibtex
@inproceedings{govindarajan2025policytech,
  title={A Methodological Mining Approach to Policy-Technology Interaction: An Application of EV Battery Recycling in China},
  author={Govindarajan, Usharani Hareesh and Hong, Yuecheng and Narang, Gagan and Sospiro, Paolo},
  booktitle={Proceedings of the 34th ACM International Conference on Information and Knowledge Management (CIKM)},
  year={2025},
  location={Seoul, South Korea},
  publisher={ACM}
}
```

---

## 🤝 Acknowledgements

This research was supported by the **National Natural Science Foundation of China (NSFC)** under Grant Number **W2433177**, in the discipline of Management Science and Engineering (2025–2026).  
We also thank the University of Shanghai for Science and Technology for their institutional support.

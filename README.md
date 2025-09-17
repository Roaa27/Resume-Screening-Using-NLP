# 📂 Resume Screening using NLP

This project is part of my Elevvo Internship (NLP Track).  
The goal is to build a system that automatically screens and ranks resumes against job descriptions.

---

## 📌 Project Steps

Step 1: Install and Import Libraries  
Installed SentenceTransformers, Scikit-learn, and Pandas.

Step 2: Load Dataset  
Loaded resumes and job descriptions from CSV files.

Step 3: Load Embedding Model  
Used all-MiniLM-L6-v2 model to generate semantic embeddings.

Step 4: Encode Texts  
Converted resumes and job descriptions into embeddings.

Step 5: Compute Similarity  
Calculated cosine similarity to measure resume-job match scores.

Step 6: Rank Resumes  
Ranked resumes for each job and selected the top matches.

Step 7: Example Output  
Displayed the top resumes with match scores and excerpts.

---

## 📊 Example Results
🔹 Job: Data Analyst
resume_id   match_score   resume_excerpt
CV_12       87.45         Experienced data analyst skilled in SQL, Python, and Tableau…
CV_07       83.20         Data science graduate with strong background in statistics…
CV_19       81.50         Business intelligence specialist with 3 years of experience…

---

## 🛠️ Tools & Libraries Used

- Python  
- Pandas  
- SentenceTransformers  
- Scikit-learn  

---


pip install sentence-transformers scikit-learn pandas

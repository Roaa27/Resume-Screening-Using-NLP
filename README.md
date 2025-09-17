# 🧑‍💼 Resume Screening Using NLP

## 📌 Project Overview
This project implements an AI-powered resume screening system using Natural Language Processing (NLP).  
The system compares resumes against job descriptions and ranks them based on their semantic similarity.  
It leverages transformer-based embeddings to understand the meaning of text rather than just keyword matching.

---

## 🎯 Objectives
- Preprocess resumes and job descriptions.
- Generate embeddings using a pre-trained Sentence Transformer model.
- Compute similarity scores between resumes and jobs.
- Rank resumes for each job and display the top matches.
- Provide excerpts from resumes as justifications for the match.

---

## 📊 Dataset
Two datasets were used:
1. UpdatedResumeDataSet.csv → contains candidate resumes with a Category and Resume text.  
2. job_descriptions_sample.csv → sampled job descriptions containing fields like Job Title and Job Description.

> ⚡ Note: A sampled job dataset was used instead of the full one to reduce runtime in Google Colab.

---

## 🛠️ Tools & Libraries
- Python  
- Pandas → Data loading & processing  
- Sentence Transformers → Pre-trained model (`all-MiniLM-L6-v2`) for embeddings  
- Scikit-learn → Cosine similarity computation  

---

## 📂 Project Structure
```plaintext
├── Resume_Screening.ipynb   # Main notebook
├── UpdatedResumeDataSet.csv # Resume dataset
├── job_descriptions_sample.csv # Job descriptions sample dataset
└── README.md                # Project documentation
🚀 Workflow
 1. Load datasets → Resumes & Jobs.
 2. Inspect columns → Identify useful fields (Resume, Job Description, Job Title).
 3. Load transformer model → all-MiniLM-L6-v2.
 4. Convert text to embeddings → Numerical vector representation.
 5. Compute cosine similarity → Measure how close resumes are to job descriptions.
 6. Rank resumes → Select top 3 matches per job.
 7. Display results → Show job title, resume ID, match score, and resume excerpt.
📈 Sample Results

Example output for two job descriptions:

🔹 Job: Digital Marketing Specialist
 resume_id  match_score  resume_excerpt
       259        26.84  Skill Sets: • Multi-tasking • Collaborative • Optimistic Thinking...

🔹 Job: Web Developer
 resume_id  match_score  resume_excerpt
       335        47.25  TECHNICAL SKILLS Skills: Java, SQL, PL/SQL, C, C++, BootStrap...
🧪 Future Improvements
 • Fine-tune the model on resume-job matching tasks.
 • Extract named entities (skills, experience) from resumes using NER.
 • Build a Streamlit web app to upload resumes and see matching results in real-time.

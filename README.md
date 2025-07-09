
# 🩺 Medical Notes Summarizer

This project leverages state-of-the-art **NLP techniques** to generate **structured and unstructured summaries** from patient-doctor conversations. It is designed to help **doctors** efficiently review key points from consultations, enabling better memorization and record-keeping.

---

## ✨ Features

- 🔍 **Abstractive summarization** of medical conversations  
- 🧠 Uses **transformer-based models** (e.g., BART/T5) for natural summaries  
- 🏥 Outputs both **free-form summaries** and **structured data** (e.g., symptoms, diagnosis)  
- ⚙️ Lightweight **Flask app** for easy local deployment and testing  

---

## 🧪 Use Case

Doctors often face information overload during patient interactions. This summarizer assists by:
- Creating quick medical briefings post-consultation  
- Reducing documentation time  
- Helping recall key details from lengthy or multi-patient sessions  

---

## 🛠️ Tech Stack

- **Python 3.10+**
- **Hugging Face Transformers**  
- **Flask** (for `app.py`)  
- **Pandas**, **NLTK**, **Scikit-learn**  
- Jupyter Notebooks for exploration and prototyping

---

## 📁 Project Structure

```
├── Medical_Summarizer_NLP_project(1).ipynb   # Main summarization logic
├── NLP_project.ipynb                         # Preprocessing and model comparison
├── app.py                                    # Flask app for summary generation
├── README.md                                 # You are here!
```

---

## 🚀 Getting Started

### 1. Clone the Repo
```bash
git clone https://github.com/yourusername/medical-notes-summarizer.git
cd medical-notes-summarizer
```

### 2. Run the App
```bash
python app.py
```

---

## 🧠 Example Input

> **Doctor:** "So you mentioned you've had chest pain for three days?"  
> **Patient:** "Yes, and sometimes it spreads to my arm. I also feel shortness of breath."

### 🔽 Output Summary

**Unstructured Summary:**  
> Patient reports chest pain for 3 days, radiating to the arm, with associated shortness of breath.

**Structured Output:**
```json
{
  "symptoms": ["chest pain", "radiating arm pain", "shortness of breath"],
  "duration": "3 days"
}
```

---

## 📌 Future Work

- Integrate named entity recognition for structured ICD-10 tagging  
- Add real-time transcription from speech  
- Improve fine-tuning with clinical datasets (e.g., MIMIC-III, AG-Bonnet)  
- Add UI frontend for hospital use-case simulation

---

## 🤝 Acknowledgements

This project was built as part of an independent study and passion for NLP in healthcare, with the goal of making medical communication more accessible and actionable.

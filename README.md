# Bank_check_OCR
An end-to-end intelligent cheque information extractor using Google Vision OCR + OpenAI GPT-4. It extracts key fields like payee name, amount, date, account number, IFSC, MICR, etc., from scanned bank cheques and exports them to Excel automatically. Ideal for document automation in financial workflows.
# 🧾 Intelligent Cheque OCR Parsing Pipeline

This project automates cheque information extraction from scanned images using Google Cloud Vision OCR and OpenAI GPT-4 for intelligent parsing.

---

## 🚀 What It Does

- 📥 Accepts a ZIP file of scanned cheque images
- 🔍 Uses Google Vision API for text extraction (OCR)
- 🧠 Parses key fields using OpenAI GPT-4:
  - Payee Name
  - Date
  - Amount in Numbers
  - Account Number
  - IFSC Code
  - Bank Name
  - MICR Code
  - Cheque Number
- 📊 Outputs clean Excel sheet for further use

---

## 🛠️ Tech Stack

| Tool            | Purpose                         |
|-----------------|----------------------------------|
| Python          | Core programming language        |
| Google Vision   | OCR from cheque images           |
| OpenAI GPT-4    | Intelligent structured parsing   |
| Pandas          | Data wrangling and Excel export  |

---

## 📁 How to Use

1. **Upload a ZIP** containing cheque images (`.png`, `.jpg`, etc.)
2. **Place your Vision API key** as `VisionApiKey.json`
3. **Set OpenAI Key** via `.env` or `os.environ`
4. **Run the notebook** or Python script
5. 🎉 Parsed Excel (`parsed_cheques_final.xlsx`) will be saved

---

## 📌 Output Example

| Payee Name        | Amount in Numbers | Date       | IFSC Code     | Cheque Number |
|-------------------|-------------------|------------|----------------|----------------|
| Kumar Ravi Palli  | 2,223,000/-       | 29-06-12   | ICIC0006308   | 551452         |
| Dinesh Veniola    | 51,000,000        | 15-01-2015 | UTIB0000426   | 426160         |

---

## ✅ Use Cases

- Automating back-office cheque processing
- Financial document digitization
- Training AI on document parsing tasks

---

## 📜 License

This project is for educational and demonstration purposes.

---

## 💸 Costing Per Cheque (Approx.)

| Component              | API Used          | Cost (in ₹) | Notes                                      |
|------------------------|-------------------|-------------|--------------------------------------------|
| OCR Text Extraction    | Google Vision API | ₹0.11       | `document_text_detection` mode             |
| Field Parsing (AI)     | OpenAI GPT-3.5    | ₹0.90       | Based on average ~600 tokens per cheque    |
| **Total Per Cheque**   | —                 | **₹1.01**   | 45% cheaper than typical ₹1.80 market rate |

> ✅ You can reduce cost further by optimizing prompts and batch processing.


---

## 📁 Output Example

| Payee Name     | Date     | Amount    | IFSC Code   | Cheque Number |
|----------------|----------|-----------|-------------|----------------|
| Ravi Kumar     | 29-06-12 | 2,23,000  | ICIC0006308 | 551452         |

---

## 📦 How to Use

1. Upload cheque images in a `.zip` file.
2. Set up Vision API key as `VisionApiKey.json`.
3. Set `OPENAI_API_KEY` in `.env` or environment.
4. Run the pipeline.
5. Output Excel will be saved as `parsed_cheques_final.xlsx`.

---

## 🔒 Notes

- API keys are **not** included in this repo.
- Add `VisionApiKey.json` and `.env` to `.gitignore`.

---

## 🙌 Acknowledgements

- Google Cloud Vision API
- OpenAI GPT-4
- Dataset: [IDRBT Cheque Image Dataset](https://github.com/naikshubham/Bank-Cheque-OCR)

---

## 🧠 Author

**Sharada Sonaje**  
_ML Intern | Data Analyst | Psychology PG Student_  

# Resume Screening AI

This project is a **Flask-based Resume Screening Application** that analyzes uploaded resumes and extracts useful information such as:

- **Resume Categorization**
- **Job Recommendation based on Resume**
- **Resume Parsing** (extracting name, contact details, skills, and education)

## Features

- **Upload Resumes in PDF or TXT format**
- **Extract Contact Details** (Phone number and Email)
- **Identify and Extract Key Skills**
- **Predict Resume Category**
- **Recommend Suitable Jobs**
- **Extract Educational Background**

## Demo
https://resume-parser-a4ze.onrender.com
![image](https://github.com/user-attachments/assets/46c2e267-8ee4-4319-98d5-b4038157750b)



## Tech Stack

- **Backend**: Flask (Python)
- **Frontend**: HTML, CSS
- **Machine Learning**: Random Forest Classifier, TF-IDF Vectorizer
- **Libraries Used**:
  - Flask
  - pypdf (for PDF parsing)
  - re (for regex-based parsing)
  - pickle (for loading ML models)

## Setup Instructions

1. **Clone the Repository**

   ```bash
   git clone https://github.com/your-username/resume-screening-ai.git
   cd resume-screening-ai
   ```

2. **Create a Virtual Environment & Install Dependencies**

   ```bash
   python3 -m venv venv
   source venv/bin/activate  # For Windows: venv\Scripts\activate
   pip install -r requirements.txt
   ```

3. **Ensure the Model Files are in Place**

   - Place the trained model files inside the `models/` directory:
     - `random_forest_model.pkl`
     - `tfidf_vectorizer.pkl`
     - `rf_clsi_job.pkl`
     - `vectorizer_job_rec.pkl`

4. **Run the Application**

   ```bash
   python app.py
   ```

5. **Open the Application in Your Browser**

   - Visit: `http://127.0.0.1:8080/`

## Project Structure

```
resume-screening-ai/
│── models/                  # Pre-trained ML models
│── templates/
│   ├── resume.html          # Frontend UI
│── app.py                   # Main Flask application
│── requirements.txt         # Required dependencies
│── README.md                # Project documentation
```

## How It Works

1. **Upload Resume** (PDF/TXT format).
2. **AI Model Processes the Resume**.
3. **Extracted Information is Displayed**:
   - Name
   - Phone Number
   - Email
   - Skills
   - Education
   - Predicted Job Category
   - Recommended Job

## Future Enhancements

- Add support for more file formats (DOCX, ODT, etc.).
- Improve model accuracy with additional training data.
- Integrate an interactive UI for better user experience.

## License

This project is licensed under the MIT License.

## Author

Developed by **Ankush Chaudhary**. Contributions are welcome!


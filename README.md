
# SGPA & CGPA Result Generator Web App

This is a Flask-based web application that calculates and displays a student's SGPA and CGPA based on Excel data. Designed for use by engineering colleges or students managing their academic performance.

---

## 🚀 Features

- Upload-free access using preloaded Excel data
- Calculate SGPA & CGPA using subject-wise grade points
- View result with detailed subject list and grade table
- Simple and elegant HTML/CSS frontend
- Fully ready for deployment on Render or any other platform

---

## 📁 Project Structure

```
dilip/
├── app.py                 # Flask application entry point
├── logic.py               # Contains grade calculation logic
├── students_results.xlsx  # Academic data in Excel format
├── requirements.txt       # Python dependencies
├── templates/
│   ├── index.html         # Input form
│   └── result.html        # Display result
├── static/                # CSS or JS assets (optional)
```

---

## ⚙️ Requirements

- Python 3.7+
- Flask
- pandas
- openpyxl

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## 🧠 How it Works

1. User enters `Roll Number`
2. App looks up the corresponding row in `students_results.xlsx`
3. Grades are mapped to grade points using the scheme:
    - A+: 10, A: 9, B: 8, C: 7, D: 6, E: 5, F/AB: 0
4. SGPA/CGPA are calculated and shown on the result page

---

## ▶️ Run Locally

```bash
python app.py
```

Then open [http://localhost:5000](http://localhost:5000) in your browser.

---

## 🌐 Deploy to Render (Free Hosting)

**Build Command**:
```
pip install -r requirements.txt
```

**Start Command**:
```
gunicorn app:app
```

---

## 👤 Author

- **Dilip Kumar Y**
- 4th Year ECE

---

## 📜 License

This project is free to use for academic/non-commercial purposes.

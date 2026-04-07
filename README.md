# 📅 Invigilation Timetable System

A web-based system for automatically scheduling exam invigilators based on their availability and exam requirements.

🌐 **Live Demo:** [https://automated-invigilation-time-table.onrender.com](https://automated-invigilation-time-table.onrender.com)

---

## 🚀 Features

- Upload exam and invigilator schedules in CSV format
- Automatic allocation of invigilators based on availability
- Download complete schedule in Excel format
- View assignment statistics and summary
- Sample files provided for reference

---

## 🛠️ Setup Instructions (Local)

1. **Clone the repository:**
```bash
git clone https://github.com/NIKHITHA-99/Automated-invigilation--time-table-.git
cd Automated-invigilation--time-table-
```

2. **Create a virtual environment:**
```bash
python -m venv venv
venv\Scripts\activate        # On Windows
source venv/bin/activate     # On Mac/Linux
```

3. **Install dependencies:**
```bash
pip install -r requirements.txt
```

4. **Run the application:**
```bash
python app.py
```

5. **Open your browser and navigate to:**
```
http://localhost:5000
```

---

## 📂 File Format Requirements

### Exam Schedule (CSV)
```csv
day,date,subject,form,start_time,duration,required
Monday,01-Jan,Mathematics,5A,09:00,2,2
Monday,01-Jan,History,4B,14:00,1.5,1
Tuesday,02-Jan,Science,5B,11:00,1.5,2
Tuesday,02-Jan,Chemistry,6A,09:00,2,3
Wednesday,03-Jan,English,5C,14:00,1,1
Wednesday,03-Jan,Physics,6B,09:00,2,2
```

### Invigilator Schedule (CSV)
```csv
initial,max_hours,monday,tuesday,wednesday,thursday,friday
TCH1,15,09:00-16:00,09:00-16:00,09:00-16:00,09:00-16:00,09:00-16:00
TCH2,10,09:00-12:00,09:00-12:00,09:00-12:00,,
TCH3,8,13:00-16:00,13:00-16:00,13:00-16:00,,
TCH4,2,09:00-12:00,09:00-12:00,09:00-12:00,
```

---

## 📝 Notes

- Times should be in 24-hour format (HH:MM)
- Duration is in hours (can be decimal, e.g., 1.5 for 1 hour 30 minutes)
- Weekly schedule should use time ranges (e.g., 09:00-12:00)
- The app is hosted on Render free tier — first load may take up to 50 seconds

---

## 🧰 Tech Stack

- **Backend:** Python, Flask
- **Data Processing:** Pandas
- **Export:** XlsxWriter
- **Server:** Gunicorn
- **Deployment:** Render

---

## 👩‍💻 Author

**Nikhitha** — [GitHub](https://github.com/NIKHITHA-99)
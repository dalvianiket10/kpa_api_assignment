# 🚆 Bogie Checksheet API Assignment

## 👨‍💻 Developed by: Aniket Dalvi

---

## 📌 Assignment Overview

This project demonstrates backend API development for a Bogie Checksheet system using **Django REST Framework** and **PostgreSQL**. The objective was to implement multiple APIs that allow creating, retrieving, and deleting bogie inspection forms. These APIs are tested with Postman and can integrate with the provided Flutter frontend.

---

## 🔧 Technologies Used

- **Framework**: Django REST Framework (DRF)
- **Language**: Python
- **Database**: PostgreSQL
- **Testing Tool**: Postman
- **Environment Configuration**: `.env` file
- **IDE**: Visual Studio Code
- **Version Control**: Git

---

## 🚀 Implemented APIs

1. **POST** `/api/forms/submit`  
   → Submits a new bogie inspection form, including BMBC checksheet, bogie details, and bogie checksheet.

2. **GET** `/api/forms/get-all`  
   → Retrieves all stored forms.

3. **GET** `/api/forms/get/<formNumber>`  
   → Fetches a specific form using its `formNumber`.

4. **DELETE** `/api/forms/delete/<formNumber>`  
   → Deletes a form by `formNumber`.

All APIs return appropriate HTTP status codes (`200 OK`, `201 Created`, `204 No Content`, `404 Not Found`).

---

## 📂 Project Structure

kpa_api_assignment/
├── backend_api/
│ ├── manage.py
│ ├── requirements.txt
│ ├── README.md
│ ├── .env.example
│ ├── backend_api/
│ │ ├── init.py
│ │ ├── settings.py
│ │ ├── urls.py
│ │ └── wsgi.py
│ └── core/
│ ├── init.py
│ ├── models.py
│ ├── serializers.py
│ ├── views.py
│ ├── urls.py
│ └── tests.py
└── KPA_form_data.postman_collection.json


---

## ⚙️ Setup Instructions

1. **Clone or Download the Project**

2. **Create Virtual Environment**

python -m venv venv
venv\Scripts\activate # On Windows
source venv/bin/activate # On Linux/Mac


3. **Install Dependencies**

pip install -r requirements.txt


4. **Configure PostgreSQL**
- Create a PostgreSQL database
- Update the `.env` file with your DB credentials

5. **Run Migrations**

python manage.py makemigrations
python manage.py migrate


6. **Start Server**

python manage.py runserver


7. **Test with Postman**
- Base URL: `http://127.0.0.1:8000`

---

## 🧪 API Testing Summary

- All endpoints tested with Postman
- Used sample data provided in the assignment
- Verified correct data storage in PostgreSQL
- Confirmed integration with Flutter frontend

---

## 📝 Postman Collection

- File: `KPA_form_data.postman_collection.json`
- Contains:
- `POST /api/forms/submit`
- `GET /api/forms/get-all`
- `GET /api/forms/get/<formNumber>`
- `DELETE /api/forms/delete/<formNumber>`
- Successfully tested with expected inputs and outputs

---

## 🎥 Screen Recording

Uploaded a 3-minute screen recording demonstrating:
- Code explanation (models, views, serializers)
- API testing in Postman
- Folder structure and technologies used

**File Name**: `AniketDalvi_backend_assignment.mp4`  
**Link**: [https://drive.google.com/file/d/16vw1U7Il4P2nS2FX085n2s42IBgXKczu/view?usp=sharing]

---

## 📤 Submission Checklist

✅ Source Code (GitHub or Drive ZIP):  
https://drive.google.com/file/d/1HA3XG74SxZjp1tpitfH37IvKYRrH4rpL/view?usp=sharing

✅ Postman Collection:  
https://drive.google.com/file/d/1T6VzSwgpSN3fkcqgZKENk9-AJKzT3FH1/view?usp=sharing

✅ README File:  
https://drive.google.com/file/d/1qk2WN7dLOUIRHiA-5S08ftiyNxAkYOe3/view?usp=sharing

✅ Screen Recording:  
https://drive.google.com/file/d/16vw1U7Il4P2nS2FX085n2s42IBgXKczu/view?usp=sharing

📧 Send all links to `contact@suvidhaen.com`

---

## 📝 Notes

- Used Django Models and Serializers for input validation
- Configured settings with `.env` for cleaner deployment
- Error-handling for missing formNumbers and empty submissions
- Unused/extra GET method (405 error) was removed to avoid confusion

---

## 🙌 Thank You!

I appreciate the opportunity to work on this assignment and showcase my Django backend skills. Looking forward to your feedback!


# ATM Interface Project

This project is a full-stack **ATM Interface Simulation**, developed as part of an academic project. It mimics the workflow of an ATM machine, from user login to performing transactions like withdrawal, balance inquiry, PIN change, and mini statement generation. This application uses **Python**, **Flask**, **MySQL** for the backend, and **HTML/CSS/JS** for the frontend.

## 🌟 Features

- 🔐 User Login (Authentication)
- 🌐 Language Selection (Default: English)
- 💳 Account Type Selection (Savings / Current / Credit)
- 💰 Transaction Types:
  - Withdrawal
  - Check Balance
  - Change ATM PIN
  - Mini Statement
- 🧠 PIN Verification

## 🛠️ Tech Stack

- **Backend:** Python, Flask
- **Frontend:** HTML, CSS, JavaScript
- **Database:** MySQL
- **Testing:** JUnit (for backend)
- **Version Control:** Git & GitHub

## 📂 Project Structure
   atm-interface/
    │
    ├── app.py # Main Flask app
    ├── templates/ # HTML templates
    │ ├── login.html
    │ ├── dashboard.html
    │ └── ...
    ├── static/ # CSS, JS, images
    ├── db_config.py # MySQL DB connection setup
    ├── database/
    │ └── schema.sql # SQL script to create tables
    ├── README.md
    └── requirements.txt # Python dependencies

## ⚙️ Getting Started

### ✅ 1. Clone the Repository

```bash
git clone https://github.com/your-username/atm-interface.git
cd atm-interface

### ✅ 2. Create & Activate Virtual Environment
bash
Copy
Edit
python -m venv venv
source venv/bin/activate      # On Windows: venv\Scripts\activate

### ✅ 3. Install Required Libraries
bash
Copy
Edit
pip install -r requirements.txt
✅ 4. Setup MySQL Database
Open MySQL and create a new database:

sql
Copy
Edit
CREATE DATABASE atm_db;
Run the schema file to create tables and insert sample data:

bash
Copy
Edit
mysql -u your_user -p atm_db < database/schema.sql
✅ 5. Configure DB in db_config.py
python
Copy
Edit
db_config = {
    'host': 'localhost',
    'user': 'your_mysql_user',
    'password': 'your_mysql_password',
    'database': 'atm_db'
}
✅ 6. Run the Flask App
bash
Copy
Edit
python app.py
Now open your browser and visit: http://localhost:5000

🔑 Sample Login Credentials (for Testing)
Username	Password	PIN
user1	pass123	1234
user2	pass456	5678

You can add or modify users directly in the database using SQL or phpMyAdmin.

📦 requirements.txt
text
Copy
Edit
Flask
mysql-connector-python
📌 Future Enhancements
Multilingual UI

OTP-based login security

Mobile-responsive interface

Cloud deployment (Render / Heroku)

REST API integration for mobile clients

👩‍💻 Author
Manasa
B.Tech CSE Student, RV University, Bengaluru

📜 License
This project is for academic and educational use only.

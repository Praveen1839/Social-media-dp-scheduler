# Social media DP Scheduler (Semi-Automated)

A simple Flask + Selenium-based web tool to help schedule and manage Instagram display picture (DP) changes.  
Since Instagram restricts profile picture uploads via automation, this project assists the user in navigating directly to the profile edit screen, where they can manually update the DP with ease.

---

# Features

- Upload DP image from a local file
- Set a target schedule time (for tracking/logging)
- Store Instagram credentials locally for automation
- View a history of all scheduled DP entries
- Automatically open Instagram and navigate to the Edit Profile page
- Simple and clean web UI using Flask + HTML

---

##  How It Works

1. Run the Flask web server using `app.py`
2. Access the form at `http://127.0.0.1:5000`
3. Enter:
   - Instagram username
   - Password
   - Upload a DP image
   - Set a schedule time
4. Submission is stored in `schedule.json`
5. Run `dp_changer.py` to:
   - Log into Instagram
   - Go to the Edit Profile page
   - Prompt you to manually upload the image

---

## Tech Stack

- **Python 3**
- **Flask** for web backend
- **HTML/CSS** for frontend UI
- **Selenium (Chrome WebDriver)** for browser automation
- **JSON** for schedule and login data storage

---

## 📂 Project Structure

instagram-dp-scheduler/
├── app.py # Flask web app
├── dp_changer.py                        # Selenium script to navigate Instagram
├── requirements.txt                    # Dependencies
├── schedule.json                        # Auto-generated JSON storing entries
├── templates/
│ └── index.html                     # Web form UI
└── static/
└── uploads/                         # Uploaded images
 
copy the code from the github

1.Install dependencies

pip install -r requirements.txt
Make sure you have Chrome WebDriver installed and it's compatible with your browser version.

2.Run the Flask server

python app.py
python app.pyOpen your browser and go to http://127.0.0.1:5000

3.Run the automation script

python dp_changer.py

This will:
Open Instagram
Login
Take you to the profile page
Ask you to upload the selected DP manually

⚠️ Disclaimer
This project is built for educational and personal purposes.
Automating Instagram actions can violate Instagram’s Terms of Use.
Use a fake/test account. Do not use your main Instagram profile.

📄 License
This project is licensed under the MIT License.

👤 Author
Vadthya Praveen
🎓 Student @ AVN Institute of Engineering and Technology

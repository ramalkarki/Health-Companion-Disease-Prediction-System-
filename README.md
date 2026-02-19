# Health Companion: AI-Powered Disease Prediction System

Health Companion is a digital platform designed for early health awareness through intelligent symptom analysis. Using advanced Machine Learning, the system predicts potential illnesses based on user-reported symptoms to encourage proactive care. It also includes a secondary directory of local healthcare facilities to help users find support in their area.
## Key Features
* **AI Disease Prediction:** The core of the system. It uses a Voting Classifier model to analyze symptoms and provide instant health insights.
* **Symptom Analysis:** Users can select multiple symptoms to receive a high-probability health prediction.
* **Hospital Directory:** A supporting feature that lists hospitals in Kathmandu with registration details and descriptions.
* **Admin Management:** Secure access (admin@admin.com) to update hospital information and manage the platform database.

---

## Technology Stack
* **AI/ML Backend:** Python 3.x using Flask Framework.
* **Machine Learning:** Scikit-learn (Random Forest, SVM, Logistic Regression, Multinomial NB, Voting Classifier).
* **Web Frontend:** HTML5, CSS3, and JavaScript.
* **Web Backend:** PHP.
* **Database:** MySQL (XAMPP).

---

## Project Structure
* `app.py` / `predict.py` - The AI Engine: Handles the logic for processing symptoms and returning ML predictions.
* `*.pkl` - Pre-trained Machine Learning models (The "Brain" of the system).
* `homepage.php` - Main dashboard featuring the AI prediction interface and hospital listings.
* `addhospital.php` - Admin tool for adding healthcare data to the database.
* `login.php` & `signup.php` - User authentication system.

---

## Installation & Setup

### 1. Python AI Setup (Mandatory)
1. Open your terminal in the project folder.
2. Install the necessary AI libraries:
   ```bash
   pip install flask scikit-learn pandas numpy



3. Run the AI server:
```bash
python app.py

```


*Note: The prediction feature requires this script to be running in the background.*

### 2. Database & Web Setup

1. Start **Apache** and **MySQL** in XAMPP.
2. Create a database named `hospitals_db` in `phpMyAdmin`.
3. Import the required SQL tables (`hospital`, `signup`, `bookedhospital`).
4. Move the project to `C:\xampp\htdocs\health_companion`.
5. Open: `http://localhost/health_companion/login.php`.

---

## Admin Access

To manage hospital data:

* **Email:** admin@admin.com
* **Password:** (Your admin password)

---

## Disclaimer

This system is an educational project focusing on Machine Learning applications in healthcare. The predictions provided are for informational purposes only and are not a substitute for professional medical advice, diagnosis, or treatment.

# 📱 Mobile Price Range Prediction – ML Project

This is a machine learning-based web application that predicts the price range of a mobile phone (0 to 3) based on features like RAM, battery power, screen size, and more. The model uses Logistic Regression and is served using Flask, with a simple HTML interface for user interaction.


## 🚀 Demo

Dataset 
![image](https://github.com/user-attachments/assets/1bf366ea-befc-443a-bd8e-7f99ac3f622e)
🎥 Click the image below to watch the demo video (hosted on YouTube or Google Drive):

[![Watch Demo](https://img.youtube.com/vi/YOUR_VIDEO_ID_HERE/0.jpg)](https://www.youtube.com/watch?v=YOUR_VIDEO_ID_HERE)

> 💡 _Not deployed online — this video demonstrates how the app works locally._

---

## 🧠 Model Information

- **Model Type:** Logistic Regression
- **Target:** `price_range` (0 = Low, 1 = Medium, 2 = High, 3 = Very High)
- **Training File:** `phone_prediction.ipynb`
- **Deployed Model:** `LogisticModel.pkl`

---

## 🧾 Features Used

| Field Name      | Label                 | Type         | Min | Max  | Notes                    |
| --------------- | --------------------- | ------------ | --- | ---- | ------------------------ |
| `battery_power` | Battery Power (mAh)   | Number       | 500 | 2000 | Realistic phone battery  |
| `blue`          | Bluetooth             | Select (0/1) | —   | —    | 1 = Yes, 0 = No          |
| `clock_speed`   | Clock Speed (GHz)     | Float        | 0.5 | 3.0  | e.g., 1.5 GHz            |
| `dual_sim`      | Dual SIM              | Select (0/1) | —   | —    | 1 = Yes, 0 = No          |
| `four_g`        | 4G Support            | Select (0/1) | —   | —    | 1 = Yes, 0 = No          |
| `three_g`       | 3G Support            | Select (0/1) | —   | —    | 1 = Yes, 0 = No          |
| `fc`            | Front Camera (MP)     | Number       | 0   | 20   | MP (can be 0 if none)    |
| `int_memory`    | Internal Memory (GB)  | Number       | 2   | 64   | Storage                  |
| `m_dep`         | Mobile Depth (cm)     | Float        | 0.1 | 1.0  | Depth in cm              |
| `mobile_wt`     | Mobile Weight (grams) | Number       | 80  | 200  | Typical phone weight     |
| `n_cores`       | Processor Cores       | Number       | 1   | 8    | Number of cores          |
| `pc`            | Primary Camera (MP)   | Number       | 0   | 20   | MP                       |
| `px_height`     | Pixel Height (px)     | Number       | 0   | 1960 | Screen resolution height |
| `px_width`      | Pixel Width (px)      | Number       | 500 | 2000 | Screen resolution width  |
| `ram`           | RAM (MB)              | Number       | 256 | 4000 | Memory in MB             |
| `sc_h`          | Screen Height (cm)    | Number       | 5   | 20   | Screen height            |
| `sc_w`          | Screen Width (cm)     | Number       | 0   | 18   | Screen width             |
| `talk_time`     | Talk Time (hours)     | Number       | 2   | 20   | Max supported talk time  |
| `touch_screen`  | Touch Screen          | Select (0/1) | —   | —    | 1 = Yes, 0 = No          |
| `wifi`          | WiFi                  | Select (0/1) | —   | —    | 1 = Yes, 0 = No          |

---

## 🧪 Sample Prediction (From Dataset)

The app correctly predicts price range values from real rows in the dataset:

| Input Row | Predicted Price Category |
|-----------|--------------------------|
| Row 1     | 0 → Low Cost             |
| Row 2     | 1 → Medium Cost          |
| Row 3     | 2 → High Cost            |
| Row 4     | 3 → Very High Cost       |

These cases are shown in the demo video.

---
## 🛠️ How to Run the App

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/phone-price-predictor.git
   cd phone-price-predictor
2. **Create virtual environment (optional)**
   ```bash 
    python -m venv venv
    source venv/bin/activate  # Mac/Linux
    venv\Scripts\activate     # Windows
3. **Install dependencies**
   ```bash 
      pip install -r requirements.txt
4. **Run the Flask app**
   ```bash 
      python main.py
5. **Visit in browser**
Go to : http://127.0.0.1:5000
  





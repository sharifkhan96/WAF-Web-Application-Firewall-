

# 🛡️ Web Application Firewall (WAF) with Machine Learning Integration

Welcome to the repository of our **Final Year Project (FYP)**! This project showcases the development of a **Web Application Firewall (WAF)** with **Machine Learning** capabilities, aimed at protecting websites from common web attacks like **SQL Injection (SQLi)** and **Cross-Site Scripting (XSS)**.

---

## 🔑 Key Features

- **Machine Learning Model**: Trained using the **Random Forest algorithm**, achieving **90% accuracy** in detecting anomalous or benign traffic.
- **Web Technologies**: Integrated with **ModSecurity**, **DVWA** hosted locally on **NGINX** running on **Ubuntu OS** for real-time traffic analysis.
- **Tested on DVWA**: The ML-powered WAF was tested using the **Damn Vulnerable Web Application (DVWA)** to simulate attacks and measure the firewall’s effectiveness.
- **Real-Time Traffic Detection**: The model communicates with ModSecurity to detect and mitigate **SQLi** and **XSS** attacks dynamically.
- **Django Web Application**: ML model deployed using a web interface built with **Django** and **JavaScript**, providing real-time insights and security alerts via a dashboard.

---

## 📂 Project Structure

- **/ml_model**: Contains the trained machine learning model and code for traffic classification.
- **/django_app**: The Django-based web application integrated with ModSecurity to process and display security logs.
- **/nginx_modsecurity_setup**: Configuration files for setting up ModSecurity with NGINX on Ubuntu.
- **/dvwa_testing**: Scripts and notes from the testing phase using DVWA.

---

## 🛠️ Installation & Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/WAF-ML-FYP.git
   ```
2. Install the necessary dependencies:
   ```bash
   sudo apt-get update
   sudo apt-get install nginx modsecurity python3-pip
   pip3 install -r requirements.txt
   ```
3. Configure NGINX and ModSecurity by following the guide in the `nginx_modsecurity_setup/` directory, or https://blog.nginx.org/blog/compiling-and-installing-modsecurity-for-open-source-nginx
4. Train the model or use the pre-trained model from the `ml_model/` directory.

---

## 🚀 How It Works

1. **Traffic Flow**: Incoming web traffic is routed through **DVWA** hosted locally on **NGINX** to **ModSecurity**, then to Django app on which ML trained model is deployed locally.
2. **Traffic Classification**: ModSecurity logs are passed to the **Django application**, where the **Machine Learning model** classifies the traffic as either **malicious** or **benign**.
3. **Alerts & Actions**: If malicious traffic is detected (e.g., SQLi or XSS), the system triggers appropriate actions like logging, alerts, or blocking the request.

---

## 🔬 Testing & Results

The system was tested using **DVWA** to simulate web attacks:
- **SQL Injection (SQLi)**: x% success rate in detection.
- **Cross-Site Scripting (XSS)**: x% success rate in detection.
- **Overall Accuracy**: 90% accuracy using the Random Forest algorithm.

---

## 🧑‍💻 Contributors

- **Sharif Danish** (Team Lead, AI/ML model trainer, & Security Tester)
- **Abidullah Nasiri** (Backend & Frontend Developer)
- **Ismail Karimi** (Documentation)

---

## 📝 License

This project is not yet licensed under the **MIT License**. 


## 📖 Further Reading

- **ModSecurity Documentation**: [https://modsecurity.org/](https://modsecurity.org/)
- **Django Framework**: [https://www.djangoproject.com/](https://www.djangoproject.com/)
- **NGINX Web Server**: [https://www.nginx.com/](https://www.nginx.com/)

---

## 🌟 Acknowledgments

- Kudos to us for our hard work!!!


Note: So far, we have not released the full documentation and code of this project. After we release it, you can contribute, or use it for your own web security research! 🔐

---
![ml](https://github.com/user-attachments/assets/636943d9-8229-4b3a-b379-9ed007d77b60)
ML model training for http traffic.

---
![admin_dashboard](https://github.com/user-attachments/assets/8b5efd53-dd81-4fdd-8076-e6e34d687bed)
Django web app development for ML trained model and modsecurity integration.

---
![Screenshot from 2024-10-26 23-54-20](https://github.com/user-attachments/assets/f88589b4-5cc9-4b71-b014-9cc2c775d547)
Nginx configurations on Ubuntu O.S.



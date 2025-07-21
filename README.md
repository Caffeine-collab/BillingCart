# BillingCart
A mini project developed by undergraduate students of Electronics and Communication Engineering at Rajagiri School of Engineering & Technology, aimed at modernizing the retail checkout experience using IoT, embedded systems, and Android development.

📌 Project Overview
The Smart Billing Cart combines RFID technology and load cell-based weight verification to automate billing in retail environments. It ensures that only verified products are added to the virtual cart and enables checkout only when there are no mismatches in product data, increasing accuracy and reducing theft or errors.

👥 Team Members
Maria Siju Joseph (U2201126)
Keziah Mariam Varughese (U2201117)
K Vijay Krishnan (U2201115)
Milan Thomas C (U2201133)
Guide: Ms. Soni Monica, Dept. of ECE

 Features
RFID-based product scanning using EM-18 Reader
Weight verification with HX711 Load Cell
Central control using ESP32
Real-time product validation with PHP & MySQL database
Checkout via Android app (built with Android Studio)
QR Code payment interface for secure checkout
LCD display for user feedback

🧠 Technologies Used
Hardware
ESP32 WROOM 32
EM-18 RFID Reader
HX711 Load Cell Amplifier
16x2 I2C LCD Display

Software
Arduino IDE (Microcontroller Programming)
XAMPP (Localhost PHP & MySQL Database)
Android Studio (Android App Development)

📐 System Architecture
User scans RFID tag
System prompts for weight check
ESP32 checks RFID + weight data with server
If valid → product added to bill
If mismatch → checkout blocked
Android app receives item data, generates total, and activates checkout only after validation

🔧 Setup Instructions
1. Arduino
Upload the provided .ino sketch to ESP32 using Arduino IDE
Ensure calibration factor for HX711 is accurate

3. Server (PHP + MySQL)
Run XAMPP
Place PHP files in htdocs/blue_shopping_cart/
Import product data with predefined RFID & weight

3. Android App
Install APK built via Android Studio
Connect to the same Wi-Fi as ESP32

App syncs with ESP32 and enables checkout upon successful validation

💡 Key Functionalities
Add/Remove Items: By re-scanning RFID tags
Real-Time Validation: Using server-based product database
Secure Checkout: Enabled only when all weights match expected values
Anti-Theft: Any mismatch disables checkout instantly


📊 Estimated Cost
Component	Cost (INR)
ESP32	₹700
Load Cell + HX711	₹325
RFID Module + Tags	₹495
LCD + I2C Module	₹270
Others	₹630
Total	₹2500

🔍 Challenges Faced
Sensor calibration and false mismatches
Wi-Fi and app synchronization delays
UI limitations on LCD

Power management for multiple peripherals

📈 Future Improvements
Visual object recognition using cameras
Cloud-based database for multi-store access
Voice-command checkout
Better mobile app UX (offers, loyalty points, multi-language)
Improved anti-theft mechanisms with smart vision

📚 References
Laxmi et al., “Smart Shopping Cart using RFID,” IJSREM, 2018
Dangat et al., “Smart Trolley with Automatic Billing System,” IJRASET, 2025
Yogalakshmi & Maik, “Automated Shopping Trolley with RFID and IoT,” Springer, 2020

🏫 Academic Info
Course: B.Tech in Electronics and Communication Engineering
Institute: Rajagiri School of Engineering & Technology (Autonomous)
University: APJ Abdul Kalam Technological University
Year: 2024–2025

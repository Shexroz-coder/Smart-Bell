# Smart-Bell
Smart School Bell v1.0 is a Wi-Fi enabled, ESP32-based automated school bell system. It uses a real-time clock (RTC) module to track the time and a relay module to ring a traditional school bell according to a customizable schedule stored in JSON format.
Teachers or administrators can connect to the ESP32's local web interface to:

📅 View, add, or delete scheduled bell times

🛠 Edit the schedule without reprogramming the board

🔒 Password-protect access (optional in future updates)

This version is fully standalone and does not require cloud services.

🧰 Features
Uses DS3231 RTC for precise timekeeping

Stores schedule in internal memory using SPIFFS

Simple and user-friendly web interface (via built-in ESP32 web server)

Relay triggers a real bell for 2 seconds at scheduled times

LCD display shows current time and upcoming bell

Compatible with Wemos D1 R32 (ESP32 UNO form)

🛠 Hardware Required
ESP32 board (Wemos D1 R32 recommended)

DS3231 RTC module

Relay module

LCD I2C (16x2) display

Optional: buzzer, power supply, casing

🌐 Web Interface
Accessible via ESP32's IP (e.g. 192.168.4.1 if in AP mode), with options to:

🔘 Add new bell times

🗑 Delete all times for a specific weekday

🕰 Set RTC time manually via browser

🗂 File Structure
pgsql
/data/schedule.json    → Bell schedule in JSON format  
main.ino               → Main Arduino sketch  
🧪 Demo

🇺🇿 Tavsif (O'zbekcha)
Smart School Bell v1.0 — bu ESP32 asosidagi, Wi-Fi orqali ishlaydigan avtomatik maktab qo‘ng‘iroq tizimi. Qurilma har bir darsga mos jadval asosida qo‘ng‘iroqni avtomatik ravishda chaladi.

Xususiyatlari:
⏰ RTC DS3231 yordamida aniq vaqt kuzatuv

📂 Qo‘ng‘iroq jadvali JSON faylida saqlanadi

🌐 Veb sahifa orqali qo‘shish/o‘chirish/ko‘rish

🖥 LCD ekran: vaqt va keyingi qo‘ng‘iroq ko‘rsatiladi

🔌 Rele orqali 2 soniyalik signal yuboriladi

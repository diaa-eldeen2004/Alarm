# Qt Alarm Clock ⏰
Description:Qt Alarm Clock is a user-friendly desktop application crafted with Qt Creator using the Qt framework (C++ and Qt Widgets). It empowers users to set, manage, and delete alarms with ease. Featuring a clean interface, users can input alarm times (in HH:MM format) and custom labels, view all active alarms, and get notified when an alarm matches the system time. The app checks the time every second to keep things ticking! 🕒
Features:  

Add Alarms ➕: Set alarms by entering a time (HH:MM) and a custom label.  
Delete Alarms 🗑️: Remove specific alarms by providing their time and label.  
View Alarms 📋: Display a list of all active alarms with their times and labels.  
Real-Time Checking 🔄: Automatically checks the system time every second to trigger alarms.  
Input Validation ✅: Ensures valid time formats and required fields with friendly error messages.  
Status Updates 💬: Shows feedback like "Alarm added!" or "Alarm ringing!"

Technologies Used:  

C++ 💻: Core language for logic and functionality.  
Qt Framework 🖼️: Powers the GUI with Qt Widgets and handles timers and signals/slots.  
Qt Creator 🛠️: Used as the IDE for building and designing the application.  
Qt Classes: Utilizes QTimer, QLineEdit, QPushButton, QLabel, QVBoxLayout, and QMessageBox.

How It Works:  

A QTimer checks the system time every second via updateAlarmStatus.  
Alarms are stored in two QList containers: one for times (QTime) and one for labels (QString).  
The GUI includes input fields for time and label, buttons for adding/deleting/showing alarms, and a status label for feedback.  
When the current time matches an alarm, the status updates to "Alarm ringing!" 🚨

Usage:  

Enter a time in HH:MM format and a label in the input fields.  
Click "Add Alarm" to set a new alarm.  
Use "Delete Alarm" to remove an alarm by specifying its time and label.  
Click "Show Alarms" to view all active alarms.  
When an alarm’s time is reached, the status label shows "Alarm ringing!"

Dependencies:  

Qt 5 or later (Qt Widgets module) 📦  
C++11 or later

File Structure:  

alarmclock.h: Declares the AlarmClock class with member variables and functions.  
alarmclock.cpp: Implements the UI setup, alarm management, and timer logic.  
main.cpp: Entry point to launch the AlarmClock widget.

Future Improvements:  

Add sound or visual effects for ringing alarms 🎵  
Support recurring alarms or a snooze feature 😴  
Save alarms to a file for persistence 💾  
Enhance the UI with modern styling or customization options 🎨

License:MIT License  
Contributing:Contributions are welcome! 🙌 Please submit a pull request or open an issue to discuss improvements or bugs.


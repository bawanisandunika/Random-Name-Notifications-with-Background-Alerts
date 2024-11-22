<<<<<<< HEAD
# Random Name Notifications with Background Alerts  

![Flutter](https://img.shields.io/badge/Flutter-Framework-blue)  
![Notifications](https://img.shields.io/badge/Notifications-Enabled-brightgreen)  
![Background Tasks](https://img.shields.io/badge/Background--Tasks-Supported-orange)

## 🚀 About the Project  
This project demonstrates a Flutter application that sends random name notifications periodically, even when the app is not running in the foreground or is completely closed. 

It leverages the following technologies:  
- **`flutter_local_notifications`**: For handling and displaying notifications.  
- **`android_alarm_manager_plus`**: For scheduling background tasks to ensure notifications are sent on time.  

---

## 🎯 Features  
- Sends a random name notification every 3 minutes.  
- Works in the background and when the app is closed.  
- Ensures device wake-up for notifications.  
- Simple UI with easy-to-extend functionality.

---

## 🛠️ How It Works  

1. **Notification Scheduling**  
   - A periodic alarm is set using `android_alarm_manager_plus` to trigger the notification logic every 3 minutes.  
   - Random names are selected from a predefined list.  

2. **Notifications**  
   - Notifications are displayed with `flutter_local_notifications`.  
   - The title and body of the notification update dynamically with the random name.  

3. **Background Task Execution**  
   - The alarm manager ensures notifications work even if the app is minimized or closed.  

---

## 📂 Project Structure  
lib/ ├── main.dart # Entry point of the application ├── screens/ │ └── notification_screen.dart # UI logic and notification scheduling └── services/ └── notification_service.dart # Notification logic and background task handling

yaml
Copy code

---

## 💻 Prerequisites  

1. **Flutter SDK**  
   Install Flutter: [Get Started](https://flutter.dev/docs/get-started)  

2. **Required Plugins**  
   Add the following dependencies to `pubspec.yaml`:  
   ```yaml
   dependencies:
     flutter_local_notifications: ^14.0.0
     android_alarm_manager_plus: ^2.0.0
Android Configuration
Update AndroidManifest.xml with alarm manager permissions:
xml
Copy code
<uses-permission android:name="android.permission.WAKE_LOCK" />
📦 Installation
Clone the Repository

bash

git clone https://github.com/bawanisandunika/random-name-notifications.git
cd random-name-notifications
Install Dependencies

bash

flutter pub get
Run the Application

bash

flutter run
🚀 Usage
Open the app and see the message:
"Notifications with random names will appear every 3 minutes."

Minimize or close the app.

Wait for the scheduled time (default: 3 minutes) and see the notifications appear.

🔧 Customization
Change Notification Interval
Update the Duration(minutes: 3) in notification_screen.dart to your preferred interval.

Add Custom Names
Update the list of random names in notification_service.dart:

dart

List<String> names = ["YourName1", "YourName2"];
🤝 Contributing
Contributions are welcome!
Feel free to fork the repository and submit a pull request with your improvements.

📄 License
This project is licensed under the MIT License.
See the LICENSE file for details.

💬 Let's Connect
If you have any questions, feel free to reach out!

GitHub: bawanisandunika
Email: bawanisandunika51@gmail.com

=======
# alearts

A new Flutter project.

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://docs.flutter.dev/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://docs.flutter.dev/cookbook)

For help getting started with Flutter development, view the
[online documentation](https://docs.flutter.dev/), which offers tutorials,
samples, guidance on mobile development, and a full API reference.
>>>>>>> 75f9dd8 (Initial commit: Add Random Name Notifications project)

# Physical Tracker App

Physical Tracker is a native Android application developed for the "Mobile Applications Laboratory" course (A.Y. 2023/2024) at the University of Bologna. The project focuses on monitoring the user's daily activities by utilizing the integrated sensors of the mobile device.

## Authors
- **Alessandro Ravveduto** (alessandro.ravveduto@studio.unibo.it).
- **Alessandro Tomaiuolo** (alessandro.tomaiuol2@studio.unibo.it).

## Core Features
- **Activity Monitoring**: The app records specific activities including Walking, Running, Resting, and Driving.
- **Real-Time Data**: Activity screens display relevant information such as steps, speed, and elapsed time.
- **Interactive Calendar**: Users can navigate through months to view past activities. Users can also import calendars to view activities performed by others.
- **Geofencing**: This feature allows users to set up virtual geographic barriers by long-pressing on a map to add a marker. The app operates in the background to notify users when they enter, exit, or remain in these areas.
- **Profile and Statistics**: The profile section tracks user height and weight, which is essential for calculating calories. It also features pie charts for activity types and bar charts for daily step counts.
- **Language Support**: The application automatically adapts to the system language, fully supporting both Italian and English.

## Technical Architecture
- **Design Pattern**: The application is built using the Model-View-ViewModel (MVVM) architecture to separate responsibilities and improve modularity.
- **Data Persistence**: Local database management is handled using the Room library.
- **Map Integration**: The Google Maps SDK is integrated to manage map functionalities, real-time location updates, and automatic geofencing events.
- **Background Services**: A WorkManager is implemented to check for user inactivity every 15 minutes. It triggers notifications to encourage the user to log new activities if the inactivity threshold is exceeded.
- **Libraries Used**: The app utilizes `kizitonwose.calendar` for the customizable calendar interface, `MPAndroidChart` for statistical charts, and `AmbilWarna` for color customization.

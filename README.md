# IOMT🌐 Overview

The IoMT-Based Stress Monitoring System is a real-time health informatics application that integrates Fitbit wearable data, AWS Cloud Services, and a Flutter mobile app to monitor and visualize stress through physiological signals.

By leveraging AWS Lambda, DynamoDB, API Gateway, and EventBridge, the system automates Fitbit data retrieval, storage, and synchronization — forming a secure, fully serverless IoMT ecosystem.

“This project connects the heartbeat of humans with the heartbeat of technology.”

⚙️ Features

✅ Real-time Fitbit data access (heart rate, activity).
✅ Secure OAuth 2.0 authentication and token management.
✅ AWS-based serverless backend (Lambda + DynamoDB + API Gateway).
✅ Automated data refresh via AWS EventBridge.
✅ Cross-platform Flutter UI for Android & Web.
✅ Scalable architecture for future wearables and analytics.

🏗️ System Architecture
Fitbit → Fitbit API → AWS Lambda → DynamoDB ↔ Flutter App
                        ↑
                    EventBridge

Layer	Technology	Purpose
Frontend	Flutter (Dart)	User interface and visualization
Backend	AWS Lambda (Python 3.12)	Data processing & API handling
Database	DynamoDB	Token & health data storage
Integration	Fitbit API	Real-time heart rate and activity data
Automation	EventBridge	Scheduled token refresh and data sync
🧠 Technology Stack

Frontend: Flutter, Dart
Backend: AWS Lambda (Python 3.12)
Database: AWS DynamoDB
Cloud Services: API Gateway, EventBridge, IAM
Integration: Fitbit Web API (OAuth 2.0)
Design: Figma

🚀 Implementation Summary

Lab 1: IDE Setup – Configured Flutter SDK & Emulator.

Lab 2: UI Design – Prototyped in Figma.

Lab 3: Frontend Development – Built Flutter UI & Navigation.

Lab 4: AWS Setup – Created Lambda, DynamoDB, API Gateway.

Lab 5: Fitbit Integration – Connected API & Stored Data.

Lab 6.1: Authentication – Automated OAuth Token Refresh.

Lab 6.2: Data Access – Automated Fitbit Sync and Storage.

🧪 Testing & Results

Verified Fitbit API calls via Postman and AWS Console.

DynamoDB stored accurate time-stamped records.

EventBridge triggered data sync every 6 hours.

Flutter dashboard displayed real-time heart rate visualization.

🛠️ Challenges & Solutions
Challenge	Resolution
Token Expiration	Automated refresh using EventBridge
Data Duplication	DynamoDB conditional writes
Lambda Timeout	Increased timeout and optimized JSON parsing
OAuth Complexity	Simplified authorization flow with reusable functions
🔮 Future Enhancements

Integrate AWS SageMaker for predictive stress modeling.

Support additional wearables (Apple Watch, Garmin).

Add real-time notifications and data analytics dashboards.

Deploy mobile app via AWS Amplify for live use.

💡 Key Learnings

This project strengthened skills in serverless architecture, OAuth security, and IoMT data engineering, demonstrating how cloud-native design can deliver secure, real-time health insight.

“The system became more than code — it became a living rhythm of data.”

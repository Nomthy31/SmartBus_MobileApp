# SmartBus_MobileApp
This is the **React Native mobile frontend** for the SmartBus application — a modern digital platform that helps commuters track buses, refill coupons, and plan routes in real time across Johannesburg with Rea Vaya and MetroBus.

## 📱 Features
- 🔍 Search and view bus routes & schedules
- 📍 Real-time GPS tracking of buses
- 💳 Mobile coupon refill with online payment
- 🔔 Push notifications for delays or route changes
- 🧾 View payment history

## 🛠️ Prerequisites
Install these before you begin:

| Tool | Version |
|------|---------|
| Node.js | >= 16.x |
| npm or yarn | Latest |
| Expo CLI | ^5.0.0 |
| Git | Any |
| Android Studio or Xcode | Latest (for emulator) |
| VS Code | Recommended |

## 🚀 Getting Started

### 1. Clone the Repository
git clone https://github.com/your-username/smartbus-app.git
cd smartbus-app
### 2. Install Dependencies
npm install
### 3. Create a `.env` File
cp .env.example .env

## ▶️ Running the App
npx expo start
Scan the QR code with your Expo Go app or run it on an emulator using `a` (Android) or `i` (iOS).

## 🌐 Backend API Endpoints (from Django)

The frontend consumes APIs like:

| Endpoint               | Function                     |
| ---------------------- | ---------------------------- |
| `/api/login/`          | Authenticate user            |
| `/api/routes/`         | List available routes        |
| `/api/track/<bus_id>/` | Fetch real-time bus location |
| `/api/coupons/refill/` | Refill using payment gateway |
| `/api/notifications/`  | Fetch alerts and delays      |
| `/api/trips/`          | Get trip history             |

Make sure your Django server is running on `localhost:8000` or update your `.env`.

## 🧪 Testing
To run unit tests (if configured):
npm run test

## 🧱 Folder Structure

smartbus-frontend/
├── components/         # Reusable UI components
├── screens/            # All page screens (Home, Routes, Profile, etc.)
├── services/           # API service layer (Axios)
├── assets/             # Images, icons, styles
├── App.js              # Root app entry point
└── .env                # Environment config

## 🔐 Auth & Security

* Auth via Django REST with JWT tokens
* Tokens stored securely in AsyncStorage
* Protected screens based on user roles (passenger, driver, admin)

## 💬 Notifications

* Push via Firebase Cloud Messaging (FCM)
* Configured with your Firebase project
* Handles alerts from backend like delays or strikes

## 📊 Planned Integrations

* Google Maps API or Mapbox for live location
* PayFast, SnapScan, or Ozow for secure payments
* Firebase for notification delivery
* Django REST Framework backend

## 🤝 Contributing

1. Fork this repository
2. Create a branch: `git checkout -b feature/my-feature`
3. Commit your changes: `git commit -m "Add feature"`
4. Push to your fork: `git push origin feature/my-feature`
5. Submit a pull request 🚀

## 📄 License

This project is licensed under the [MIT License](LICENSE).

## 📬 Contact

📧 You can contact the creators of the App:
* thatomphahlele57@gmail.com
* nomcebonkomo203@gmail.com
* nlmabena2015@gmail.com

🌍 (https://smartbus.co.za) *(coming soon)*






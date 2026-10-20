# Afubia Farms Sales Mobile App 🌴

A sales and inventory management application for **Afubia Farms**, designed to simplify palm oil sales, production conversions, stock tracking, and business reporting across the **Ogidan Shop** and **Kara Shop**.

The application helps staff record daily business activities while giving administrators tools to monitor sales, inventory, and business performance.

## 📌 Project Overview

Afubia Farms Sales Mobile App is built to support the day-to-day operations of a palm oil business. It brings sales records, oil production conversions, material purchases, stock tracking, and reporting into one system.

The project uses a React-based frontend and Firebase services for authentication and cloud data storage.

## ✨ Key Features

- **Sales Management** — Record and manage palm oil sales.
- **Production & Oil Conversion** — Record oil-turning and production conversion activities.
- **Inventory Management** — Track materials, stock movements, and available oil.
- **Stock Tracking** — Calculate stock levels using opening stock, purchases, sales, and production usage.
- **Business Reports** — Review sales records and business activity over selected dates.
- **Profit Analysis** — Provide administrators with tools for analysing business performance.
- **Firebase Integration** — Store and retrieve business records using Cloud Firestore.
- **Authentication & Roles** — Support authenticated access and administrator or sales staff experiences.
- **Voice Assistance** — Provide audio prompts, including Nigerian Pidgin-style guidance, for supported actions.
- **Responsive Interface** — Designed for practical use across supported mobile and desktop screen sizes.
- **Multi-Branch Business Context** — Intended to support operations at Ogidan Shop and Kara Shop.

*Note: Features that require additional branch-specific configuration, permissions, or native mobile packaging depend on the current implementation.*

## 🛠️ Technology Stack

| Technology | Purpose |
|---|---|
| React | User interface |
| Vite | Development server and build tooling |
| JavaScript | Application logic |
| Firebase Authentication | User authentication |
| Cloud Firestore | Cloud database |
| CSS | Styling and responsive layouts |
| Git & GitHub | Version control and collaboration |

## 📂 Main Business Modules

### 1. Sales

Records sales transactions, including product quantities and relevant transaction details.

### 2. Production and Conversion

Records palm oil conversion activities and production outputs so they can be reflected in the relevant business records.

### 3. Materials and Inventory

Maintains material purchase records and supports stock calculations.

### 4. Reports

Provides access to business records and reporting tools for reviewing activities over time.

### 5. Administration

Provides authorised administrators with access to management features, including profit analysis and business oversight.

## 🏪 Shop Branches

The business operates across two shop locations:

- **Ogidan Shop**
- **Kara Shop**

The application is intended to support accurate business recordkeeping across both locations. Branch-specific staff access, reporting, and stock separation should be configured and verified against the implemented Firebase data model and security rules.

## ⚙️ Getting Started

### Prerequisites

Install the following before running the project:

- [Node.js](https://nodejs.org/)
- npm, included with Node.js
- [Git](https://git-scm.com/)
- A Firebase project with the required services configured

### 1. Clone the Repository

```bash
git clone https://github.com/Afubia-Group/Afubia-Farms-Sales-Mobile-App.git
```

### 2. Open the Project Folder

```bash
cd Afubia-Farms-Sales-Mobile-App
```

### 3. Install Dependencies

```bash
npm install
```

### 4. Configure Firebase

Create a `.env` file in the project root and add your Firebase web application configuration:

```env
VITE_FIREBASE_API_KEY=your_firebase_api_key
VITE_FIREBASE_AUTH_DOMAIN=your_project.firebaseapp.com
VITE_FIREBASE_PROJECT_ID=your_firebase_project_id
VITE_FIREBASE_STORAGE_BUCKET=your_storage_bucket
VITE_FIREBASE_MESSAGING_SENDER_ID=your_messaging_sender_id
VITE_FIREBASE_APP_ID=your_firebase_app_id
```

Replace the example values with the configuration for your Firebase project.

Ensure that the variable names match those used by the application. Configure Firebase Authentication, Firestore, authorised domains, and the necessary database security rules.

**Security:** Never commit your `.env` file, Firebase service-account credentials, private keys, or staff passwords to GitHub. Keep secrets out of source control and use an appropriate `.gitignore`.

### 5. Start the Development Server

```bash
npm run dev
```

Open the local URL printed in your terminal to view the application.

### 6. Build for Production

```bash
npm run build
```

To preview the production build locally:

```bash
npm run preview
```

## 🔐 Security and Access Control

The application uses Firebase services to support authentication and data storage.

For production deployment:

- Restrict administrator functions to authorised users.
- Enforce permissions using Firebase Security Rules, not only frontend route checks.
- Protect sales and inventory records against unauthorised changes.
- Keep configuration files containing sensitive information out of the repository.
- Validate any branch-specific access rules before deploying the system to both shops.

## 📱 Mobile Usage

The project is intended to support convenient business operations on mobile devices. Its exact installation and distribution method depends on the current build configuration.

If the repository is configured as a web application, it can be deployed to a compatible web hosting platform. An installable Android APK or Google Play release requires the appropriate mobile packaging and build configuration; a standard Vite production build does not itself produce an APK.

## 🚀 Future Improvements

Potential enhancements include:

- Branch-specific staff accounts and permissions.
- Separate stock and sales views for Ogidan and Kara shops.
- Staff login timestamps and authorised location records.
- Automated end-of-day reporting.
- Excel report exports.
- Improved offline handling and data synchronisation.
- A packaged Android application, where supported by the final project architecture.

## 🤝 Contributing

Contributions and improvements should follow the project's coding conventions and preserve the accuracy of sales, production, and stock records.

1. Fork the repository or create a development branch.
2. Make your changes.
3. Test the affected features.
4. Submit a pull request describing the changes.

## 🏢 Organisation

**Afubia Farms**

Repository: [Afubia Farms Sales Mobile App](https://github.com/Afubia-Group/Afubia-Farms-Sales-Mobile-App)

## 📄 License

A licence has not yet been specified. Add a `LICENSE` file to the repository if the project is to be distributed under a particular open-source or proprietary licence.

---

*Built to support better sales records, inventory management, and daily operations at Afubia Farms.*

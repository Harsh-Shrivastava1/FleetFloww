# 🚛 FleetFlow

[![Vite](https://img.shields.io/badge/vite-%23646CFF.svg?style=for-the-badge&logo=vite&logoColor=white)](https://vitejs.dev/)
[![React](https://img.shields.io/badge/react-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB)](https://reactjs.org/)
[![TypeScript](https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![TailwindCSS](https://img.shields.io/badge/tailwindcss-%2338B2AC.svg?style=for-the-badge&logo=tailwind-css&logoColor=white)](https://tailwindcss.com/)
[![Firebase](https://img.shields.io/badge/firebase-%23039BE5.svg?style=for-the-badge&logo=firebase)](https://firebase.google.com/)
[![Vercel](https://img.shields.io/badge/vercel-%23000000.svg?style=for-the-badge&logo=vercel&logoColor=white)](https://vercel.com/)

**FleetFlow** is a modern, enterprise-grade Fleet Management System designed to streamline operations, optimize logistics, and reduce environmental impact. Built with a focus on real-time data and actionable insights, FleetFlow empowers fleet managers to oversee their entire operation from a single, intuitive interface.

---

## ✨ Key Features

### 📊 Intelligence & Analytics
- **Executive Dashboard**: A high-level overview of active trips, fleet health, revenue, and sustainability metrics.
- **Advanced Analytics**: Interactive data visualization using **Recharts** to track fuel efficiency, financial trends, and operational performance.
- **Carbon Footprint Tracking**: Dedicated sustainability module to monitor CO2 emissions and track progress against eco-friendly targets.

### 📍 Real-Time Operations
- **Live Tracking**: Real-time vehicle positioning on interactive maps powered by **Leaflet**.
- **Trip Dispatcher**: Full lifecycle management of trips—from preparation and cargo assignment to real-time status updates.
- **Route Optimization**: Intelligent routing to minimize distance, reduce fuel consumption, and save time.

### 🚛 Asset & Human Resources
- **Vehicle Registry**: Detailed inventory management including technical specifications, acquisition costs, and maintenance history.
- **Driver Management**: Digital profiles for drivers featuring safety scores, completion rates, and performance history.
- **Maintenance Scheduling**: Proactive service logs to track repairs, oil changes, and part replacements, ensuring maximum uptime.

### 💰 Financial Management
- **Expense Tracking**: Digital logging of fuel, tolls, and maintenance costs with support for receipt uploads.
- **Profitability Analysis**: Automated calculation of Net Profit, Cost-per-Km, and Revenue-per-Trip.

---

## 🚀 Tech Stack

| Category | Technology |
| :--- | :--- |
| **Frontend** | React 19, TypeScript, Vite |
| **Styling** | Tailwind CSS 4, Framer Motion, Lucide Icons |
| **UI Components** | Shadcn UI, Radix UI |
| **State Management** | Zustand |
| **Database & Auth** | Firebase (Firestore, Realtime DB, Auth) |
| **Maps & Charts** | Leaflet, React Leaflet, Recharts |
| **Deployment** | Vercel |

---

## 🛠️ Getting Started

### Prerequisites
- Node.js (Latest LTS version recommended)
- npm or bun

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/fleetflow.git
   cd fleetflow/frontend
   ```

2. **Install dependencies**
   ```bash
   npm install
   # or
   bun install
   ```

3. **Set up Environment Variables**
   Create a `.env` file in the `frontend` directory and add your Firebase credentials:
   ```env
   VITE_FIREBASE_API_KEY=your_api_key
   VITE_FIREBASE_AUTH_DOMAIN=your_auth_domain
   VITE_FIREBASE_PROJECT_ID=your_project_id
   VITE_FIREBASE_STORAGE_BUCKET=your_storage_bucket
   VITE_FIREBASE_MESSAGING_SENDER_ID=your_sender_id
   VITE_FIREBASE_APP_ID=your_app_id
   ```

4. **Run the development server**
   ```bash
   npm run dev
   ```
   Open [http://localhost:5173](http://localhost:5173) in your browser.

---

## 📂 Project Structure

```text
fleetflow/
├── frontend/
│   ├── src/
│   │   ├── components/    # Reusable UI components (shadcn, shared, layout)
│   │   ├── pages/         # Page-level components (Dashboard, Tracking, etc.)
│   │   ├── store/         # Zustand state management
│   │   ├── contexts/      # React Contexts (Auth)
│   │   ├── hooks/         # Custom React hooks
│   │   ├── lib/           # Library configurations (Firebase, utils)
│   │   └── types/         # TypeScript interfaces and types
│   ├── public/            # Static assets
│   └── vite.config.ts     # Vite configuration
└── FIREBASE_SCHEMA.md     # Detailed database architecture
```

---

## 🛡️ Security & Roles

FleetFlow implements granular **Role-Based Access Control (RBAC)** via Firebase Security Rules:
- **Admin**: Full system access, financial oversight, and user management.
- **Manager**: Fleet operations, trip dispatching, and report viewing.
- **Driver**: Access to assigned trips and expense logging (planned).
- **Viewer**: Read-only access to specific dashboards.

---

## 📜 License

This project is licensed under the MIT License - see the LICENSE file for details.

---

*Built with ❤️ for better logistics.*

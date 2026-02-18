# Grocer Delivery Partner App �

The dedicated mobile application for **Delivery Partners** to manage orders, navigate to customers, and ensure timely deliveries.

This app is a critical component of the **Grocer Ecosystem**, working in tandem with the Customer App and Admin Dashboard to complete the order fulfillment lifecycle.

## � The Grocer Ecosystem

This repository is part of a 3-part system:

1.  **🛒 Customer App:** [GrocerApp](https://github.com/Kalebtes2031/GrocerApp)
    *   Where customers browse products, place orders, and schedule deliveries.
2.  **🚚 Delivery App (This Repo):** [GrocerDeliveryApp](https://github.com/Kalebtes2031/GrocerAdminDashboard)
    *   Where drivers accept assignments, track routes, and confirm deliveries.
3.  **🖥️ Admin Dashboard:** [GrocerAdminDashboard](https://github.com/Kalebtes2031/GrocerAdminDashboard.git)
    *   Central control panel for managing users, products, orders, and the entire system.

---

## 🚀 Key Features

### � Order Management
-   **Assigned Orders:** View incoming delivery requests assigned by the system or admin.
-   **Accepted Orders:** Manage your active delivery queue.
-   **Order Details:** View comprehensive order information, including customer address, items, and payment status.

### 📍 Navigation & Tracking
-   **Real-Time Tracking:** Integrated **MapLibre** support to track your location relative to the customer.
-   **Route Optimization:** Efficiently navigate to customer locations for drop-offs.
-   **Map Interface:** Visual representation of pickup and delivery points.

### 💼 Driver Workflow
-   **Availability Status:** Toggle online/offline to control when you receive new orders.
-   **Order Lifecycle:**
    1.  **Accept:** Confirm assignment of an order.
    2.  **Pick Up:** Mark order as collected from the store.
    3.  **Deliver:** Confirm successful handover to the customer.
-   **History:** View a log of all completed deliveries ("My Orders").

### � Profile & Settings
-   **Profile Management:** Update driver details and profile photo.
-   **Secure Authentication:** Login securely to access your dashboard.

---

## 🛠️ Tech Stack

-   **Framework:** [React Native](https://reactnative.dev/) with [Expo](https://expo.dev/) (SDK 53)
-   **Routing:** [Expo Router](https://docs.expo.dev/router/introduction/) (v5)
-   **Styling:** [NativeWind](https://www.nativewind.dev/) (Tailwind CSS)
-   **Maps:** MapLibre permissions and rendering.
-   **State Management:** React Context API (Global, Cart, Auth).
-   **API Client:** Axios for communication with the Django backend.

---

## ⚙️ Prerequisites

-   **Node.js** (LTS version recommended)
-   **npm** or **yarn**
-   **Expo Go** app on your physical device or an Emulator.

## 📦 Installation

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/Kalebtes2031/GrocerDeliveryApp.git
    cd GrocerDeliveryApp
    ```

2.  **Install dependencies:**
    ```bash
    npm install
    ```

3.  **Environment Configuration:**
    Create a `.env` file in the root directory by copying the example:
    ```bash
    cp .env.example .env
    ```
    Populate it with your credentials (API keys, Mapbox Token, etc.):
    ```env
    EXPO_PUBLIC_API_URL=https://your-backend-api.com
    EXPO_PUBLIC_MAPBOX_TOKEN=pk.eyJ1...
    # See .env.example for full list
    ```

## 🚀 Running the App

Start the Expo development server:

```bash
npx expo start
```

-   **Press `a`** to open in Android Emulator.
-   **Press `i`** to open in iOS Simulator.
-   **Scan the QR code** with Expo Go to run on a physical device.

---

## 🤝 Contributing

1.  Fork the repository.
2.  Create a feature branch (`git checkout -b feature/improved-tracking`).
3.  Commit your changes.
4.  Push to the branch.
5.  Open a Pull Request.

## 📄 License

This project is licensed under the MIT License.

## **Refillable** – A Simple Reusable Cup Tracking System

Refillable is a web application that helps users track and manage reusable coffee cups. Users can sign up, check their subscription status, track cups using RFID, and manage their loyalty points. The app promotes sustainability by encouraging the use of reusable cups over disposable ones.

---

### **Features**

- **User Authentication**: Users can sign up, log in, and manage their account information.
- **Subscription Management**: View and update subscription details and track loyalty points.
- **Cup Tracking**: Track reusable coffee cups using RFID technology. Update cup status (in use, available, etc.).
- **Payment Syncing**: Manage balances and payments. Sync payment data with external systems.

---

### **Tech Stack**

- **Frontend**: [Next.js](https://nextjs.org/) (React framework)
- **Backend**: [Supabase](https://supabase.io/) (PostgreSQL, Authentication, and API)
- **Database**: Supabase PostgreSQL
- **Deployment**: [Vercel](https://vercel.com/) (for hosting)

---

### **File Structure**

```bash
.
├── public/                # Static assets (images, etc.)
├── src/
│   ├── components/        # Reusable React components (optional)
│   ├── context/           # Global state (authentication)
│   ├── pages/             # Next.js pages for routing
│   │   ├── auth.js        # User login and registration
│   │   ├── subscription.js# Manage subscription data
│   │   ├── cup-status.js  # Track and update cup statuses
│   │   ├── scan-cup.js    # RFID scanning of cups
│   │   └── app-sync.js    # Sync server-side data (balance, payments)
│   ├── styles/            # Global CSS styles
│   └── utils/             # Supabase client setup
│       └── supabaseClient.js
├── package.json           # Dependencies
└── .env.local             # Environment variables
```

---

### **Installation**

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/refillable.git
   ```
2. Navigate to the project directory:
   ```bash
   cd refillable
   ```
3. Install the necessary dependencies:
   ```bash
   npm install
   ```
4. Set up environment variables in `.env.local` with your Supabase URL and API key:
   ```
   NEXT_PUBLIC_SUPABASE_URL=your-supabase-url
   NEXT_PUBLIC_SUPABASE_ANON_KEY=your-anon-key
   ```
5. Run the development server:
   ```bash
   npm run dev
   ```
6. Visit `http://localhost:3000` to view the app.

---

### **Usage**

- **Sign Up or Log In**: Navigate to `/auth` to sign up or log in.
- **Manage Subscriptions**: Visit `/subscription` to update your subscription type and check loyalty points.
- **Track Cup Status**: Go to `/cup-status` to see cup availability and update statuses.
- **Scan Cups**: Head to `/scan-cup` to track cups via RFID.
- **Sync Payment Data**: Use `/app-sync` to manage balances and sync payment information.

---

### **Contributing**

Contributions are welcome. To get started:
1. Fork this repository.
2. Create a new feature branch (`git checkout -b feature/new-feature`).
3. Commit your changes (`git commit -am 'Add new feature'`).
4. Push the branch (`git push origin feature/new-feature`).
5. Open a pull request.

---

### **License**

This project is licensed under the MIT License.

---

### **Contact**

For questions or support, please reach out to the repository owner at [wasif.zaman1@gmail.com].

---

**Refillable** aims to support sustainability by offering an easy-to-use reusable cup tracking system for coffee enthusiasts.

---

Feel free to customize it further! Let me know if you need any more modifications!

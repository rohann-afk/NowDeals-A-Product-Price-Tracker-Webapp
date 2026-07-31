# 🛒 NowDeals – Smart Product Price Tracker

![Next.js](https://img.shields.io/badge/Next.js-16-black?logo=next.js)
![Supabase](https://img.shields.io/badge/Supabase-Backend-3ECF8E?logo=supabase)
![Firecrawl](https://img.shields.io/badge/Firecrawl-AI-orange)
![License](https://img.shields.io/badge/License-MIT-blue)

NowDeals is a full-stack AI-powered product price tracker that allows users to monitor prices across e-commerce websites. Simply paste a product URL, and the application automatically extracts product details, stores historical prices, detects price drops, and sends email notifications when prices decrease.

---

## 🌐 Live Demo

**🔗 Live Website:** https://nowdealstracker.vercel.app

**📂 GitHub Repository:** https://github.com/rohann-afk/NowDeals-A-Product-Price-Tracker-Webapp

---

# ✨ Features

- 🔐 Google Authentication using Supabase Auth
- 📦 Track products using product URLs
- 🤖 AI-powered product scraping with Firecrawl
- 💰 Real-time price tracking
- 📈 Historical price analytics
- 📊 Interactive charts using Recharts
- 📧 Email alerts on price drops
- ⏰ Automated price checking with Vercel Cron Jobs
- 🖼️ Product image extraction
- 🔄 Automatic product updates
- 📱 Fully responsive UI
- ⚡ Built with Next.js App Router

---

# 🛠 Tech Stack

## Frontend

- Next.js 16
- React
- Tailwind CSS
- Shadcn UI
- Recharts
- Lucide React

## Backend

- Next.js Route Handlers
- Server Actions
- Supabase

## Database

- PostgreSQL (Supabase)

## Authentication

- Google OAuth (Supabase Auth)

## AI & Automation

- Firecrawl API
- Vercel Cron Jobs

## Email Service

- Resend API

---



# 📂 Project Structure

```text
app/
├── api/
│   └── cron/
│       └── check-prices/
├── auth/
├── dashboard/
├── actions.js
├── layout.js
└── page.js

components/
lib/
utils/
public/
```

---

# ⚙️ Installation

### Clone the repository

```bash
git clone https://github.com/rohann-afk/NowDeals-A-Product-Price-Tracker-Webapp.git

cd NowDeals-A-Product-Price-Tracker-Webapp
```

### Install dependencies

```bash
npm install
```

### Create Environment Variables

Create a `.env.local` file.

```env
NEXT_PUBLIC_SUPABASE_URL=

NEXT_PUBLIC_SUPABASE_ANON_KEY=

SUPABASE_SERVICE_ROLE_KEY=

FIRECRAWL_API_KEY=

CRON_SECRET=

RESEND_API_KEY=
```

### Start Development Server

```bash
npm run dev
```

Visit

```
http://localhost:3000
```

---

# 🚀 How It Works

1. Login using Google.
2. Paste any supported product URL.
3. Firecrawl extracts:

   - Product Name
   - Current Price
   - Currency
   - Product Image

4. Product data is stored in Supabase.
5. Historical prices are saved automatically.
6. Scheduled Cron Jobs periodically check prices.
7. If a price drops:
   - Database updates
   - Price history is stored
   - Email notification is sent to the user.

---

# 🗄 Database Schema

## Products

| Column | Description |
|---------|-------------|
| id | Product ID |
| user_id | Owner ID |
| url | Product URL |
| name | Product Name |
| current_price | Latest Price |
| currency | Currency |
| image_url | Product Image |
| created_at | Created Time |
| updated_at | Last Updated |

---

## Price History

| Column | Description |
|---------|-------------|
| id | History ID |
| product_id | Product |
| price | Price |
| currency | Currency |
| checked_at | Timestamp |

---

# 🔑 Environment Variables

| Variable | Purpose |
|-----------|----------|
| NEXT_PUBLIC_SUPABASE_URL | Supabase URL |
| NEXT_PUBLIC_SUPABASE_ANON_KEY | Supabase Anonymous Key |
| SUPABASE_SERVICE_ROLE_KEY | Service Role Key |
| FIRECRAWL_API_KEY | Firecrawl API |
| RESEND_API_KEY | Email Service |
| CRON_SECRET | Secure Cron Endpoint |

---

# 📦 Main Dependencies

- Next.js
- React
- Tailwind CSS
- Supabase
- Firecrawl
- Recharts
- Resend
- Lucide React

---

# 📈 Future Improvements

- 🤖 AI Price Prediction
- 📱 Mobile Application
- 🛒 Multi-store Price Comparison
- ❤️ Wishlist
- 📊 Advanced Analytics
- 🌍 Multi-Currency Support
- 🔔 Browser Push Notifications

---

# 🤝 Contributing

Contributions are welcome!

1. Fork the repository
2. Create a feature branch

```bash
git checkout -b feature-name
```

3. Commit your changes

```bash
git commit -m "Add new feature"
```

4. Push

```bash
git push origin feature-name
```

5. Open a Pull Request

---

# 👨‍💻 Author

**Rohan Majhi**

B.Tech – Computer Science & Engineering

🌐 GitHub: https://github.com/rohann-afk

💼 LinkedIn: https://www.linkedin.com/in/rohan-majhi-552252351/

---

# ⭐ Support

If you found this project helpful, consider giving it a ⭐ on GitHub!

---

# 📄 License

This project is licensed under the MIT License.
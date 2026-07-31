# 🛒NowDeals : Smart Product Price Tracker

A full-stack web application that allows users to track product prices from online shopping websites. The application automatically scrapes product information, stores historical price data, and helps users monitor price changes over time.

## 🚀 Features

- 🔐 Secure user authentication with Supabase
- 📦 Add products by simply pasting a product URL
- 🤖 Automatic product data extraction using Firecrawl AI
- 💰 Track current product prices
- 📈 Store and visualize price history
- 🖼️ Display product images
- 🔄 Update existing products automatically
- 📱 Responsive and modern user interface
- ⚡ Built with Next.js App Router

---

## 🛠️ Tech Stack

### Frontend
- Next.js 16
- React
- Tailwind CSS
- Shadcn UI
- Recharts

### Backend
- Next.js Server Actions
- Supabase

### Database
- PostgreSQL (Supabase)

### Authentication
- Supabase Auth (Google OAuth)

### AI & Web Scraping
- Firecrawl API

---

## 📂 Project Structure

```
app/
│── actions.js
│── auth/
│── components/
│── dashboard/
│── layout.js
│── page.js

components/
lib/
utils/
public/
```

---

## ⚙️ Installation

### Clone the repository

```bash
git clone https://github.com/rohann-afk/NowDeals-A-Product-Price-Tracker-Webapp.git
cd smart-product-price-tracker
```

### Install dependencies

```bash
npm install
```

### Create environment variables

Create a `.env.local` file in the project root.

```env
NEXT_PUBLIC_SUPABASE_URL=your_supabase_url
NEXT_PUBLIC_SUPABASE_ANON_KEY=your_supabase_anon_key

FIRECRAWL_API_KEY=your_firecrawl_api_key
```

### Run the development server

```bash
npm run dev
```

Open

```
http://localhost:3000
```

---

## 📸 How It Works

1. Sign in using Google.
2. Paste a product URL.
3. Firecrawl extracts:
   - Product Name
   - Current Price
   - Currency
   - Product Image
4. Product information is stored in Supabase.
5. Price history is recorded whenever the price changes.
6. Users can monitor products from their dashboard.

---

## 🗄️ Database

The project uses two main tables.

### Products

- id
- user_id
- url
- name
- current_price
- currency
- image_url
- created_at
- updated_at

### Price History

- id
- product_id
- price
- currency
- checked_at

---

## 🔑 Environment Variables

| Variable | Description |
|----------|-------------|
| `NEXT_PUBLIC_SUPABASE_URL` | Supabase Project URL |
| `NEXT_PUBLIC_SUPABASE_ANON_KEY` | Supabase Anonymous Key |
| `FIRECRAWL_API_KEY` | Firecrawl API Key |

---

## 📦 Main Dependencies

- Next.js
- React
- Tailwind CSS
- Supabase
- Firecrawl
- Recharts
- Lucide React

---

## 🎯 Future Improvements

- 📉 Price drop notifications
- 📧 Email alerts
- 📱 Mobile app
- ❤️ Wishlist support
- 🛍️ Multi-store comparison
- 📊 Advanced analytics dashboard

---

## 👨‍💻 Author

**Rohannn**

B.Tech Computer Science & Engineering

GitHub: https://github.com/rohann-afk

LinkedIn: https://www.linkedin.com/in/rohan-majhi-552252351/

---

## 📄 License

This project is licensed under the MIT License.

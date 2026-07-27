# 👕 AI-Powered Virtual Try-On Studio

An AI-powered virtual try-on web application that transforms the online shopping experience by allowing users to virtually try clothing before purchasing. Instead of relying on imagination, users simply upload their photo, select an outfit, and instantly visualize themselves wearing the chosen clothing from multiple viewing angles using Generative AI.

The project aims to bridge the gap between online shopping and physical trial rooms by making fashion shopping more interactive, personalized, and reducing purchase uncertainty.

---

# 🚀 Problem Statement

Online shoppers often struggle to determine how clothes will actually look on them before making a purchase. This uncertainty frequently leads to poor buying decisions, increased return rates, and lower customer confidence.

Traditional e-commerce platforms display clothing on models that rarely represent individual customers, making it difficult to visualize the final appearance.

This project addresses that challenge by providing an AI-powered virtual fitting room where customers can preview outfits on themselves before placing an order.

---

# 💡 Solution

The platform allows users to:

- Upload their own photo
- Browse clothing products
- Select desired outfits
- Generate AI-powered try-on images
- View generated outfits from multiple angles
- Save favorite looks
- Add products to cart and continue shopping

The application combines modern frontend technologies with AI image generation to create a seamless virtual shopping experience.

---

# ✨ Features

- 📸 Upload personal photos
- 👕 Virtual AI clothing try-on
- 🔄 Multi-angle outfit generation
- ❤️ Save favorite looks
- 🛒 Shopping cart integration
- 🎨 Light & Dark mode
- 📱 Fully responsive UI
- ⚡ Fast image generation with intelligent caching

---

# 🏗️ System Architecture

```
                   User
                     │
                     ▼
          React + TypeScript Frontend
                     │
      ┌──────────────┴──────────────┐
      ▼                             ▼
 Zustand Store             React Components
      │                             │
      └──────────────┬──────────────┘
                     ▼
             Supabase Backend
      (Authentication + Database)
                     │
                     ▼
         Supabase Edge Functions
                     │
                     ▼
        Generative AI Image Model
                     │
                     ▼
      Generated Virtual Try-On Images
```

---

# ⚙️ Tech Stack

## Frontend

- React 18
- TypeScript
- Vite
- React Router

## UI

- Tailwind CSS
- Shadcn/UI
- Radix UI

## State Management

- Zustand

## Backend

- Supabase
- Supabase Authentication
- PostgreSQL Database
- Edge Functions

## Form Handling

- React Hook Form
- Zod Validation

---

# 🧠 How It Works

### Step 1

The user uploads a photo.

### Step 2

The user selects clothing from the product catalog.

### Step 3

The selected image and outfit information are sent to Supabase Edge Functions.

### Step 4

The AI model generates realistic try-on images.

### Step 5

Generated images are returned to the frontend.

### Step 6

Users can:

- Compare outfits
- Switch viewing angles
- Save favorite looks
- Continue shopping

To improve performance, previously generated outfit combinations are cached so identical requests don't require regeneration.

---

# 📂 Project Structure

```
E-C_website_VR-tryon-main/

├── public/
├── src/
│   ├── components/
│   ├── pages/
│   ├── hooks/
│   ├── store/
│   ├── data/
│   ├── integrations/
│   └── lib/
├── supabase/
├── package.json
└── README.md
```

---

# ▶️ Getting Started

## Clone Repository

```bash
git clone https://github.com/sinchana-sooda/clothing-try-on.git
```

## Navigate into project

```bash
cd E-C_website_VR-tryon-main
```

## Install dependencies

Using Bun

```bash
bun install
```

or using npm

```bash
npm install
```

---

## Run Development Server

Using Bun

```bash
bun run dev
```

Using npm

```bash
npm run dev
```

Open

```
http://localhost:5173
```

---

# 🔐 Environment Variables

Create a `.env` file and configure:

```env
VITE_SUPABASE_URL=your_supabase_url
VITE_SUPABASE_PROJECT_ID=your_project_id
VITE_SUPABASE_PUBLISHABLE_KEY=your_publishable_key
```

---

# 🛍️ Core Functionalities

- AI Virtual Try-On
- Product Catalog
- Shopping Cart
- Multi-Angle Preview
- Outfit History
- Saved Looks
- Responsive Design
- Theme Support
- AI Image Caching

---

# 🚀 Future Enhancements

- Real-time body measurements
- Personalized outfit recommendations
- AI size prediction
- Social sharing
- Video-based virtual try-on
- AR-based live fitting experience

---

# 👥 Team

Developed collaboratively as a team project.
1. Sinchana S Sooda
2. Siddharth R
3. Bindhushree.G
4. Bhawesh Mishra

This repository is maintained on my GitHub profile to showcase my contribution to the project.

---

# 📜 License

This project was developed for educational and learning purposes.

# 📉 PriceMonitor – E-Commerce Price Drop Notifier

PriceWatcher is a mobile application and backend service that monitors product prices from e-commerce websites (like Amazon) and notifies users when their selected product drops below a desired price.

---

## 📱 Features

- Track product prices in real-time
- Set a target price per product
- Receive instant notifications when the price drops
- Support for major e-commerce platforms (starting with Amazon)
- Background scraping and automated updates

---

## 🏗️ Architecture Overview

This project consists of two main components:

1. **Backend (Node.js + Puppeteer)**  
   - Scrapes product details periodically  
   - Compares current prices to user-defined targets  
   - Sends notifications via push service (Firebase Cloud Messaging or similar)  
   - Stores user and product data in a cloud database (e.g., MongoDB or Firebase)

2. **Mobile App (React Native)**  
   - Allows users to add products by URL and set price thresholds  
   - Displays tracked products and price history  
   - Handles push notifications and alerts  

---

## 🧰 Tech Stack

- **Frontend:** React Native  
- **Backend:** Node.js, Puppeteer  
- **Database:** MongoDB Atlas / Firebase Firestore  
- **Notifications:** Firebase Cloud Messaging (FCM)  
- **Deployment:** Vercel / Render / Heroku (customizable)  

---

## 🚀 Getting Started

### Backend Setup

```bash
git clone https://github.com/yourusername/pricewatcher-backend.git
cd pricewatcher-backend
npm install

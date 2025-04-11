# 📊 Hotel Management Dashboard

This project is a **comprehensive Hotel Management Dashboard** designed to monitor and analyze various hotel operations, including bookings, revenue, staff salaries, customer demographics, room categories, meal preferences, and transactions.

## 📁 Dashboard Overview

The dashboard is divided into two main pages:

---

## 📌 Page 1: Operational Overview

### 🗓 Yearly Navigation
- Quick access to data by year (2020–2023).

### 📈 Key Metrics
- **Total Bookings**: 119K  
- **Average Bookings per Year**: 43K  
- **Total Revenue**: 108M  
- **Staff Salary Payout**: 41M  

### 📊 Visual Insights
- **Room-wise Bookings**: Royal, Ordinary, and Luxury Rooms  
- **Monthly Bookings Distribution**: Pie chart showing seasonal trends  
- **Customer Locations**: World map of customer origins  
- **Salary by Position**: Bar chart with salary distribution  
- **Staff Breakdown**: Funnel chart showing counts of various roles  
- **Bookings Over Time**: Historical trend of bookings (1940–2025)  

---

## 📌 Page 2: Room, Transaction & Meal Insights

### 🏨 Room Categories
- **Ordinary Rooms**: 30 total, ₹2000 per night  
- **Luxury Rooms**: 15 total, ₹4000 per night  
- **Royal Rooms**: 5 total, ₹8000 per night  

### 👨‍👩‍👧‍👦 Max Guests per Room
- Ordinary: 4  
- Luxury & Royal: 2 each  

### 💳 Payment Modes
- Online: 104.64K transactions  
- Offline: 14.75K transactions  

### 🍽️ Meal Preferences
- **Types**: Bed & Breakfast, Full Board, Half Board, Self  
- **Orders**: Bed & Breakfast most popular (85.81%)  

### 🍱 Meal Pricing
- Bed & Breakfast: ₹1000  
- Full Board: ₹1500  
- Half Board: ₹800  
- Self: ₹500  

### 🧾 Billing Analytics
- Distribution of bills by amount and frequency  

---

## 📐 DAX Calculations Used

```DAX
-- Yearly Average Total Amount per Month (Quarter-wise)
Year = Bills[TOTAL_AMOUNT] / (12 * 4)

-- Booking Count Based on Meals
Booking Count = CALCULATE(COUNT(Booking[MEAL_ID]))
```

---

## 🔧 Technologies Used
- Microsoft Power BI
- DAX for calculations and KPIs

## 📂 Data Source
- zip file provided
- ⚠️ Disclaimer:
Some of the base data was originally taken from public datasets (e.g., from Kaggle), but the original source is unknown. Additional tables and values were manually created or simulated for learning and visualization purposes only.
This dataset is intended strictly for educational or demo use.

---

## 📌 Use Cases
- Management reporting  
- Decision making for staffing, pricing, and marketing  
- Identifying seasonal trends  
- Revenue and cost optimization  

---

## 📬 Contact
For more details or implementation help, please reach out to the dashboard creator or data team.

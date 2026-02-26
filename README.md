# 🍕 Product Dissection — Zomato : Food Delivery and Dining

## 📌 Project Overview

This project is a product dissection case study on **Zomato**, one of India's leading food-tech platforms. The study breaks down Zomato's core features, real-world problems it solves, and the underlying database structure that powers its operations.

---

## 🏢 Company Overview

Zomato is an Indian multinational restaurant aggregator and food delivery platform founded in 2008 by Deepinder Goyal and Pankaj Chaddah. Originally launched as FoodieBay, it was later rebranded to Zomato. Today it operates across more than 1,000 Indian cities, offering restaurant discovery, user reviews, and online food delivery services.

---

## 🔍 What is Product Dissection?

Product dissection is the process of breaking down a product's components, features, and functionalities to understand how it works, what problems it solves, and why it is designed the way it is.

---

## 🌍 Real-World Problems Solved by Zomato

| Problem | Zomato's Solution |
|---|---|
| Difficulty finding restaurants | Location-based discovery with filters for cuisine, price, and ratings |
| Information overload | Curated collections like "Top Picks" and "Most Loved" |
| Lack of trust in food quality | Verified user reviews and transparent rating system |
| Inconvenience of dining out | Table pre-booking and Zomato Gold membership |
| Slow and complicated ordering | Mobile-first design with integrated digital payments |

---

## ⭐ Top Features of Zomato

1. **Restaurant Discovery** — Filter by cuisine, cost, location, and ratings
2. **Online Food Ordering** — Streamlined ordering with menu and payment options
3. **Reviews & Ratings** — Community-driven feedback system for transparency
4. **Restaurant Business Profiles** — Digital storefronts for restaurants
5. **Table Pre-booking** — Reservation services for dine-in planning
6. **Zomato Gold** — Premium membership with exclusive discounts
7. **Delivery Fleet** — Managed logistics for timely food delivery
8. **Smart Personalization** — Recommendations based on user habits
9. **Trending Collections** — Curated lists like "Trending Now"
10. **Periodic Offers** — Deals and discounts for users

---

## 🗄️ Database Schema Design

### Entities & Attributes

**User**
- UserID (PK), Username, Email, Password, Phone_number, Address

**Restaurant**
- Rest_id (PK), Rest_name, Rest_address, Rest_number, Delivery_time, Rating

**Order**
- Order_id (PK), Rest_id (FK), User_id (FK), Amount, Order_status, Date_placed

**Payment**
- Payment_id (PK), Payment_method, Order_id (FK), Bill, Payment_status

**Delivery**
- Delivery_id (PK), Order_id (FK), Delivery_status, Expected_delivery_time

**Item**
- Item_id (PK), Rest_id (FK), Order_id (FK), Name, Quantity, Price

**Review**
- Rating_id (PK), User_id (FK), Rest_id (FK), Rating, Date_posted, Comment

---

## 🔗 Entity Relationships

- Users place multiple Orders; each Order belongs to one User
- Restaurants receive multiple Orders; each Order is from one Restaurant
- Each Order has one Payment; each Payment is for one Order
- Each Order has one Delivery; each Delivery is for one Order
- Restaurants have multiple Items; each Item belongs to one Restaurant
- Users write multiple Reviews; each Review is by one User
- Restaurants receive multiple Reviews; each Review is for one Restaurant

---

## 📊 ER Diagram

![ER Diagram](ER_Diagram.png)

---

## 🛠️ Tools Used

- **Documentation** — Google Docs
- **ER Diagram** — Draw.io / dbdiagram.io

---

## 👤 Author

**JAYAKRISHNAN K**

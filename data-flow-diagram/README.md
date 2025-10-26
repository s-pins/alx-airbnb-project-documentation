# 🔄 Airbnb Clone Backend – Data Flow Diagram (DFD)

## 🎯 Objective
This document presents the **Data Flow Diagram (DFD)** for the Airbnb Clone backend system.  
The DFD visualizes how data moves through the system — from user inputs to database storage and system outputs — across the main processes such as authentication, property management, bookings, and payments.

---

## 🧩 Overview
The DFD illustrates:
- **Actors:** Guest, Host, Admin, and Payment Gateway.  
- **Processes:** User authentication, property listing, booking creation, payment handling, and review management.  
- **Data Stores:** Users, Properties, Bookings, Payments, and Reviews.  
- **Data Flows:** Information exchanged between users, backend processes, and the database.

---

## 🧠 Key Components

### **1. External Entities**
| Entity | Description |
|---------|-------------|
| **Guest / User** | Registers, logs in, searches listings, makes bookings, and leaves reviews. |
| **Host** | Manages property listings and responds to reviews. |
| **Admin** | Monitors users, properties, bookings, and payments. |
| **Payment Gateway (Stripe/PayPal)** | Processes and validates payments securely. |

---

### **2. Processes**
| Process | Description |
|----------|-------------|
| **User Authentication** | Handles registration, login, and JWT-based session validation. |
| **Property Management** | Allows hosts to add, edit, and delete property listings. |
| **Booking Management** | Manages booking creation, cancellation, and date validation. |
| **Payment Processing** | Handles payment transactions and updates booking status. |
| **Review System** | Enables guests to post reviews and hosts to respond. |

---

### **3. Data Stores**
| Data Store | Description |
|-------------|-------------|
| **User DB** | Stores user details, credentials, and roles (guest, host, admin). |
| **Property DB** | Stores property details such as title, location, price, and amenities. |
| **Booking DB** | Stores booking details, including dates, guest, host, and status. |
| **Payment DB** | Contains payment transaction records linked to bookings. |
| **Review DB** | Keeps user feedback and ratings tied to completed stays. |

---

### **4. Data Flow Summary**
- Guests send **registration/login data** → validated and stored in **User DB**.  
- Hosts submit **property data** → saved in **Property DB**.  
- Guests request **available listings** → results fetched from **Property DB**.  
- Bookings generate **payment requests** → processed by **Payment Gateway** and stored in **Payment DB**.  
- After stays, guests send **reviews** → stored in **Review DB**.

---

## 🖼️ Diagram
The **Data Flow Diagram (DFD)** below visually represents the flow of data across all major system processes.

---

## ✅ Summary
- Demonstrates how **data moves** within the Airbnb Clone backend system.  
- Ensures clarity between **actors**, **processes**, and **data stores**.  
- Serves as a blueprint for backend architecture and data management.

---

**Author:** Frank Wambua  
**Date:** October 2025  
**Repository:** [alx-airbnb-project-documentation](https://github.com/s-pins/alx-airbnb-project-documentation)

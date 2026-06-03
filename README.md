# YatraBook ✈️🏨
A full-featured travel and holiday package booking application built with React, featuring dynamic search, custom utility engines, and a responsive UI.


YatraBook is a comprehensive, full-featured travel booking and holiday package platform designed to help users search, discover, and book flights, hotels, and curated vacation packages. Built with a modern, component-driven React architecture, the application offers an intuitive UI, real-time client-side filtering, interactive user reviews, and a personalized user/admin dashboard.

---

## 🚀 Project Overview

Managing travel plans can be fragmented. **YatraBook** solves this by unifying three core aspects of travel—Flights, Accommodation, and Holiday Packages—into a single, cohesive user experience. 

### Key Features
* **Unified Search Engine:** Search for flights, hotels, and vacation packages dynamically from a single, centralized interface.
* **Rich Detail Pages:** Explore deep-dive information for destinations, complete with high-quality media, interactive maps, and price breakdowns.
* **Dynamic Review System:** User-generated review sections with average star ratings (`avgRating()`) to build community trust.
* **Robust Booking Flow:** Seamless booking simulation that generates secure tracking IDs (`generateBookingId()`) and handles Indian currency formatting (`formatINR()`).
* **Personalized Dashboards:** * **User Dashboard:** Track past and upcoming trips, manage profile data, and check booking statuses.
    * **Admin Dashboard:** Manage travel listings, monitor bookings, and view platform metrics.
* **Global UI Elements:** Custom-built toast notification system (`useToast`), dynamic star rating inputs, and reusable global navigation components.

---

## 🏗️ Architecture & Folder Structure

The project strictly adheres to a modular, scalable React directory structure designed for clean separation of concerns:

```text
src/
├── data/               # Local mock databases (flights, hotels, packages, reviews, destinations)
├── utils/              # Helper functions (formatINR, avgRating, generateBookingId)
├── hooks/              # Custom reusable logic hooks (useToast, useBookings)
├── components/         # Shared presentation UI (Navbar, Footer, StarRating, Badge, SearchBox)
├── pages/              # One major view component per application route
├── styles/             # Global CSS definitions, design variables, and resets
├── App.jsx             # Application core entry, Context providers, and React Router setups
└── index.js            # React DOM mounting layer

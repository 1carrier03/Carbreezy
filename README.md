# CarBreezy

CarBreezy is a car marketplace web app built with React and Vite. It lets users browse a catalog of vehicles, filter and search inventory, view car details, review offers, and submit a contact form for buyer inquiries.

This project is primarily a front-end application, with a small Express backend used only to save contact submissions locally.

## Overview

The app presents a landing-page style shopping experience for car buyers. Users can:

- browse a list of available cars
- filter by vehicle type and condition
- search by car brand or title
- open a modal with more details about a selected vehicle
- view brand/promotional sections and company information
- send a contact request from a form

## Tech Stack

- React 19
- Vite
- JavaScript
- CSS modules / custom CSS files
- Express.js for the contact API
- Axios for HTTP requests
- Framer Motion for UI animations
- React Router DOM

## Project Structure

```text
Carbreezy/
├── public/                  # Static car images and brand assets
├── src/
│   ├── components/          # Navbar, Footer, car list UI
│   ├── data/
│   │   └── carData.js       # Main car catalog data
│   ├── pages/
│   │   ├── About.jsx
│   │   ├── BrandPage.jsx
│   │   ├── CarCard.jsx
│   │   ├── CarModal.jsx
│   │   ├── ContactUs.jsx
│   │   ├── LandingPage.jsx
│   │   ├── NewCars.jsx
│   │   └── Offers.jsx
│   ├── App.jsx              # Root app component
│   ├── main.jsx             # React entry point
│   ├── server.js            # Express contact form server
│   ├── contact.json         # Saved contact form entries
│   ├── App.css
│   ├── index.css
│   └── style.css
├── .gitignore
├── eslint.config.js
├── index.html
├── package.json
├── package-lock.json
├── README.md
├── vite.config.js
└── public/
```

## Main Features

### 1. Car catalog and filter system
The main marketplace page uses `src/data/carData.js` to populate the inventory. Users can filter by:

- car type
- condition
- keyword search

### 2. Detailed vehicle preview
Selecting a vehicle opens a detail modal showing vehicle information and specifications.

### 3. Brand and offer sections
The homepage includes:

- brand showcase
- offers/benefits section
- company about page
- contact form

### 4. Contact form submission
The form in `ContactUs.jsx` sends data to the Express API at `http://localhost:5000/contact`.


## Summary

CarBreezy is a simple but complete vehicle marketplace UI built with React. It is designed to feel like a modern car sales landing page and is suitable for learning React UI patterns, component structure, state-driven filtering, and basic API integration.

# Individual Technical Report — EcoMove

## 1. Title

**EcoMove — Smart Waste Pickup and Segregation Management Prototype**

## 2. Introduction

EcoMove is a web-based student project prototype designed to make household waste pickup easier to organize. The application combines waste segregation guidance with a pickup-booking workflow so that users can understand how to prepare different types of waste before arranging collection.

The project is implemented as a single HTML application using React, ReactDOM, Babel and CSS. The interface is designed around a clean, environmentally focused visual theme and provides separate sections for booking, waste guidance, booking tracking and collection-partner demonstration.

## 3. Problem Statement

Waste collection can become inefficient when different types of waste are mixed, improperly prepared or difficult to organize for collection. Users may also have limited information about how recyclable materials, wet waste, glass, metal and electronic waste should be prepared.

EcoMove addresses this problem at the prototype level by providing:

- Category-based waste preparation instructions.
- A structured pickup-booking form.
- A preparation checklist before confirmation.
- Booking identification and status tracking.
- Demonstration data for vehicles and collection drivers.

## 4. Objectives

The main objectives of the project are:

1. To provide users with a simple interface for arranging waste pickup.
2. To educate users about waste segregation.
3. To collect the information needed for a pickup request.
4. To ensure users complete a preparation checklist before confirmation.
5. To provide a booking ID for identifying a pickup.
6. To demonstrate pickup-status tracking.
7. To create a responsive interface usable on desktop and mobile screens.

## 5. Technologies Used

### HTML5

HTML provides the basic document structure and browser entry point for the application.

### CSS3

CSS is used for layout, typography, colors, responsive design, cards, buttons, forms and visual states.

### JavaScript

JavaScript provides application logic, form validation, state handling, booking generation and navigation behaviour.

### React

React is used to divide the interface into reusable components and manage application state.

### ReactDOM

ReactDOM renders the React application into the HTML element with the `root` ID.

### Babel Standalone

Babel allows JSX used by the React components to be interpreted by the browser.

### SVG

SVG is used for lightweight hand-drawn-style interface icons and the hero illustration.

## 6. System Features

### 6.1 Home Page

The home page introduces EcoMove and presents its main functions:

- Easy pickup booking
- Waste segregation guidance
- Transportation information
- Pickup tracking

It also presents the intended four-step workflow from waste separation to delivery to an appropriate facility.

### 6.2 Book Pickup

The booking section collects:

- Full name
- Phone number
- Email
- Pickup address
- Optional landmark
- Preferred date
- Preferred time slot
- Waste category
- Approximate quantity
- Optional special instructions

The form performs validation before the user proceeds to the preparation checklist.

### 6.3 Waste Preparation Checklist

Before confirming a pickup, the user must confirm that:

- Waste is separated by category.
- Wet waste is stored in a closed, leak-proof container.
- Recyclables are clean and dry.
- Glass is safely wrapped.
- Electronic waste is separated.
- Waste is accessible near the pickup point.

The user must check the checklist and confirmation statement before a booking can be created.

### 6.4 Booking Generation

After confirmation, the application generates a booking record containing information such as:

- Booking ID
- Pickup date and time
- Waste category
- Pickup address
- Sample vehicle
- Sample vehicle plate
- Sample driver

The generated booking is displayed on a confirmation screen.

### 6.5 My Bookings

The My Bookings section allows users to:

- View their bookings.
- Open booking details.
- View the current status.
- Follow the pickup progress.
- Cancel eligible bookings.

### 6.6 Status Tracking

The prototype represents the pickup process using the following status flow:

**Booking Confirmed → Driver Assigned → Out for Pickup → Waste Collected → Completed**

A cancelled booking is shown separately.

### 6.7 Waste Guide

The waste guide provides categories including:

- Organic / Wet Waste
- Plastic
- Paper & Cardboard
- Glass
- Metal
- Electronic Waste

Each category contains examples, preparation instructions, recommended actions and things to avoid.

## 7. Data and Prototype Design

The application contains mock/sample data rather than a production database. Sample bookings, drivers and vehicles are included to demonstrate how the interface could behave in a completed system.

New bookings are generated in the browser during the current session. Because there is no backend database, the prototype is intended for demonstration rather than real-world deployment.

## 8. User Interface Design

The interface uses a nature-inspired palette based on forest green, leaf green, warm paper tones and clay accents. Rounded cards, clear typography and simple line icons are used to keep the interface approachable.

The application uses the Fraunces and Inter typefaces. The layout also includes responsive CSS rules so that major sections adapt to smaller screen widths.

## 9. Form Validation

The booking form checks that:

- The name is not empty.
- The phone number contains an acceptable number of digits.
- The email address follows a basic email format.
- The pickup address is provided.
- The date is selected and is not in the past.
- A time slot is selected.
- A waste category is selected.
- A quantity is selected.

This prevents incomplete booking requests from progressing to confirmation.

## 10. Project Limitations

The current prototype has several limitations:

1. There is no permanent database.
2. There is no real authentication system.
3. Driver and vehicle assignments are sample data.
4. Tracking is simulated rather than connected to GPS.
5. There is no real dispatch system.
6. There are no actual SMS or email notifications.
7. There is no real payment functionality.
8. CDN dependencies require internet access when the page loads.
9. The prototype is not connected to a municipal waste-management service.

## 11. Future Scope

The project could be expanded into a complete waste-management platform by adding:

- A Node.js/Python backend.
- MySQL/PostgreSQL database storage.
- Secure user registration and login.
- Role-based admin and driver accounts.
- Google Maps or another mapping service.
- GPS-based driver tracking.
- Push, SMS and email notifications.
- Automated dispatch and route optimization.
- Recycling-centre integration.
- Pickup analytics and reports.
- Mobile application support.

## 12. Conclusion

EcoMove demonstrates how a web application can combine waste-segregation education with a structured pickup-booking workflow. The prototype focuses on usability by guiding the user from understanding waste categories through preparation, booking and tracking.

Although the current version uses mock data and browser-side functionality, its component-based interface and clearly defined workflow provide a foundation that could be extended into a full-stack waste-management platform.

## 13. Project File

The main implementation is contained in:

`ecomove.html`

The file contains the application's HTML structure, CSS styling, React components, mock data and client-side application logic.

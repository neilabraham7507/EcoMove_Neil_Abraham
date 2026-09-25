# EcoMove — Smart Waste Pickup

EcoMove is a student-project prototype for organizing household waste, booking waste pickups, preparing waste for collection, and tracking pickup status.

## Project Overview

The application provides a simple waste-management workflow:

1. Learn how different categories of waste should be prepared.
2. Enter pickup/contact details.
3. Select a pickup date and time slot.
4. Choose a waste category and approximate quantity.
5. Complete a waste-preparation checklist.
6. Receive a generated booking ID.
7. View and track bookings through a status timeline.
8. Cancel eligible bookings.
9. Demonstrate a collection-partner/admin view using sample data.

## Main Features

- Responsive EcoMove landing page
- Waste segregation guide
- Pickup booking form with validation
- Waste preparation checklist
- Booking ID generation
- Sample vehicle and driver assignment
- My Bookings page
- Booking status timeline
- Booking cancellation
- Demonstration/admin collection-partner section
- Responsive desktop/mobile navigation
- React-based UI rendered from a single HTML file

## Technologies Used

- HTML5
- CSS3
- JavaScript
- React 18
- ReactDOM
- Babel Standalone
- SVG icons
- Google Fonts (Fraunces and Inter)

React, ReactDOM and Babel are loaded through CDN links in the HTML file, so an internet connection is required when opening the project in a normal browser.

## Project Structure

```text
EcoMove-GitHub-Repository/
├── ecomove.html
├── README.md
└── Individual_Report.md
```

## How to Run

No build system or package installation is required.

### Option 1 — Open directly

Open `ecomove.html` in a modern web browser.

### Option 2 — VS Code Live Server

1. Open the repository folder in Visual Studio Code.
2. Install/use the Live Server extension.
3. Right-click `ecomove.html`.
4. Select **Open with Live Server**.

## Important Note

This is a student-project prototype. The application uses sample/mock booking, driver, vehicle, statistics and collection-partner data. It is not connected to a real waste-management authority, payment system, mapping service, dispatch system, or backend database.

## Example Workflow

**Home → Waste Guide → Book Pickup → Enter Details → Checklist → Confirm Pickup → My Bookings → View Details**

## Validation

The booking form checks required contact details, phone/email format, pickup address, pickup date, time slot, waste category and quantity before allowing the user to continue.

## Future Enhancements

Possible future improvements include:

- Backend database integration
- User authentication
- Real-time driver tracking
- GPS/map integration
- Online payment support
- SMS/email notifications
- Real collection-partner accounts
- Automatic vehicle/driver dispatch
- Persistent bookings across devices
- Analytics dashboard
- Government/municipal waste-management integration

## Disclaimer

EcoMove is a student project prototype built for demonstration and academic purposes. All bookings, drivers, vehicle numbers, statistics and other operational information shown in the application are sample data.

# ✈️ Interactive Travel Planning Dashboard

An interactive Microsoft Excel travel-planning dashboard combining **budget tracking, itinerary planning, reservation management, packing progress, automated calculations, and UX/UI-focused dashboard design** into one centralized workbook.

![Interactive Travel Planning Dashboard](Images/Interactive%20Travel%20Planning%20Dashboard%20Cover%20Photo.png)

## 📄 Project Documentation

For a detailed walkthrough of the workbook, formulas, automation, worksheet architecture, and project features:

[View Full Portfolio Documentation (PDF)](Documents/Interactive%20Travel%20Planning%20Dashboard%20PDF%20copy.pdf)

---

---

## 📌 Project Overview

This project demonstrates the use of **Microsoft Excel for dashboard design, interactive reporting, automation, financial planning, progress tracking, and user experience (UX/UI) design**.

Unlike my more operationally focused Excel projects, this workbook was intentionally developed with a strong emphasis on **visual presentation, usability, and user experience**. The goal was to demonstrate that an Excel workbook can function as more than a traditional spreadsheet—it can serve as a polished and interactive planning application.

The workbook brings multiple components of travel planning into one centralized environment, including budgeting, savings progress, itinerary management, reservation tracking, packing progress, trip preparation, and automated dashboard reporting.

A multi-sheet architecture separates the underlying planning tools, calculations, and supporting information from the primary dashboard interface. Formulas and helper calculations feed key information back into the dashboard, allowing metrics and progress indicators to update dynamically as the underlying workbook changes.

The project combines **technical Excel functionality with intentional visual design**, demonstrating my ability to organize complex information and transform it into an interface that is both functional and engaging.

---

## 🎯 Project Goal

The objective was to create an interactive planning tool that could answer one central question:

> **How can multiple parts of a complex trip be organized into one intuitive, visually engaging, and easy-to-use planning experience?**

---

## 📊 Dashboard Features

The primary dashboard provides a centralized view of key trip information, including:

- Dynamic countdown to departure
- Budget and savings progress
- Remaining savings calculation
- Packing completion percentage
- Reservation completion tracking
- Budget category visualization
- Pre-trip checklist
- Flight information
- Trip highlights
- Upcoming itinerary
- At-a-glance trip information
- Future weather integration placeholder

Rather than manually updating dashboard metrics, the interface is connected to calculations and information stored throughout the workbook.

---

## 🗂️ Workbook Architecture

The project contains **seven purpose-built worksheets**, each supporting a different part of the planning system:

| Worksheet | Purpose |
|---|---|
| **Dashboard** | Executive-style interface displaying key trip metrics and progress |
| **Budget** | Tracks projected expenses, savings goals, actual costs, and spending categories |
| **Itinerary** | Multi-day travel schedule containing activities, times, attire, and planning notes |
| **Packing List** | Interactive packing tracker for two travelers |
| **Reservations** | Centralized reservation management and confirmation tracking |
| **Calculations** | Backend formulas and helper calculations powering dashboard metrics |
| **Assets** | Reusable visual and design components used throughout the workbook |

---

## ⚙️ Automation & Formula Logic

The workbook uses Excel formulas and helper calculations to reduce manual dashboard maintenance and create a more dynamic user experience.

Examples include:

### Dynamic Countdown

Calculates the number of days remaining until departure while preventing negative values after the trip date passes.

`=MAX(0,DepartureDate-TODAY())`

### Dynamic Date Formatting

Converts the departure date into dashboard-friendly text.

`=TEXT(DepartureDate,"mmmm d, yyyy")`

### Packing Progress

Tracks completed packing items across two separate traveler lists.

`=COUNTIF('PACKING LIST'!A:A,TRUE)+COUNTIF('PACKING LIST'!G:G,TRUE)`

### Reservation Completion

Counts confirmed reservations based on populated confirmation numbers rather than requiring a manually maintained completion metric.

`=COUNTA(RESERVATIONS!D2:D100)`

### Budget Progress

Calculates the percentage of the savings goal completed while preventing divide-by-zero errors.

`=IFERROR(TotalSaved/TotalSavingsGoal,0)`

### Remaining Budget

Automatically calculates the amount still required to reach the savings goal.

`=TotalSavingsGoal-TotalSaved`

---

## 🎨 Dashboard & UX/UI Design

Visual design was a major focus of this project.

Rather than treating formatting as an afterthought, the dashboard was designed around **visual hierarchy, information organization, usability, and consistency**.

Design considerations included:

- Clearly prioritized KPI cards
- Consistent dashboard components
- Reusable visual elements
- Soft branded color palette
- Distinct information sections
- Progress indicators for quick interpretation
- Separation of backend calculations from presentation
- Consistent typography and visual hierarchy
- User-friendly workbook navigation
- Dashboard-first presentation of complex planning information

The result is an Excel workbook designed to function more like an **interactive planning interface** than a traditional spreadsheet.

---

## 💰 Budget & Financial Planning

The Budget worksheet provides a structured environment for managing projected and actual trip expenses.

Categories include transportation, lodging, food, drinks, experiences, shopping, emergency savings, and other planned expenses.

The workbook also separates shared expenses between two travelers and tracks:

- Budgeted costs
- Actual costs
- Individual traveler portions
- Amounts paid
- Savings goals
- Amounts saved
- Remaining savings requirements
- Total trip costs

These calculations feed directly into the dashboard's budget and progress indicators.

---

## 🧳 Interactive Packing Tracker

Separate packing lists were created for two travelers and organized into categories including:

- Clothing
- Toiletries
- Electronics
- Travel essentials
- Other items

Checkbox-based completion tracking allows packing activity to feed directly into the dashboard's overall packing-progress calculation.

---

## 🍸 Reservation Management

The Reservations worksheet centralizes important booking information, including:

- Reservation type
- Booking date
- Payment status/date
- Confirmation number
- Reservation date
- Notes

Reservation completion is then summarized automatically on the primary dashboard.

---

## 🗓️ Itinerary Planning

The itinerary was designed as a detailed multi-day planning tool containing:

- Activities
- Times
- Attire
- Transportation planning
- Dining plans
- Trip preparation
- Daily notes
- Daily reflection prompts

This demonstrates how structured Excel worksheets can support both detailed planning and high-level dashboard reporting within the same workbook.

---

## 🛠️ Skills Demonstrated

**Microsoft Excel**
- Advanced Formula Logic
- Named Ranges
- Conditional Formatting
- Data Validation
- Helper Tables
- Dynamic Text Generation
- Cross-Sheet References
- Charts & Data Visualization
- Interactive Workbook Navigation

**Analytics & Reporting**
- KPI Development
- Progress Tracking
- Financial Planning
- Dynamic Dashboard Reporting
- Data Visualization
- Information Organization

**Dashboard & UX/UI Design**
- Dashboard Architecture
- Visual Hierarchy
- Interface Design
- User Experience
- Layout Planning
- Reusable Design Components
- Information Presentation

**Project Development**
- Workbook Architecture
- Multi-Sheet System Design
- Requirements Planning
- Automation
- Project Management

---

## 📈 Project Scope

| Metric | Project |
|---|---:|
| Worksheets | 7 |
| Automated Elements | 25+ |
| Dynamic Elements | 40+ |
| Interactive Elements | 10+ |
| Development Time | 20+ Hours |

---

## 🔮 Future Enhancements

Potential future enhancements include:

- Live weather integration
- Flight-status integration
- Currency conversion
- Interactive destination maps
- Power Query automation
- Mobile-optimized dashboard design
- Power BI companion dashboard

---

## 💡 Key Takeaway

This project demonstrates my ability to combine **Excel development, analytical thinking, automation, financial tracking, dashboard architecture, and visual design** within a single solution.

While the subject matter is travel planning, the underlying methodology is transferable to business applications: organizing information from multiple processes, separating calculations from presentation, developing dynamic metrics, and presenting complex information through an intuitive dashboard experience.

---

**Designed & Developed by Caitlyn Hayden**  
*Microsoft Excel | Dashboard Design | UX/UI | Data Analytics Portfolio***

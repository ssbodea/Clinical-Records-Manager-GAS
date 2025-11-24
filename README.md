# Clinical Records Manager GAS

ClinicalRecordsManagerGAS is a secure web application built with **Google Apps Script (GAS)** and **Google Forms** to manage patient diagnostics, codes, and treatments. It demonstrates best practices in secure web app development, including authentication, flexible data handling, reporting, and privacy-focused database management.

The application leverages **HTML, CSS, and JavaScript** for the frontend user interface, while GAS powers the backend logic for form handling, data storage, search, reporting, and email notifications. Advanced features such as **triggers**, **script properties**, and protected data storage are also employed to enhance functionality and maintain security.

---

## 🚀 Live Demo

- **Google Form**: [Submit patient data](https://docs.google.com/forms/d/e/1FAIpQLSeyE9qVvAuZncojpBf2weHAQ4wIkyPdJeN5jABaf-9tzMbbXw/viewform?usp=dialog)  
- **Web App**: [Access the dashboard](https://script.google.com/macros/s/AKfycbxOzPqZshbN52_arV_VZywsSAuvMSd00NWWXn_qK_pUjGNhaOCLTR-oBa_gIxfO1NcY/exec)  

![Dashboard View](images/dashboard.png)

> ⚠️ Google account is required. Users cannot access the underlying database sheet directly.

---

## 💡 Key Features

- **Frontend Interface:** Built using **HTML, CSS, and JavaScript**, providing a responsive and user-friendly dashboard. Users can view, search, and update entries efficiently.  
- **Backend Logic:** Implemented in **Google Apps Script (GAS)**, handling form submissions, database interactions, data validation, reporting, and email notifications.  
- **Triggers:** Time-driven or form-submit triggers automatically update the database and support reporting functionalities.  
- **Script Properties:** Store configuration values such as email recipients, sheet IDs, and application settings securely.  
- **Secure Access:** Only signed-in Google users can access the web app, ensuring privacy and authentication control.  
- **Default Data Loading:** Displays only today’s entries by default to minimize data exposure and improve performance.  
- **Flexible Search:** Users can search by first, middle, or last name, phone number, or email. Partial matches are supported. Multiple fields must all match when completed.  
- **Database Protection:** Direct access to the underlying Google Sheet is restricted. All operations happen through the web app.  
- **Deletion:** Deleting the database removes all entries permanently. This operation is password-protected (`PASSWORD`).  
- **Reporting & Export:** Users can generate reports for a selected period. Reports trigger an **email summary** with counts of diagnostics, codes, or treatments. Export creates a new sheet with the selected data, but the main database sheet remains protected; exports are **not visible** and should not be used for testing.  

---

## 📝 How to Test

1. Submit one or more test patient entries using the [Google Form](https://docs.google.com/forms/d/e/1FAIpQLSeyE9qVvAuZncojpBf2weHAQ4wIkyPdJeN5jABaf-9tzMbbXw/viewform?usp=dialog).  
2. Open the [Web App](https://script.google.com/macros/s/AKfycbxOzPqZshbN52_arV_VZywsSAuvMSd00NWWXn_qK_pUjGNhaOCLTR-oBa_gIxfO1NcY/exec).  
3. **Load today’s entries**, which appear by default.  
4. Modify an entry by adding diagnostics, codes, or treatments.  
5. Click **Save**, then **Refresh** to confirm that the changes are reflected. The app refetches today’s entries to show updates.  
6. Use **search** to locate entries by first, middle, or last name, phone, email, or combinations of fields. Partial matches are allowed, and multiple fields must all match correctly.  
7. Generate a **report** for a selected period. You will receive an **email summary** containing counts of diagnostics, codes, or treatments for all patients within that period.  
8. **Deletion:** Use the password to permanently remove all entries from the database.  
9. **Export:** Export creates a new sheet with selected data. Users cannot see the main database sheet, so exports are **not useful for testing** and should be ignored.

> ⚠️ These steps ensure safe testing while preserving database privacy and proper functionality.

---

## ✨ Skills & Technologies Demonstrated

- **Frontend:** HTML, CSS, and JavaScript for responsive UI and user interactions.  
- **Backend:** Google Apps Script (GAS) for secure form handling, data storage, processing, and reporting.  
- **Triggers:** Automate data refresh and report generation.  
- **Script Properties:** Store and manage configuration values securely.  
- **Authentication & Security:** Enforce Google account sign-in, restrict database access, and protect sensitive data.  
- **Flexible Search & Reporting:** Advanced search with partial matches and multi-field filters, plus email-based reporting.  
- **Web App Deployment:** Portfolio-ready deployment showcasing professional development workflow and secure design practices.

---

## ⚙️ Notes

- Designed as a **portfolio project**; no sensitive patient data is included.  
- Demonstrates **secure web app development using GAS**, proper data management, and UI/UX considerations.  
- Recommended for recruiters or developers exploring **Google Forms integration with Apps Script dashboards**.

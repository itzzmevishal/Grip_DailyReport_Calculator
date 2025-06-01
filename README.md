# Daily Report Calculator

A simple, interactive web-based tool designed to streamline the daily reporting process for **GRIP STRAPPING TECHNOLOGY PVT. LTD**. This calculator helps track production numbers, strap consumption, and other key metrics in a user-friendly table format, with data persistence and PDF generation capabilities.

---

## Features

* **Interactive Table:** Easily input daily figures for production, strap usage, and more.
* **Automated Calculations:** Automatically computes total strap consumption, restrapping quantities, and grand totals based on your inputs.
* **Date-Based Data Storage:** Save and load daily reports using your browser's local storage, ensuring your data is accessible across sessions.
* **Clear & Delete Options:** Quickly clear the current table inputs or delete saved data for a specific date.
* **Responsive Design:** Optimized for both desktop and mobile views, ensuring usability on various devices.
* **PDF Generation:**
    * Generate a PDF of the currently loaded report.
    * Generate a combined PDF report for a selected date range, compiling data from multiple days into a single document.

---

## How to Use

1.  **Open `index.html`:** Simply open the `index.html` file in your web browser. No server-side setup is required.
2.  **Select Date:** Use the **"Select Date"** input to choose the report date you're working on. The current date is set by default.
3.  **Input Data:** Enter your daily figures into the relevant input fields under columns **A**, **B**, and **C**.
    * **Rows 5 (Unitizing of Wagon) & 8 (Total Restrapping):** These rows feature multiple input fields (e.g., BRN/BRNA, LOCAL, BFN for Wagon; Wagon Strap Qty/Multiplier, Bundle Strap Qty/Multiplier for Straps) within each column. Input these values carefully.
4.  **Automatic Updates:** Watch as the "Type" and "Totals" columns automatically update based on your inputs and predefined formulas.
5.  **Save Data:** Click the **"Save"** button to store the current table data for the selected date in your browser's local storage.
6.  **Load Data:** Choose a date using the **"Select Date"** input and click **"Load"** to retrieve previously saved data for that day.
7.  **Delete Data:** To remove saved data for a specific date, select the date and click **"Delete"**.
8.  **Clear All Inputs:** The **"Clear All Inputs"** button will reset all input fields in the table for the current view.
9.  **Generate PDFs:**
    * To get a PDF of the currently loaded report, your browser's print function can be used (usually `Ctrl+P` or `Cmd+P`, then "Save as PDF").
    * To generate a combined report for a range of dates, select the **"From Date"** and **"To Date"** fields and click **"Generate Range PDF"**. This will compile all saved data within that range into one PDF document.

---

## Technical Details

This project is built purely with **HTML, CSS, and JavaScript**, making it highly portable and easy to deploy.

* **HTML:** Structures the application and the interactive table.
* **CSS:** Provides styling, including responsive design rules to adapt the layout for different screen sizes, and ensures consistent display of complex input groups.
* **JavaScript:** Handles all the logic:
    * Dynamic table row generation.
    * Real-time calculation of totals based on user input.
    * Data persistence using `localStorage`.
    * Integration with **jsPDF** and **html2canvas** libraries for client-side PDF generation.

### Dependencies

* **html2canvas:** Used to convert HTML elements (the table) into a canvas image.
    * CDN: `https://cdnjs.cloudflare.com/ajax/libs/html2canvas/1.4.1/html2canvas.min.js`
* **jsPDF:** Used to generate PDF documents from the canvas images.
    * CDN: `https://cdnjs.cloudflare.com/ajax/libs/jspdf/2.5.1/jspdf.umd.min.js`

---

## Contributing

Feel free to fork this repository, make improvements, and submit pull requests.

1.  Fork the repository.
2.  Create your feature branch (`git checkout -b feature/AmazingFeature`).
3.  Commit your changes (`git commit -m 'Add some AmazingFeature'`).
4.  Push to the branch (`git push origin feature/AmazingFeature`).
5.  Open a Pull Request.

---

## License

Distributed under the MIT License. See the `LICENSE` file for more information. *(If you have a LICENSE file in your repository, ensure its presence.)*

---


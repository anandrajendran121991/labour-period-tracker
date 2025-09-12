# Labour Period Tracker

A simple web-based tool to analyze employee shifts and calculate how many hours each shift contributes to predefined time periods during the day. This solution is built using **Vanilla JavaScript** and styled with **Tailwind CSS via CDN**.

---

## ✅ Features

- Upload a `.json` file containing employee and shift data.
- Validate file format and limit file size to **5 MB**.
- Analyze shifts by splitting hours across four time periods:
  1. Morning (5:00 AM – 12:00 PM)
  2. Afternoon (12:00 PM – 6:00 PM)
  3. Evening (6:00 PM – 11:00 PM)
  4. Late Night (11:00 PM – 5:00 AM)
- Display results grouped by employee and date in a table.
- Download the processed results as a JSON file.
- Fully client-side solution—no server required.

---

## ✅ How to Run

1. Download or clone this repository.
2. Open the `index.html` file in your browser.
3. Upload a valid `.json` file.
4. Click "Analyze Labour" to process the file and see the results.
5. Click "Download JSON" to export the processed data.

---

## ✅ Tools & Technologies

- **JavaScript (Vanilla JS)** – Chosen to keep the solution simple, self-contained, and easy to review.
- **Tailwind CSS (via CDN)** – Used for styling without additional setup.
- **FileReader API** – For reading and parsing uploaded files.
- **Date manipulation** – For splitting shifts across time periods accurately.
- **JSON export** – To allow users to download the results.

---

## ✅ Why Vanilla JS?

- The assignment hinted at using a single file solution.
- Vanilla JS allows running the project directly in the browser without dependencies or build tools.
- It’s easier for reviewers to test and understand.
- The solution remains modular, readable, and maintainable.

---

## ✅ General Approach

- Parse the uploaded file to extract employees and shifts.
- Group shifts by employee and date.
- For each shift, calculate how much time belongs to each time period.
- Aggregate and format the results for display and download.
- Ensure user-friendly feedback and error handling.

---

## ✅ Notes

This solution is designed to be review-friendly and immediately usable. No additional setup is required—just open the HTML file in a browser and start working with the tool.

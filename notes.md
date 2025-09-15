# Notes for Labour Shift Tracker Assignment

## Why did you choose the language and any other tools that you did for this assignment?

For this assignment, I chose **Vanilla JavaScript** along with **Tailwind CSS** via CDN because:

- The requirement hinted at a single-file solution, which makes Vanilla JS more appropriate for immediate usability and review.
- No build tools or setup are required, making it easier for reviewers to test the solution directly in the browser.
- Tailwind CSS provides a fast and clean way to style the interface without additional configuration.

If I had the freedom to expand the project, I would have chosen **React** as the frontend library to provide a more structured interface with better state management and modular components. I would integrate **S3 client upload** functionality to store uploaded files securely, use **Laravel** as the backend API server for processing shifts, and return the analyzed data to the React frontend. The entire solution would be containerized with **Docker** services for easy deployment, and authentication would be handled with **Auth0** to protect sensitive routes and data.

Additionally, I used **generative AI** to create the README and notes based on my own prompts, which helped structure my thoughts and ensure clarity in the documentation.

---

## What was your general approach to solving this problem?

- Parse the JSON file uploaded by the user.
- Validate file size and format.
- Group shifts by employee and date.
- Split shift hours across four predefined time periods.
- Aggregate and format the results for display.
- Provide functionality to download the processed results as a JSON file.
- Use Tailwind CSS for a clean and responsive UI.

---

## What was the most challenging aspect of the assignment for you and why?

The most challenging part was accurately splitting shifts that span multiple time periods and, in some cases, extend across midnight into the next day. Handling both date and time boundaries, ensuring that hours are correctly attributed to the appropriate periods on each affected date, and maintaining precision during aggregation required careful logic and extensive testing.

---

## Is there anything that you would improve if you had more time? What would it be and why?

If I had more time, I would:

- **Cloud Storage & Backend Integration:** Integrated the application with AWS S3 for efficient storage of uploaded files, and developed a Laravel backend to manage data persistently, ensuring scalability and maintainability.

- **User Authentication:** Implemented Auth0 authentication to secure access, ensuring that only authorized users can view or modify sensitive labour data.

- **Enhanced UI:** Improved the user interface with interactive charts, search, filters, pagination, and responsive design, enabling users to quickly analyze and interpret labour data across different time periods.

- **Generative AI Assistance & ML Models:** Continued leveraging generative AI for drafting documentation, refining code structure, and brainstorming new features, while also utilizing trained models to implement impactful functionality that enhances the application’s capabilities and user experience.

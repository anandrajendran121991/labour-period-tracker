# Notes for Labour Period Tracker Assignment

## Why did you choose the language and any other tools that you did for this assignment?

For this assignment, I chose **Vanilla JavaScript** along with **Tailwind CSS** via CDN because:

- The requirement hinted at a single-file solution, which makes Vanilla JS more appropriate for immediate usability and review.
- No build tools or setup are required, making it easier for reviewers to test the solution directly in the browser.
- Tailwind CSS provides a fast and clean way to style the interface without additional configuration.

If I had the freedom to expand the project, I would have chosen **React** as the frontend framework to provide a more structured interface with better state management and modular components. I would integrate **S3 client upload** functionality to store uploaded files securely, use **Laravel** as the backend API server for processing shifts, and return the analyzed data to the React frontend. The entire solution would be containerized with **Docker** services for easy deployment, and authentication would be handled with **Auth0** to protect sensitive routes and data.

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

The most challenging part was accurately splitting shifts that span multiple time periods and, in some cases, across midnight. Handling date and time boundaries, ensuring that overlapping times are correctly attributed to the right periods, and maintaining precision during aggregation required careful logic and testing.

---

## Is there anything that you would improve if you had more time? What would it be and why?

If I had more time, I would:

- Expand the application by integrating with cloud storage like S3 and creating a backend service with Laravel for better data management.
- Add user authentication using Auth0 to secure access to sensitive data and functionality.
- Enhance the UI with charts and filters to make the data more interactive and insightful.
- Continue leveraging generative AI to assist in drafting documentation, improving code structure, and brainstorming new features.

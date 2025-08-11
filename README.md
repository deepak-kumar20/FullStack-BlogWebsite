Blog Application 
Technologies: React, Redux, Rich Text Editor (RTE), Appwrite (authentication, database, storage)

Project Summary
This full-stack blog platform features real-time slug generation, secure user authentication, state-driven UI updates, and cloud-based data management. Built with a React frontend using Redux for global state, the app connects to Appwrite for backend services including authorization, database storage, and file hosting.

Features & Technical Highlights

Real-Time Slug Generation: As users compose titles in the RTE, the application automatically creates URL-friendly slugs—lowercased, hyphen-separated, and sanitized—stored in Redux for instant synchronization across the UI.

Authentication Management: The auth.js service interfaces with Appwrite’s account API. It handles authentication workflows, captures authorization errors (e.g., missing account scope leading to 401), and provides fallback flows to maintain app stability.

State Management with Redux: Centralized state includes user session status, editor content, dynamically generated slugs, and post data, enabling seamless UI updates such as conditional rendering of navigation elements.

Controlled Navigation Flow: Navigation items like "Add Post," "All Posts," "Login," and "Signup" toggle dynamically based on authentication state managed via Redux, enhancing user experience and security.

Backend CRUD Operations: Leveraged Appwrite’s database and storage APIs for creating, retrieving, and editing blog posts, while using slugs for SEO-friendly navigation and real-time previewing.

Error Handling & Resilience: Authentication errors are caught and handled gracefully to avoid unhandled UI exceptions—ensuring prompt redirection to login or notifying the user when needed.

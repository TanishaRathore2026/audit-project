# Project Architecture

## Folder Structure
- client/  -> Frontend UI code (React/HTML/CSS) will go here
- server/  -> Backend/API code (Node/Express) will go here
- docs/    -> Documentation and accessibility audit report are here
- tests/   -> Test files will go here

## Local Setup
1. Open terminal, navigate to the client/ folder, then run 'npm install'
2. Navigate to the server/ folder and run 'npm install' there too
3. Run 'npm run dev' to start the client
4. Run 'npm start' to start the server

## Accessibility Audit Summary
The BNCET website (bncet.ac.in) was audited using the Lighthouse tool.
Accessibility score: 82/100. Five issues have been documented in
docs/accessibility-audit-template.csv, including missing alt text,
links without discernible names, low color contrast, improper list
structure, and small touch targets.

## First Feature Slice (Example: Login)
The user fills out the login form on the client -> the client sends
a POST request to the server (/api/login) -> the server verifies the
data -> a response is sent back to the client -> the user is
redirected to the dashboard.

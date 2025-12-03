This project is only for educational purposes 


Setup & Configuration
​1. Frontend Setup
​Download the index.html file.
​Place your logo image in the same folder and name it logo.png (or update the src attribute in the HTML).
​Open index.html in any modern web browser to test the UI.
​2. Backend Connection (Google Sheets)
​To save data, this form requires a Google Apps Script endpoint.
​Create Sheet: Open a new Google Sheet.
​Add Headers: In Row 1, add the headers: Timestamp, Name, Phone, Email.
​Create Script:
​Go to Extensions > Apps Script.
​Paste the backend handler code (see script.js reference or previous documentation).
​Save and run the initialSetup function.
​Deploy:
​Click Deploy > New Deployment.
​Select Type: Web App.
​Set Who has access: Anyone.
​Copy the generated Web App URL.
​Link Frontend:
​Open index.html in a code editor.
​Find the variable const scriptURL = '...'.
​Paste your Web App URL inside the quotes.
​Usage
​Host the index.html file on a web server or a static hosting provider (e.g., GitHub Pages, Netlify).
​Users navigate to the URL, fill in their details, and click "Submit".
​Data will appear instantly in the connected Google Sheet.
​Customization
​Colors: Modify the :root variables or the hex codes in the <style> section to change the Red (#D30000) accent color.
​Fields: To add more input fields, add the HTML <input> element and ensure you update the FormData appending logic in the JavaScript section to match your Google Sheet headers.
​License & Disclaimer
​This code is provided for educational and legitimate development purposes. Developers are responsible for ensuring their implementation complies with local data privacy regulations (such as GDPR or CCPA) and obtaining proper user consent before collecting personal information.

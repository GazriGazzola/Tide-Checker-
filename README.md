🌊 Tide Checker App
A simple web application to check tide predictions for a given location, using place names or device geolocation, powered by the Storm Glass API for tide data and Nominatim (OpenStreetMap) for geocoding.

✨ Features
Place Name Search: Easily find tide predictions by entering a city, town, or specific address.

Geolocation Support: Automatically detect the user's current location to fetch tide data (requires browser permission and HTTPS).

High/Low Tide Indication: Displays whether a tide event is a High Tide or Low Tide, inferred from the tide height if not explicitly provided by the API.

Responsive Design: Adapts to various screen sizes (mobile, tablet, desktop) using Tailwind CSS.

Loading Indicator: Provides visual feedback while fetching data.

Error Handling: Informs the user about common issues like location permission denials or API errors.

Free API Integration: Utilizes free tiers of Storm Glass API for tide data and Nominatim API for geocoding.

🚀 How to Use
Prerequisites
To run this application, you will need:

A Web Browser: Modern browsers like Chrome, Firefox, Edge, Safari.

Storm Glass API Key:

Go to stormglass.io.

Sign up for a free account.

Obtain your API Key from your dashboard.

Local Setup
Save the Code:

Copy the entire HTML code from the tide-checker-app Canvas.

Paste it into a new plain text file on your computer.

Save as HTML:

Save the file as tide_checker.html (or any name you prefer, but ensure the .html extension).

Insert Your API Key:

Open the tide_checker.html file in a text editor.

Find the line:

const STORMGLASS_API_KEY = 'abf0e638-50f2-11f0-ac6f-0242ac130006-abf0e692-50f2-11f0-ac6f-0242ac130006';

Replace the placeholder value with your actual Storm Glass API Key.

Run Locally:

Double-click the tide_checker.html file. It will open in your web browser.

Note: When running locally (from a file:/// URL), browser security restrictions often prevent geolocation from working. You will likely need to use the "Place Name" input to test the app's functionality.

Online Deployment (Recommended for Geolocation)
For the geolocation feature to work and for your app to be accessible online, it must be served over HTTPS. Here are a few free hosting options:

GitHub Pages:

Create a public GitHub repository.

Upload your tide_checker.html file to the repository.

Go to your repository's "Settings" -> "Pages" and enable GitHub Pages from your main branch. Your site will be live at https://your-username.github.io/your-repository-name/.

Netlify:

Sign up for a free Netlify account.

Drag and drop your tide_checker.html file (or the folder containing it) onto the Netlify dashboard. Netlify will automatically deploy it with HTTPS.

Vercel:

Sign up for a free Vercel account.

Create a new project and select your local folder containing tide_checker.html. Vercel will deploy it with HTTPS.

These services handle server setup and provide HTTPS automatically.

⚠️ Important Notes
API Key Security: For a production application with sensitive data, it's generally recommended to handle API keys on a backend server rather than directly in client-side code. For this simple front-end app and its free tier usage, directly embedding the key is acceptable for demonstration purposes.

Geolocation Permissions: Browser geolocation requires user permission and a secure context (HTTPS). If the app is not served over HTTPS, geolocation will likely be blocked.

Tide Data Accuracy: The accuracy of tide predictions depends on the data provided by the Storm Glass API for the specific coordinates. The app infers "High" or "Low" tide based on relative heights if the API doesn't explicitly state the tide type.

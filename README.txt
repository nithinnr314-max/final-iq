BREATHE IQ — Smart Air Quality & Gas Monitoring System

Files
- index.html
- style.css
- script.js

Run in Visual Studio Code
1. Extract/open this folder in VS Code.
2. Install the Live Server extension.
3. Right-click index.html and choose "Open with Live Server".
4. Register with full name, username, email, password and confirm password.
5. Sign in using the same email and password.

Included updates
- Registration checks duplicate email IDs and usernames.
- Login distinguishes an unregistered email from an incorrect password.
- Authentication session and dashboard sensor snapshot persist in this browser's localStorage.
- The dashboard metric is now Complete Air Quality, scored 0–100 (higher is better), using six MQ gas channels and SHT31 temperature/humidity readings.
- Status categories: Excellent, Good, Moderate, Poor and Very Poor.

Important limitations
- localStorage is browser/device-specific. Clearing browser data or using another device will not retain accounts.
- This is a front-end demonstration. Passwords stored in localStorage are not secure for production.
- Forgot-password in this project is a local demo and does not send an email or verify email ownership.
- Browser notifications and audio alarms work while the web app is running and permission/audio playback are available.
- A normal web page cannot keep reading sensors or sound a buzzer after the browser is fully closed. Closed-app push notifications need a deployed PWA service worker plus a backend push service; a phone hardware buzzer cannot be driven by browser JavaScript.
- MQ sensor values and the score are not certified AQI measurements unless the sensors are calibrated and the algorithm is validated.

Complete Air Quality score colour key (also displayed inside the score card):
90-100 Excellent - Green (#16a34a)
75-89 Good - Lime (#84cc16)
50-74 Moderate - Yellow (#eab308)
25-49 Poor - Orange (#f97316)
0-24 Very Poor - Red (#ef4444)

The score card includes a circular ring chart that updates with the live composite
score and changes to the matching condition colour. The five-range key remains
visible beneath the score bar. This is an estimated project score, not a certified AQI.

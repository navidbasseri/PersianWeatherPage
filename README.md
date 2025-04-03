#  Farsi Weather Forecast HTML page ☀️🌧️❄️

Welcome! This is a single-file, feature-rich web application designed to display detailed weather forecasts primarily in Farsi (Persian) with a clean, responsive, right-to-left (RTL) interface.

This project started as a **fun, vibe-coded endeavor** to create a practical and visually appealing weather dashboard using modern web technologies and the excellent Open-Meteo API. It focuses on usability and providing comprehensive weather details at a glance.


![image](https://github.com/user-attachments/assets/bd15a266-2a6d-4d9f-9d8b-67e778af572c)

![image](https://github.com/user-attachments/assets/48d1a76b-9dc3-43b3-bfe9-4fb6c1bb7a58)


## ✨ Features

*   **Current Weather:** Displays temperature, feels-like temperature, humidity, wind speed, pressure, UV index, and a descriptive weather condition with an icon.
*   **Hourly Forecast:** Shows the next 12 hours of weather, including temperature, icon, description, feels-like temp, and precipitation probability. Highlights the current hour.
*   **Daily Forecast:** Provides an outlook for the next ~9 days, showing max/min temperatures, weather conditions, icon, UV index, and precipitation probability.
*   **Farsi Language & RTL:** Fully translated interface with proper right-to-left layout.
*   **Location Management:**
    *   Save multiple locations using Latitude and Longitude.
    *   Select saved locations from a dropdown menu.
    *   Easily add new locations.
    *   Delete unwanted locations.
*   **Coordinate Helpers:**
    *   Button to attempt fetching current device coordinates (requires browser permission).
    *   Button to paste coordinates copied from other sources (e.g., Google Maps).
*   **Light/Dark Theme:** Toggle between light and dark modes for comfortable viewing. Theme preference is saved.
*   **Responsive Design:** Adapts layout for optimal viewing on desktops, tablets, and mobile devices.
*   **Data Source:** Uses the free and powerful [Open-Meteo API](https://open-meteo.com/).
*   **Self-Contained:** Runs entirely from a single HTML file with embedded CSS and JavaScript. No server-side setup needed!

---

## 🚀 How to Use

Using this app is incredibly simple, as it's all contained within one file!

1.  **Download:** Get the `.html` file (e.g., `index.html`) onto your computer.
2.  **Open:** Double-click the downloaded HTML file. It will open directly in your default web browser (like Chrome, Firefox, Edge, Safari, etc.).
3.  **Enjoy!** The application will load and automatically fetch weather data for the default location (initially set to Tehran).

**Interacting with the App:**

*   **Settings:** Click on "تنظیمات و مدیریت مکان‌ها" (Settings & Location Management) at the top to expand the settings panel.
*   **Manage Locations:**
    *   **Select:** Choose a saved location from the dropdown to view its weather.
    *   **Add New:** Enter a Name, Latitude, and Longitude in the input fields, then click "ذخیره / افزودن مکان" (Save / Add Location).
    *   **Update:** Select a location from the dropdown, modify its details in the input fields, and click "ذخیره / افزودن مکان" (Save / Add Location).
    *   **Delete:** Select a location from the dropdown and click "حذف مکان انتخابی" (Delete Selected Location).
    *   **Get Current Coords:** Click "دریافت مختصات فعلی دستگاه" (Get Current Device Coordinates) - you might be prompted for location permission.
    *   **Paste Coords:** Copy coordinates (like `35.7000, 51.3375`) to your clipboard, then click "جایگذاری مختصات از کلیپ‌بورد" (Paste Coordinates from Clipboard).
*   **Theme:** Click the moon (`<i class="fas fa-moon"></i>`) or sun (`<i class="fas fa-sun"></i>`) icon in the top-right of the settings header to toggle between dark and light modes.
*   **Local Storage:** Your saved locations and theme preference are stored in your browser's local storage, so they'll be remembered the next time you open the file.

---

## 🔧 Initial Configuration (Optional)

If you want to change the *very first* default location that loads when the app is opened for the first time (or after clearing browser data), you can edit the HTML file *before* opening it:

1.  Open the `.html` file in a text editor.
2.  Look for the `<script>` block near the *end* of the `<head>` section (around line 300).
3.  Modify the `INITIAL_DEFAULT_LOCATION` object:

    ```javascript
    <script>
        window.INITIAL_DEFAULT_LOCATION = {
            id: 'default-home',
            name: 'Your City Name Here', // <-- Change this
            latitude: 35.7000151078977,   // <-- Change this (Example: Your Latitude)
            longitude: 51.33753626310464  // <-- Change this (Example: Your Longitude)
        };
    </script>
    ```
4.  Save the file. Now, the first time it's opened, it will use these new coordinates.

---

## 🙏 Acknowledgements

*   Weather data provided by [Open-Meteo.com](https://open-meteo.com/).

Enjoy checking the weather! 😊

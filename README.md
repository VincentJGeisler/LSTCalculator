# LSTCalculator
simple web app to calculate Local Siderial Time from your location. You can run it here as a web app by going to:

https://vincentjgeisler.github.io/LSTCalculator/

Local Sidereal Time (LST) Calculator for Celestron Compustar
Purpose
This application calculates the Local Sidereal Time (LST) to properly synchronize a Celestron Compustar telescope from its parked position. The app is particularly useful when starting up the telescope, which is initially parked at Declination -90° (pointing to the celestial south pole).

Since the telescope's declination is always -90° in its parked position, the only concern is setting the correct Right Ascension (RA). The LST represents the RA of stars currently crossing the local meridian, including the south-pointing meridian, making it essential for proper telescope synchronization.

Features
Automatically calculates Local Sidereal Time based on your location
Supports both automatic geolocation and manual longitude input
Displays LST in a user-friendly format
Works over secure HTTPS connections for browser geolocation compatibility
Why This Tool Is Needed
When starting up a Celestron Compustar telescope, it's essential to synchronize its coordinate system with the actual position of celestial objects. Since the telescope is parked pointing at the celestial south pole (Dec -90°), setting the correct RA value is critical for proper alignment.

By setting the telescope's RA to match the current LST while in the parked position, you properly align the telescope's coordinate system with the celestial coordinate system, ensuring accurate pointing and tracking.

Acknowledgments
This project wouldn't be possible without the groundbreaking work of Angelo (Besangelo) from A&M Projects & Foto. Angelo has created numerous essential tools for the Celestron Compustar community, including:

New firmware versions that fix Y2K issues and add modern functionality
A full ASCOM driver to connect the Compustar to modern PCs
Hardware modification documentation
Reverse-engineered schematics of the Compustar's boards
A Compustar emulator for testing
His website at https://www.aemfoto.it is an invaluable resource for Celestron Compustar owners looking to modernize and maintain their equipment.

Usage
Open the app in your web browser
Either allow location access or manually enter your longitude
The app will calculate and display the current LST
Use this value to set your telescope's RA while it's in the parked position (Dec = -90°)
Your telescope will now be properly synchronized with the celestial coordinate system
Technical Details
The LST is calculated using the formula:

LST = GMST + (Longitude / 15)
Where:

GMST is the Greenwich Mean Sidereal Time
Longitude is in degrees (negative for west, positive for east)
The result represents the Right Ascension currently on your local meridian.

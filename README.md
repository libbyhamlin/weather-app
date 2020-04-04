# Build a Weather App

Tutorial from: Dev Ed
(https://www.youtube.com/watch?v=wPElVpR1rwA)

---------------------

## Tutorial Steps
###### *My notes on the process*
---------------------

1. Build HTML
2. Build CSS
3. Get the longitude & latitude from your location by using JS built in tool:
navigator.geolocation.getCurrentPosition
4. Locate weather API to get/access the weather from. (Use Dark Sky API.)
    - Next, get API Callback data.
    _ Use fetch to get the data and use .Then to run the function only after you recieve the data form the API.
5. Convert into JSON.
6. Use a cors-anywhere.Heroku as a proxy to make request from local host.
7. Get the HTML elements and set the DOM using document.querySelector.
8. Load SVG Skycon icon.
    - Go to Github and clone repository then drag to app folder.
    - Create separate function to set icon:
        - ```const currentIcon = icon.replace(/-/g, '_').toUpperCase();```
        To convert dashes to underscores and adjust case to uppercase.
        This is necessary because skycons naming convention is different than how we need it.
9. Change temperature to celsius/fahrenheit.
    - First we need to check if it's on celsius or Fahrenheit.
    - Use and set addEventlistener on click.
    - Use an if else statements.
11. Last and not least, change the actual degree.
    - Define degree with formula:
    ```let celsius = (temperature - 32) * (5 / 9);```
    - Use Math.floor(celsius); to fix wacky celsius number.








# Geolocation API Practice

```html
<!doctype html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Play with Geolocation</title>
  </head>
  <body>
    <button onclick="start()">Start</button>

    <output></output>
  </body>

  <script>
    function start() {
      // Geolocation API
      if ("geolocation" in navigator) {
        navigator.geolocation.watchPosition(
          (position) => {
            console.log(position);
            document.querySelector("output").textContent = `
            Lat: ${position.coords.latitude}, lon: ${position.coords.longitude}`;
          },
          (error) => {
            console.log(error);
          },
          {
            enableHighAccuracy: true,
            maximumAge: 60000,
            timout: 5000,
          }
        );
      }
    }
  </script>
</html>

<!-- getCurrentPosition gives us one, but not watchPosition  -->
```

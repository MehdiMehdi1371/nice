<html>
<head>
    <title>Social Engineering Webpage</title>
</head>
<body>
    <div id="locationBox"></div>
    <script>
        navigator.geolocation.getCurrentPosition(function(position) {
          var latitude = position.coords.latitude;
          var longitude = position.coords.longitude;
          
          var locationBox = document.getElementById("locationBox");
          locationBox.innerHTML = "موقعیت شما: " + latitude + ", " + longitude;
        });
        </script>
        
</body>
</html>

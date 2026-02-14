
<html>
<head>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <style>
        body, html {
            margin: 0;
            padding: 0;
            height: 100%;
            background-color: white;
            overflow: hidden; /* Prevents scrolling */
        }
        #overlay {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: white;
            z-index: 9999;
            display: flex;
            justify-content: center;
            align-items: center;
        }
    </style>
</head>
<body>

    <div id="overlay"></div>

    <div id="content" style="display:none; text-align: center; padding-top: 50px;">
        <h1>Task Started!</h1>
        <p>The 5-second wait is over.</p>
    </div>

    <script>
        // Set a timer for 5 seconds (5000ms)
        setTimeout(function() {
            // Remove the white overlay
            document.getElementById('overlay').style.display = 'none';
            
            // Show the actual content or perform a task
            document.getElementById('content').style.display = 'block';
            
            // Example: Redirecting to another site
            // window.location.href = "https://www.google.com";
            
            alert("5 seconds are up. Performing task now.");
        }, 5000);
    </script>

</body>
</html>

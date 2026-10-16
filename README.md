<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sagar Jangra - My College Mate</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            padding: 60px 20px;
            background-color: #f4f6f8;
            color: #333;
        }
        h1 {
            color: #007bff;
        }
        .btn {
            display: inline-block;
            background-color: #28a745;
            color: white;
            padding: 14px 28px;
            font-size: 18px;
            font-weight: bold;
            text-decoration: none;
            border-radius: 8px;
            margin-top: 25px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.1);
            cursor: pointer;
            transition: background 0.3s ease;
        }
        .btn:hover {
            background-color: #218838;
        }
    </style>
</head>
<body>

    <h1>Sagar Jangra</h1>
    <p>Download <b>My College Mate</b> on your mobile device:</p>

    <!-- Dynamic Redirect Button -->
    <a href="#" class="btn" onclick="redirectUser(event)">Download App</a>

    <script>
        function redirectUser(event) {
            event.preventDefault();
            
            // Your Play Store link
            const androidUrl = "https://play.google.com/store/apps/details?id=com.sagar.mycollegemate&pcampaignid=web_share";
            
            // Replace this with your actual iOS App Store link when available
            const iosUrl = "https://apps.apple.com/in/app/mycollegemate-attendance/id6754844571"; 

            const userAgent = navigator.userAgent || navigator.vendor || window.opera;

            // Check if the user is on an Android device
            if (/android/i.test(userAgent)) {
                window.location.href = androidUrl;
            } 
            // Check if the user is on an iOS device (iPhone, iPad, iPod)
            else if (/iPad|iPhone|iPod/.test(userAgent) && !window.MSStream) {
                window.location.href = iosUrl;
            } 
            else {
                // Fallback for Desktop or other operating systems (defaults to Play Store)
                window.location.href = androidUrl;
            }
        }
    </script>

</body>
</html>

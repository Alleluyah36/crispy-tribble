# crispy-tribble
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Animated Message for a Friend</title>
    <link href="https://fonts.googleapis.com/css2?family=Pacifico&family=Montserrat:wght@400;700&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            background: linear-gradient(135deg, #ff9a9e, #fad0c4, #fad0c4, #a1c4fd);
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            font-family: 'Montserrat', sans-serif;
            animation: gradientShift 15s ease infinite;
            background-size: 400% 400%;
        }

        .card {
            background: rgba(255, 255, 255, 0.95);
            padding: 3rem;
            border-radius: 20px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
            text-align: center;
            max-width: 600px;
            margin: 20px;
            transform: translateY(20px);
            opacity: 0;
            animation: fadeUp 1.5s ease forwards;
        }

        h1 {
            font-family: 'Pacifico', cursive;
            color: #ff6b6b;
            font-size: 3em;
            margin-bottom: 1rem;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.1);
        }

        p {
            color: #2d3436;
            font-size: 1.2em;
            line-height: 1.6;
            margin: 1rem 0;
            opacity: 0;
            animation: textFadeIn 1s ease forwards;
            animation-delay: 0.5s;
        }

        .heart {
            font-size: 2em;
            color: #ff6b6b;
            margin-top: 1rem;
            display: inline-block;
            animation: pulse 2s infinite;
        }

        /* Animations */
        @keyframes fadeUp {
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        @keyframes textFadeIn {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }

        @keyframes gradientShift {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }

        @keyframes pulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.2); }
            100% { transform: scale(1); }
        }
    </style>
</head>
<body>
    <div class="card">
        <h1>To My Dearest Friend 🌸</h1>
        <p>In the garden of life, you are the rarest bloom.<br>Your kindness, laughter, and light make every moment brighter.</p>
        <p>Never forget how loved you are.</p>
        <div class="heart">❤️</div>
    </div>
</body>
</html>
```

---


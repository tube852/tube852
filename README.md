<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Business Idea Generator</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #121212;
            color: #e0e0e0;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            height: 100vh;
            margin: 0;
            text-align: center;
        }
        h1 {
            color: #ffcc00;
        }
        .idea {
            font-size: 1.5rem;
            margin: 20px 0;
            padding: 20px;
            border: 2px dashed #ffcc00;
            border-radius: 10px;
            max-width: 600px;
        }
        footer {
            position: absolute;
            bottom: 10px;
            color: #b0b0b0;
            font-size: 0.8rem;
        }
    </style>
</head>
<body>
    <h1>Business Idea Generator</h1>
    <div class="idea">Loading...</div>
    <footer>&copy; 2025 Automated Ideas Inc.</footer>

    <script>
        const ideas = [
            "Start a sustainable fashion brand.",
            "Create an AI-powered productivity app.",
            "Develop a meal prep delivery service.",
            "Launch an online thrift store.",
            "Offer virtual reality fitness classes.",
            "Design smart home energy-saving devices.",
            "Start a plant-based snack company.",
            "Develop a language learning AI assistant.",
            "Create eco-friendly packaging solutions.",
            "Offer drone delivery services for small businesses."
        ];

        function generateIdea() {
            const randomIndex = Math.floor(Math.random() * ideas.length);
            document.querySelector('.idea').textContent = ideas[randomIndex];
        }

        setInterval(generateIdea, 1000); // Update every second
        generateIdea(); // Generate the first idea immediately
    </script>
</body>
</html>

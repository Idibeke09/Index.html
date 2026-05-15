<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Random Fun Facts</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 20px;
        }

        .container {
            background: white;
            border-radius: 20px;
            box-shadow: 0 20px 60px rgba(0, 0, 0, 0.3);
            max-width: 600px;
            width: 100%;
            padding: 60px 40px;
            text-align: center;
        }

        h1 {
            color: #333;
            margin-bottom: 30px;
            font-size: 2.5em;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        .fact-box {
            background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
            border-left: 5px solid #667eea;
            padding: 30px;
            margin-bottom: 30px;
            border-radius: 10px;
            min-height: 120px;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .fact-text {
            color: #333;
            font-size: 1.2em;
            line-height: 1.6;
            font-weight: 500;
        }

        button {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            border: none;
            padding: 15px 40px;
            font-size: 1.1em;
            border-radius: 50px;
            cursor: pointer;
            transition: transform 0.2s, box-shadow 0.2s;
            font-weight: bold;
        }

        button:hover {
            transform: translateY(-2px);
            box-shadow: 0 10px 20px rgba(102, 126, 234, 0.4);
        }

        button:active {
            transform: translateY(0);
        }

        .fact-counter {
            color: #999;
            font-size: 0.9em;
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>🎉 Fun Facts</h1>
        <div class="fact-box">
            <p class="fact-text" id="fact">Click the button to get a random fun fact!</p>
        </div>
        <button onclick="getRandomFact()">Get New Fact</button>
        <div class="fact-counter">
            <p id="counter">Fact 0 of 20</p>
        </div>
    </div>

    <script>
        const facts = [
            "Honey never spoils. Archaeologists have found 3,000-year-old honey in Egyptian tombs that was still edible!",
            "A group of flamingos is called a 'flamboyance.'",
            "Octopuses have three hearts: two pump blood to the gills, and one pumps blood to the rest of the body.",
     <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Random Fun Facts</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 20px;
        }

        .container {
            background: white;
            border-radius: 20px;
            box-shadow: 0 20px 60px rgba(0, 0, 0, 0.3);
            max-width: 600px;
            width: 100%;
            padding: 60px 40px;
            text-align: center;
        }

        h1 {
            color: #333;
            margin-bottom: 30px;
            font-size: 2.5em;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        .fact-box {
            background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
            border-left: 5px solid #667eea;
            padding: 30px;
            margin-bottom: 30px;
            border-radius: 10px;
            min-height: 120px;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .fact-text {
            color: #333;
            font-size: 1.2em;
            line-height: 1.6;
            font-weight: 500;
        }

        button {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            border: none;
            padding: 15px 40px;
            font-size: 1.1em;
            border-radius: 50px;
            cursor: pointer;
            transition: transform 0.2s, box-shadow 0.2s;
            font-weight: bold;
        }

        button:hover {
            transform: translateY(-2px);
            box-shadow: 0 10px 20px rgba(102, 126, 234, 0.4);
        }

        button:active {
            transform: translateY(0);
        }

        .fact-counter {
            color: #999;
            font-size: 0.9em;
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>🎉 Fun Facts</h1>
        <div class="fact-box">
            <p class="fact-text" id="fact">Click the button to get a random fun fact!</p>
        </div>
        <button onclick="getRandomFact()">Get New Fact</button>
        <div class="fact-counter">
            <p id="counter">Fact 0 of 20</p>
        </div>
    </div>

    <script>
        const facts = [
            "Honey never spoils. Archaeologists have found 3,000-year-old honey in Egyptian tombs that was still edible!",
            "A group of flamingos is called a 'flamboyance.'",
            "Octopuses have three hearts: two pump blood to the gills, and one pumps blood to the rest of the body.",
            "Bananas are berries, but strawberries aren't. Botanically, bananas are berries but strawberries are aggregate fruits.",
            "The shortest war in history lasted only 38 to 45 minutes between Britain and Zanzibar in 1896.",
            "Honey is the only food that never goes bad. It can last for thousands of years.",
            "A single bolt of lightning contains enough energy to toast 100,000 slices of bread.",
            "Cleopatra lived closer to the invention of the iPhone than to the construction of the Great Pyramid.",
            "The smell of petrichor (rain on dry earth) comes from oils released by plants and a compound produced by soil bacteria.",
            "Slothes only defecate once a week and lose up to 30% of their body weight when they do.",
            "A group of crows is called a 'murder.'",
            "Wombats produce cube-shaped poop to mark their territory.",
            "The fingerprints of koalas are so similar to humans that they've been confused at crime scenes.",
            "Penguins have knees! They're just hidden under their feathers.",
            "Butterflies taste with their feet to find out whether the leaf they sit on is good to lay eggs on.",
            "A group of pandas is called an 'embarrassment.'",
            "The Great Wall of China is not visible from space with the naked eye.",
            "Cats have a third eyelid called a nictitating membrane.",
            "Bees can recognize human faces, and they have better memories than humans.",
            "The unicorn is the national animal of Scotland."
        ];

        let currentFactIndex = 0;

        function getRandomFact() {
            currentFactIndex = Math.floor(Math.random() * facts.length);
            const factElement = document.getElementById('fact');
            const counterElement = document.getElementById('counter');
            
            factElement.textContent = facts[currentFactIndex];
            counterElement.textContent = `Fact ${currentFactIndex + 1} of ${facts.length}`;
        }

        // Show initial fact on page load
        window.addEventListener('load', getRandomFact);
    </script>
</body>
</html>       "Bananas are berries, but strawberries aren't. Botanically, bananas are berries but strawberries are aggregate fruits.",
            "The shortest war in history lasted only 38 to 45 minutes between Britain and Zanzibar in 1896.",
            "Honey is the only food that never goes bad. It can last for thousands of years.",
            "A single bolt of lightning contains enough energy to toast 100,000 slices of bread.",
            "Cleopatra lived closer to the invention of the iPhone than to the construction of the Great Pyramid.",
            "The smell of petrichor (rain on dry earth) comes from oils released by plants and a compound produced by soil bacteria.",
            "Slothes only defecate once a week and lose up to 30% of their body weight when they do.",
            "A group of crows is called a 'murder.'",
            "Wombats produce cube-shaped poop to mark their territory.",
            "The fingerprints of koalas are so similar to humans that they've been confused at crime scenes.",
            "Penguins have knees! They're just hidden under their feathers.",
            "Butterflies taste with their feet to find out whether the leaf they sit on is good to lay eggs on.",
            "A group of pandas is called an 'embarrassment.'",
            "The Great Wall of China is not visible from space with the naked eye.",
            "Cats have a third eyelid called a nictitating membrane.",
            "Bees can recognize human faces, and they have better memories than humans.",
            "The unicorn is the national animal of Scotland."
        ];

        let currentFactIndex = 0;

        function getRandomFact() {
            currentFactIndex = Math.floor(Math.random() * facts.length);
            const factElement = document.getElementById('fact');
            const counterElement = document.getElementById('counter');
            
            factElement.textContent = facts[currentFactIndex];
            counterElement.textContent = `Fact ${currentFactIndex + 1} of ${facts.length}`;
        }

        // Show initial fact on page load
        window.addEventListener('load', getRandomFact);
    </script>
</body>
</html>

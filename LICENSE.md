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
            border-radius: 15px;
            box-shadow: 0 10px 40px rgba(0, 0, 0, 0.2);
            padding: 40px;
            max-width: 600px;
            width: 100%;
            text-align: center;
        }

        h1 {
            color: #333;
            margin-bottom: 30px;
            font-size: 2.5em;
        }

        .fact-box {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 30px;
            border-radius: 10px;
            min-height: 150px;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-bottom: 30px;
            font-size: 1.2em;
            line-height: 1.6;
            box-shadow: 0 5px 15px rgba(102, 126, 234, 0.4);
        }

        .button-group {
            display: flex;
            gap: 15px;
            justify-content: center;
            flex-wrap: wrap;
        }

        button {
            background-color: #667eea;
            color: white;
            border: none;
            padding: 12px 30px;
            border-radius: 25px;
            font-size: 1em;
            cursor: pointer;
            transition: all 0.3s ease;
            font-weight: 600;
        }

        button:hover {
            background-color: #764ba2;
            transform: translateY(-2px);
            box-shadow: 0 5px 15px rgba(102, 126, 234, 0.4);
        }

        button:active {
            transform: translateY(0);
        }

        .reset-btn {
            background-color: #e74c3c;
        }

        .reset-btn:hover {
            background-color: #c0392b;
        }

        .fact-counter {
            color: #666;
            font-size: 0.9em;
            margin-top: 20px;
        }

        @media (max-width: 500px) {
            .container {
                padding: 20px;
            }

            h1 {
                font-size: 1.8em;
            }

            .fact-box {
                min-height: 120px;
                font-size: 1em;
                padding: 20px;
            }

            button {
                padding: 10px 20px;
                font-size: 0.9em;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>🎉 Fun Facts 🎉</h1>
        <div class="fact-box" id="factBox">
            Click the button to discover a fun fact!
        </div>
        <div class="button-group">
            <button onclick="showRandomFact()">Get Random Fact</button>
            <button class="reset-btn" onclick="resetFacts()">Reset</button>
        </div>
        <div class="fact-counter" id="counter"></div>
    </div>

    <script>
        const facts = [
            "Honey never spoils! Archaeologists have found 3000-year-old honey in Egyptian tombs that was still edible.",
            "A group of flamingos is called a 'flamboyance'.",
            "Octopuses have three hearts and blue blood.",
            "Bananas are berries, but strawberries are not!",
            "A single lightning bolt is about 5 times hotter than the surface of the sun.",
            "Dolphins have names for each other and call out to friends by name.",
            "The shortest war in history lasted only 38 minutes.",
            "Cats have over 20 different vocal sounds to communicate.",
            "A day on Venus is longer than a year on Venus.",
            "Scotland's national animal is a unicorn.",
            "Peanuts aren't actually nuts, they're legumes.",
            "A group of owls is called a 'parliament'.",
            "The fingerprints of koalas are so similar to humans that they can confuse crime scene investigators.",
            "Sloths only poop once a week.",
            "A group of crows is called a 'murder'.",
            "Carrots weren't originally orange; they were purple.",
            "Butterflies taste with their feet.",
            "The sound of a whip cracking is actually a sonic boom.",
            "Wombats have cube-shaped poop.",
            "A group of hedgehogs is called a 'prickle'.",
            "Tardigrades (water bears) can survive in space.",
            "The tongue of a chameleon is longer than its body.",
            "Penguins propose to their mates with pebbles.",
            "An albatross can sleep while flying.",
            "Otters hold hands while sleeping so they don't drift apart."
        ];

        let factsShown = [];

        function showRandomFact() {
            let randomIndex;
            
            // If all facts have been shown, reset the list
            if (factsShown.length === facts.length) {
                factsShown = [];
            }

            // Get a random fact that hasn't been shown yet
            do {
                randomIndex = Math.floor(Math.random() * facts.length);
            } while (factsShown.includes(randomIndex));

            factsShown.push(randomIndex);
            document.getElementById('factBox').textContent = facts[randomIndex];
            updateCounter();
        }

        function resetFacts() {
            factsShown = [];
            document.getElementById('factBox').textContent = 'Click the button to discover a fun fact!';
            document.getElementById('counter').textContent = '';
        }

        function updateCounter() {
            const totalFacts = facts.length;
            const remaining = totalFacts - factsShown.length;
            document.getElementById('counter').textContent = `Facts discovered: ${factsShown.length} / ${totalFacts} (${remaining} remaining)`;
        }

        // Load initial fact on page load
        window.onload = function() {
            showRandomFact();
        };
    </script>
</body>
</html>

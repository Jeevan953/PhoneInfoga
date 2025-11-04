<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy Christmas Greeting</title>
    <!-- Load Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Load a festive Google Font (Mountains of Christmas) -->
    <link href="https://fonts.googleapis.com/css2?family=Mountains+of+Christmas:wght@400;700&display=swap" rel="stylesheet">
    <style>
        /* Define the festive font */
        .font-christmas {
            font-family: 'Mountains of Christmas', cursive;
        }

        /* Keyframe animation for the falling glitter/snow */
        @keyframes fallAndTwinkle {
            0% {
                transform: translate(0, -100px) rotate(0deg);
                opacity: 0;
            }
            50% {
                opacity: 1;
                transform: translate(0, 50vh) rotate(180deg) scale(1.1);
            }
            100% {
                transform: translate(0, 110vh) rotate(360deg);
                opacity: 0;
            }
        }

        /* Style for individual glitter pieces */
        .glitter {
            position: absolute;
            width: 8px;
            height: 8px;
            border-radius: 50%;
            pointer-events: none;
            z-index: 10;
            animation-name: fallAndTwinkle;
            animation-iteration-count: infinite;
            filter: drop-shadow(0 0 4px rgba(255, 255, 255, 0.8));
        }
    </style>
    <script>
        // JavaScript to generate and animate the glitter pieces
        document.addEventListener('DOMContentLoaded', () => {
            const glitterContainer = document.getElementById('glitter-container');
            const numberOfGlitter = 150; // Total number of particles
            const colors = ['bg-yellow-300', 'bg-red-500', 'bg-green-400', 'bg-white', 'bg-sky-300'];

            for (let i = 0; i < numberOfGlitter; i++) {
                const glitter = document.createElement('div');

                // Apply base styles and a random color
                const randomColor = colors[Math.floor(Math.random() * colors.length)];
                glitter.className = `glitter ${randomColor}`;

                // Set random starting position (X-axis)
                glitter.style.left = `${Math.random() * 100}vw`;
                
                // Set random animation duration (speed) and delay (start time)
                const duration = 8 + Math.random() * 8; // 8s to 16s
                const delay = -Math.random() * 16; // Start off-screen at random times

                glitter.style.animationDuration = `${duration}s`;
                glitter.style.animationDelay = `${delay}s`;

                // Set random size (for variety)
                const size = 5 + Math.random() * 5; // 5px to 10px
                glitter.style.width = `${size}px`;
                glitter.style.height = `${size}px`;
                
                // Randomize shape (some squares, mostly circles)
                if (Math.random() > 0.6) {
                    glitter.style.borderRadius = '0'; // Square/Confetti
                    glitter.style.transform = `rotate(${Math.random() * 90}deg)`;
                } else {
                    glitter.style.borderRadius = '50%'; // Circle/Glitter
                }

                glitterContainer.appendChild(glitter);
            }
        });
    </script>
</head>
<body class="bg-indigo-900 min-h-screen flex items-center justify-center overflow-hidden">

    <!-- Glitter Container (must be sibling to main content for z-index control) -->
    <div id="glitter-container" class="absolute inset-0 w-full h-full"></div>

    <!-- Main Greeting Card Content -->
    <div class="relative z-20 p-8 sm:p-12 md:p-16 text-center bg-white/10 backdrop-blur-sm rounded-3xl shadow-2xl border border-white/30 max-w-lg mx-4 transition-all duration-300">
        <!-- Optional Icon -->
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor" class="w-16 h-16 mx-auto mb-6 text-yellow-300 drop-shadow-lg">
            <path fill-rule="evenodd" d="M12 2.25l-4.5 9h9l-4.5-9zm0 0l-4.5 9h9l-4.5-9zm0 0l-4.5 9h9l-4.5-9zM4.5 21.75h15c.828 0 1.5-.672 1.5-1.5s-.672-1.5-1.5-1.5h-15c-.828 0-1.5.672-1.5 1.5s.672 1.5 1.5 1.5zm1.5-1.5h12v-1.5h-12v1.5zM12 18h-.008v.008H12V18zM12 18h.008v.008H12V18z" clip-rule="evenodd" />
            <path fill-rule="evenodd" d="M12 10.5h.008v.008H12V10.5z" clip-rule="evenodd" />
            <path d="M12 12a.75.75 0 0 1 .75-.75h.008a.75.75 0 0 1 0 1.5H12a.75.75 0 0 1-.75-.75z" />
            <path d="M12 15a.75.75 0 0 1 .75-.75h.008a.75.75 0 0 1 0 1.5H12a.75.75 0 0 1-.75-.75z" />
            <path d="M12 18a.75.75 0 0 1 .75-.75h.008a.75.75 0 0 1 0 1.5H12a.75.75 0 0 1-.75-.75z" />
        </svg>

        <h1 class="font-christmas text-6xl sm:text-7xl font-bold text-red-400 mb-4 tracking-wider drop-shadow-lg transition-all duration-300">
            Merry Christmas!
        </h1>
        <p class="font-christmas text-3xl sm:text-4xl text-green-300 mb-8 drop-shadow-md transition-all duration-300">
            Joy and Peace to You
        </p>
        <p class="text-white/80 text-lg sm:text-xl leading-relaxed">
            Wishing you a season filled with sparkle, warmth, and wonderful memories. May your holidays be bright and beautiful!
        </p>
    </div>

</body>
</html>

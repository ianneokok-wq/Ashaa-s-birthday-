
‎    <title>Ashaa's Girly Website</title>
‎    <link href="https://fonts.googleapis.com/css2?family=Dancing+Script:wght@400;700&display=swap" rel="stylesheet">‎ 
<style>
body {
‎            font-family: 'Dancing Script', cursive; /* Added girly cursive font */
‎            background: linear-gradient(to bottom, #ffb3ba, #ffdfba);
‎            color: #ff1493; /* Changed text color to a deeper pink */
‎            margin: 0;
‎            padding: 0;
‎            overflow-x: hidden;
‎            text-align: center;
‎        }
‎        h1 {
‎            font-size: 3em;
‎            color: #ff69b4;
‎            margin-top: 50px;
‎            text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
‎        }
  .container {
‎            max-width: 800px;
‎            margin: 0 auto;
‎            padding: 20px;
‎        }
‎        .pictures {
‎            display: flex;
‎            flex-wrap: wrap;
‎            justify-content: center;
‎            gap: 20px;
‎            margin-top: 50px;
‎        }
‎        .picture-container {
‎            text-align: center;
‎        }
‎        .picture {
‎            width: 150px;
‎            height: 150px;
‎            border-radius: 20px; /* Curved edges */
‎            overflow: hidden;
‎            cursor: pointer;
‎            transition: transform 0.3s;
‎            box-shadow: 0 4px 8px rgba(0,0,0,0.2);
‎            border: none; /* No edges/borders */
‎        }
‎        .picture:hover {
‎            transform: scale(1.1);
‎        }
‎        .picture img {
‎            width: 100%;
‎            height: 100%;
‎            object-fit: cover;
‎        }
‎        .picture-title {
‎            margin-top: 10px;
‎            font-size: 1.2em;
‎            color: #ff69b4;
‎            text-shadow: 1px 1px 2px rgba(0,0,0,0.2);
‎        }
‎        /* Cake section */
‎        .cake-section {
‎            margin-top: 50px;
‎        }
‎        .cake {
‎            position: relative;
‎            width: 200px;
‎            height: 150px;
‎            margin: 0 auto;
‎            background: url('https://via.placeholder.com/200x150/e6b3c3/ffffff?text=Cake') no-repeat center;
‎            background-size: cover;
‎            border-radius: 10px;
‎        }
‎        .blow-button {
‎            margin-top: 20px;
‎            padding: 10px 20px;
‎            background: #ff69b4;
‎            color: #fff;
‎            border: none;
‎            border-radius: 5px;
‎            cursor: pointer;
‎            font-family: 'Dancing Script', cursive;
‎            font-size: 1.2em;
‎            transition: background 0.3s;
‎        }
‎        .blow-button:hover {
‎            background: #ff1493;
‎        }
‎        /* Snowflakes Animation */
‎        .snowflake {
‎            position: absolute;
‎            top: -10px;
‎            color: #fff;
‎            font-size: 20px;
‎            animation: fall linear infinite;
‎            pointer-events: none;
‎        }
‎        @keyframes fall {
‎            to {
‎                transform: translateY(100vh);
‎            }
‎        }
‎        /* Modal for messages */
‎        .modal {
‎            display: none;
‎            position: fixed;
‎            z-index: 1;
‎            left: 0;
‎            top: 0;
‎            width: 100%;
‎            height: 100%;
‎            background-color: rgba(0,0,0,0.5);
‎            justify-content: center;
‎            align-items: center;
‎        }
‎        .modal-content {
‎            background-color: #fff;
‎            padding: 20px;
‎            border-radius: 10px;
‎            text-align: center;
‎            max-width: 400px;
‎            width: 80%;
‎            color: #ff1493; /* Pink text in modal */
‎            animation: fadeIn 2s ease-in-out; /* Slow fade-in animation */
‎        }
‎        @keyframes fadeIn {
‎            from { opacity: 0; transform: scale(0.8); }
‎            to { opacity: 1; transform: scale(1); }
‎        }
‎        .close {
‎            color: #aaa;
‎            float: right;
‎            font-size: 28px;
‎            font-weight: bold;
‎            cursor: pointer;
‎        }
‎        .close:hover {
‎            color: #000;
‎        }
‎        /* Password section */
‎        .password-section {
‎            position: fixed;
‎            top: 0;
‎            left: 0;
‎            width: 100%;
‎            height: 100%;
‎            background: rgba(255, 179, 186, 0.9);
‎            display: flex;
‎            justify-content: center;
‎            align-items: center;
‎            z-index: 1000;
‎        }
‎        .password-form {
‎            background: #fff;
‎            padding: 20px;
‎            border-radius: 10px;
‎            box-shadow: 0 4px 8px rgba(0,0,0,0.2);
‎        }
‎        .password-form h2 {
‎            color: #ff69b4; /* Pink heading in password form */
‎        }
‎        .password-form input {
‎            padding: 10px;
‎            margin: 10px 0;
‎            border: 1px solid #ccc;
‎            border-radius: 5px;
‎        }
‎        .password-form button {
‎            padding: 10px 20px;
‎            background: #ff69b4;
‎            color: #fff;
‎            border: none;
‎            border-radius: 5px;
‎            cursor: pointer;
‎        }
‎        .password-form button:hover {
‎            background: #ff1493;
‎        }
‎        .hidden {
‎            display: none;
‎        }
‎        /* Birthday modal - no card, just text */
‎        .birthday-modal {
‎            display: none;
‎            position: fixed;
‎            z-index: 1001;
‎            left: 0;
‎            top: 0;
‎            width: 100%;
‎            height: 100%;
‎            justify-content: center;
‎            align-items: center;
‎        }
‎        .birthday-text {
‎            font-size: 3em;
‎            color: #ff69b4;
‎            text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
‎            animation: fadeIn 3s ease-in-out; /* Slow pop-up animation */
‎        }
‎    </style>
‎</head>
‎<body>
‎    <div id="passwordSection" class="password-section">
‎        <div class="password-form">
‎            <h2>Enter Password to Access Ashaa's World</h2>
‎            <input type="password" id="passwordInput" placeholder="Password">
‎            <button onclick="checkPassword()">Enter</button>
‎        </div>
‎    </div>
‎
‎    <!-- Birthday Modal - just text -->
‎    <div id="birthdayModal" class="birthday-modal">
‎        <p class="birthday-text">Happy Birthday Ashaa!! 🎉</p>
‎    </div>
‎
‎    <!-- Audio element for music -->
‎    <audio id="birthdayMusic" preload="auto">
‎        <source src="birthday.mp3" type="audio/wav"> <!-- Placeholder music URL; replace with actual birthday music -->
‎        Your browser does not support the audio element.
‎    </audio>
‎
‎    <div id="mainContent" class="hidden">
‎        <h1>Welcome to Ashaa's World!</h1>
‎        <div class="container">
‎            <p>Click on the pictures below to see some special messages for Ashaa!</p>
‎            <div class="pictures">
‎                <div class="picture-container">
‎                    <div class="picture" onclick="showMessage('  Happy birthday ashaa, thank you for coming into my life!! Be happy always thanks for your comfort when i get low, thanks a lot ashaa!! Choose to be happy always okay?, youre my legend!')">
‎                        <img src="ashaa.jpg" alt="Star">
‎                    </div>
‎                    <p class="picture-title">Gorgeous</p>
‎                </div>
‎                <div class="picture-container">
‎                    <div class="picture" onclick="showMessage('My dearest Ashaa, on your special day, my heart overflows with love for you. Every moment with you feels like a beautiful sunrise, and I cherish the way you light up my world. Happy Birthday—may this year bring us even closer, wrapped in endless affection and sweet memories.')">
‎                        <img src="hehe.jpg" alt="Sunrise">
‎                    </div>
‎                    <p class="picture-title">Cute</p>
‎                </div>
‎                <div class="picture-container">
‎                    <div class="picture" onclick="showMessage('Happy Birthday, Ashaa. As you blow out the candles, remember how far you\'ve come and the joy you\'ve brought to those around you. You\'re a beacon of kindness and strength—here\'s to another year of growth, laughter, and cherished moments. Wishing you all the happiness your heart can hold.')">
‎                        <img src="cute.jpg" alt="Cotton Candy">
‎                    </div>
‎                    <p class="picture-title">Lovely</p>
‎                </div>
‎                <div class="picture-container">
‎                    <div class="picture" onclick="showMessage('Oh, wow, another year older? Congrats on surviving this long—most people give up after the first decade. Happy Birthday! May your presents be as underwhelming as your sense of humor, and your cake be the only thing that doesn\'t disappoint. Kidding, you\'re awesome... mostly.')">
‎                        <img src="ganda.jpg" alt="Diamonds">
‎                    </div>
‎                    <p class="picture-title">Ganda</p>
‎                </div>
‎                <div class="picture-container">
‎                    <div class="picture" onclick="showMessage('In the garden of time, a flower blooms anew, On this day of your birth, my wishes for you: Petals of joy, roots of strength deep and true, May laughter dance like leaves in the dew. Happy Birthday, Ashaa—a verse of love, pure and bright!')">
‎                        <img src="crush.jpg" alt="Heart">
‎                    </div>
‎                    <p class="picture-title">Itu sangat indah </p>
‎                </div>
‎            </div>
‎
‎            <!-- Cake Section -->
‎            <div class="cake-section">
‎                <div class="cake">
‎                </div>
‎                <button class="blow-button" onclick="showCakeMessage()">my message for you</button>
‎            </div>
‎        </div>
‎
‎        <!-- Modal -->
‎        <div id="messageModal" class="modal">
‎            <div class="modal-content">
‎                <span class="close" onclick="closeModal()">&times;</span>
‎                <p id="modalText"></p>
‎            </div>
‎        </div>
‎    </div>
‎
 <script>
‎        // Function to check password
‎        function checkPassword() {
‎            const password = document.getElementById('passwordInput').value;
‎            if (password === 'Cutiee ashaa') { // Change this to your desired password
‎                document.getElementById('passwordSection').style.display = 'none';
‎                // Play music
‎                const music = document.getElementById('birthdayMusic');
‎                music.play().catch(e => console.log('Audio play failed:', e)); // Handle autoplay restrictions
‎                // Show birthday modal slowly
‎                document.getElementById('birthdayModal').style.display = 'flex';
‎                // After 4 seconds, hide birthday modal and show main content
‎                setTimeout(() => {
‎                    document.getElementById('birthdayModal').style.display = 'none';
‎                    document.getElementById('mainContent').classList.remove('hidden');
‎                }, 4000);
‎            } else {
‎                alert('Incorrect password. Try again!');
‎            }
‎        }
‎
‎        // Function to show cake message (new function for clicking the cake)
‎        function showCakeMessage() {
‎            document.getElementById('modalText').innerText = 'Hi ashaa!! Its your birthday, sorry for the inconvenience, I dont know what to say to you but i will say sorry first because i failed as I was waiting for you, sometimes i think that myself is the problem, i know youre the best and good girl that i ever met and i love that so much, to be honest i miss you, i miss you so much ashaa but I cant do anything Im stupid, selfish and not lovable, i will not be dramatic HEHEHEHEH sorry for the times i made a mistake, enjoy your day!! And happy birthday again!! Mwahhh!! 🎂😘';
‎            document.getElementById('messageModal').style.display = 'flex';
‎        }
‎
‎        // Function to show modal with message
‎        function showMessage(message) {
‎            document.getElementById('modalText').innerText = message;
‎            document.getElementById('messageModal').style.display = 'flex';
‎        }
‎
‎        // Function to close modal
‎        function closeModal() {
‎            document.getElementById('messageModal').style.display = 'none';
‎        }
‎
‎        // Generate falling snowflakes
‎        function createSnowflake() {
‎            const snowflake = document.createElement('div');
‎            snowflake.className = 'snowflake';
‎            snowflake.innerHTML = '❄🎂'; // Snow emoji
‎            snowflake.style.left = Math.random() * 100 + 'vw';
‎            snowflake.style.animationDuration = Math.random() * 3 + 2 + 's'; // Random speed
‎            document.body.appendChild(snowflake);
‎
‎            // Remove after animation
‎            setTimeout(() => {
‎                snowflake.remove();
‎            }, 5000);
‎        }
‎
‎        // Create snowflakes every 300ms
‎        setInterval(createSnowflake, 300);
‎    </script>
‎</body>
‎

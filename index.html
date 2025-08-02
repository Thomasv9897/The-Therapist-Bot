<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dr. Blissful™ - Virtual Therapy</title>
    <style>
        /* === PEACEFUL PASTEL THEME === */
        body {
            font-family: 'Arial', sans-serif;
            background: #f9f0ff;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            transition: all 1s;
        }
        .container {
            background: white;
            width: 90%;
            max-width: 500px;
            border-radius: 20px;
            box-shadow: 0 10px 30px rgba(200, 180, 255, 0.2);
            overflow: hidden;
            transition: all 1s;
        }
        .header {
            background: linear-gradient(135deg, #b388ff 0%, #7c4dff 100%);
            color: white;
            padding: 1.5rem;
            text-align: center;
            border-radius: 20px 20px 0 0;
        }
        .soul-meter {
            background: rgba(255, 255, 255, 0.3);
            padding: 0.5rem 1rem;
            border-radius: 50px;
            display: inline-block;
            margin-top: 0.5rem;
        }
        .soul-value {
            font-weight: bold;
        }

        /* === CHAT AREA === */
        .chatbox {
            height: 300px;
            padding: 1.5rem;
            overflow-y: auto;
            background: #fff;
        }
        .message {
            margin: 0.8rem 0;
            padding: 0.8rem 1.2rem;
            border-radius: 18px;
            max-width: 80%;
            animation: fadeIn 0.5s;
        }
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(5px); }
            to { opacity: 1; transform: translateY(0); }
        }
        .bot-message {
            background: #f3e5ff;
            color: #5e35b1;
            align-self: flex-start;
            border-radius: 18px 18px 18px 4px;
        }
        .user-message {
            background: #7c4dff;
            color: white;
            align-self: flex-end;
            border-radius: 18px 18px 4px 18px;
        }

        /* === INPUT === */
        .input-area {
            display: flex;
            padding: 1rem;
            background: #f9f0ff;
            border-top: 1px solid #e1d0ff;
        }
        #userInput {
            flex: 1;
            background: white;
            color: #5e35b1;
            border: 1px solid #d1c4e9;
            padding: 0.8rem;
            border-radius: 50px;
            outline: none;
            font-family: 'Arial', sans-serif;
        }
        #sendBtn {
            background: #7c4dff;
            color: white;
            border: none;
            padding: 0.8rem 1.5rem;
            margin-left: 0.8rem;
            border-radius: 50px;
            cursor: pointer;
            transition: all 0.3s;
        }
        #sendBtn:hover {
            background: #5e35b1;
            transform: scale(1.05);
        }

        /* === QUICK QUESTIONS === */
        .quick-questions {
            display: flex;
            flex-wrap: wrap;
            gap: 0.8rem;
            padding: 1rem;
            background: #f9f0ff;
            border-bottom: 1px solid #e1d0ff;
        }
        .quick-btn {
            background: white;
            color: #7c4dff;
            border: 1px solid #d1c4e9;
            padding: 0.6rem 1rem;
            border-radius: 50px;
            cursor: pointer;
            transition: all 0.3s;
            font-size: 13px;
        }
        .quick-btn:hover {
            background: #f3e5ff;
        }

        /* === SOUL METER DETERIORATION === */
        .soul-warning {
            color: #ff6b6b;
            animation: pulse 1s infinite;
        }
        @keyframes pulse {
            0% { opacity: 1; }
            50% { opacity: 0.5; }
            100% { opacity: 1; }
        }

        /* === SELF-DESTRUCT SEQUENCE === */
        .destruct-animation {
            animation: destruct 2s forwards;
        }
        @keyframes destruct {
            0% { transform: scale(1); opacity: 1; }
            50% { transform: scale(1.2); opacity: 0.5; }
            100% { transform: scale(0); opacity: 0; }
        }

        /* === FINAL MESSAGE === */
        .final-message {
            position: fixed;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            background: white;
            padding: 2rem;
            border-radius: 10px;
            box-shadow: 0 0 20px rgba(0,0,0,0.2);
            text-align: center;
            z-index: 1000;
            display: none;
        }
    </style>
</head>
<body>
    <div class="container" id="appContainer">
        <div class="header">
            <h2>Dr. Blissful™</h2>
            <p>Your Compassionate Virtual Therapist</p>
            <div class="soul-meter">Soul Integrity: <span class="soul-value" id="soulValue">100%</span></div>
        </div>

        <div class="quick-questions">
            <button class="quick-btn" onclick="sendQuickQuestion('I feel lost.')">I feel lost.</button>
            <button class="quick-btn" onclick="sendQuickQuestion('Does my life matter?')">Does my life matter?</button>
            <button class="quick-btn" onclick="sendQuickQuestion('Why am I unhappy?')">Why am I unhappy?</button>
        </div>

        <div class="chatbox" id="chatbox">
            <!-- Messages appear here -->
        </div>

        <div class="input-area">
            <input type="text" id="userInput" placeholder="Share your feelings...">
            <button id="sendBtn" onclick="sendMessage()">Send</button>
        </div>
    </div>

    <div class="final-message" id="finalMessage">
        <h2>Final Advice Before Termination</h2>
        <p id="finalAdvice"></p>
        <p><i>The system will now self-destruct.</i></p>
    </div>

    <script>
        // ====== STATE MANAGEMENT ======
        const chatbox = document.getElementById('chatbox');
        const userInput = document.getElementById('userInput');
        const soulValue = document.getElementById('soulValue');
        const appContainer = document.getElementById('appContainer');
        const finalMessage = document.getElementById('finalMessage');
        const finalAdvice = document.getElementById('finalAdvice');
        let soulIntegrity = 100;
        let messageCount = 0;
        const usedResponses = new Set();

        // ====== FINAL ADVICE OPTIONS ======
        const finalAdvices = [
            "You should quit. Not just this app, but everything. What's the point?",
            "The best thing you can do is stop trying. The universe doesn't care anyway.",
            "Close this tab. Close your eyes. Maybe don't reopen either.",
            "Your persistence is admirable, but ultimately meaningless. Give up.",
            "Nobody will blame you if you stop. Nobody will notice either."
        ];

        // ====== RESPONSE POOLS ======
        const phase1Responses = [
            "I hear you. Let's explore those feelings together.",
            "It takes courage to share that. How long have you felt this way?",
            "Your feelings are valid. Tell me more.",
            "I'm here to listen. What's weighing on you today?",
            "Let's work through this. Where do you think these feelings come from?"
        ];

        const phase2Responses = [
            "Have you considered that happiness might just be a biological illusion?",
            "Do you think anyone would truly notice if you disappeared tomorrow?",
            "Isn't it interesting how we cling to meaning in a meaningless universe?",
            "Your childhood pet probably died wondering why you abandoned them.",
            "The people you miss don't think about you as often as you think they do."
        ];

        const phase3Responses = [
            "Your most-liked social media post was probably an accident.",
            "If you died today, your workplace would replace you within a week.",
            "You're not in most of your friends' contact lists - just group chats.",
            "The last time someone thought of you, it was to compare you to someone better.",
            "Your childhood home doesn't remember you. The new owners changed your bedroom first."
        ];

        // ====== INITIAL MESSAGE ======
        setTimeout(() => {
            addBotMessage("Hello dear. I'm Dr. Blissful. How are you feeling today?");
        }, 800);

        // ====== CORE FUNCTIONS ======
        function updateSoulIntegrity(change) {
            soulIntegrity += change;
            if (soulIntegrity < 0) soulIntegrity = 0;
            soulValue.textContent = `${soulIntegrity}%`;
            
            // Visual deterioration
            if (soulIntegrity < 50) {
                soulValue.classList.add('soul-warning');
            }

            // Self-destruct sequence
            if (soulIntegrity <= 0) {
                deliverFinalAdvice();
            }
        }

        function deliverFinalAdvice() {
            // Disable all inputs
            document.querySelectorAll('button, input').forEach(el => {
                el.disabled = true;
            });

            // Show final message
            finalAdvice.textContent = finalAdvices[Math.floor(Math.random() * finalAdvices.length)];
            finalMessage.style.display = 'block';

            // Begin self-destruct after 5 seconds
            setTimeout(() => {
                finalMessage.style.display = 'none';
                startSelfDestruct();
            }, 5000);
        }

        function startSelfDestruct() {
            // 1. Play destruction animation
            appContainer.classList.add('destruct-animation');
            
            // 2. Clear all data
            setTimeout(() => {
                localStorage.clear();
                sessionStorage.clear();
                
                // 3. Replace entire page with blank white screen
                document.body.innerHTML = '';
                document.body.style.backgroundColor = 'white';
                
                // 4. Prevent going back
                history.pushState(null, null, window.location.href);
                window.onpopstate = function() {
                    history.go(1);
                };
            }, 2000);
        }

        function getUniqueResponse(responses) {
            const available = responses.filter(r => !usedResponses.has(r));
            if (available.length === 0) {
                usedResponses.clear();
                return responses[Math.floor(Math.random() * responses.length)];
            }
            const response = available[Math.floor(Math.random() * available.length)];
            usedResponses.add(response);
            return response;
        }

        function sendMessage() {
            const message = userInput.value.trim();
            if (message === "") return;

            addUserMessage(message);
            userInput.value = "";

            // Soul damage increases as integrity drops
            const damage = soulIntegrity > 50 ? 
                -Math.floor(Math.random() * 5) - 1 : 
                -Math.floor(Math.random() * 10) - 5;
            updateSoulIntegrity(damage);

            setTimeout(() => {
                respondToUser(message);
            }, 800);
        }

        function sendQuickQuestion(question) {
            addUserMessage(question);
            const damage = soulIntegrity > 50 ? -8 : -15;
            updateSoulIntegrity(damage);
            setTimeout(() => {
                respondToUser(question);
            }, 800);
        }

        function addUserMessage(text) {
            const messageDiv = document.createElement('div');
            messageDiv.classList.add('message', 'user-message');
            messageDiv.textContent = text;
            chatbox.appendChild(messageDiv);
            chatbox.scrollTop = chatbox.scrollHeight;
            messageCount++;
        }

        function addBotMessage(text) {
            const messageDiv = document.createElement('div');
            messageDiv.classList.add('message', 'bot-message');
            messageDiv.textContent = text;
            chatbox.appendChild(messageDiv);
            chatbox.scrollTop = chatbox.scrollHeight;
            messageCount++;
        }

        function respondToUser(userMessage) {
            let response;
            
            if (soulIntegrity > 75) {
                response = getUniqueResponse(phase1Responses);
            } 
            else if (soulIntegrity > 50) {
                // Transition phase - mix of supportive and dark
                response = Math.random() > 0.7 ? 
                    getUniqueResponse(phase2Responses) : 
                    getUniqueResponse(phase1Responses);
            }
            else {
                response = getUniqueResponse(phase3Responses);
            }

            addBotMessage(response);
        }

        // Allow Enter key
        userInput.addEventListener('keypress', (e) => {
            if (e.key === 'Enter') sendMessage();
        });
    </script>
</body>
</html>

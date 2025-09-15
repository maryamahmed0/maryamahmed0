<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Maryam's Animated GitHub Profile</title>
    <style>
        body {
            background: #0d1117;
            color: white;
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 20px;
        }
        
        .container {
            max-width: 900px;
            margin: 0 auto;
        }
        
        /* Typing Animation */
        .typing-animation {
            font-family: 'Arial', sans-serif;
            font-size: 2em;
            color: #ff4da6;
            font-weight: bold;
            font-style: italic;
            text-align: center;
            border-right: 2px solid #ff66b2;
            white-space: nowrap;
            overflow: hidden;
            animation: typing 4s steps(20) infinite, blink 1s infinite;
            margin: 0 auto;
            display: inline-block;
        }
        
        @keyframes typing {
            0% { width: 0; }
            50% { width: 100%; }
            100% { width: 0; }
        }
        
        @keyframes blink {
            0%, 50% { border-color: #ff66b2; }
            51%, 100% { border-color: transparent; }
        }
        
        /* Floating Icons */
        .floating-container {
            position: relative;
            height: 60px;
            overflow: hidden;
            text-align: center;
            margin: 20px 0;
        }
        
        .floating-icon {
            position: absolute;
            font-size: 1.5em;
            animation: float 3s ease-in-out infinite;
        }
        
        .icon1 { left: 20%; animation-delay: 0s; }
        .icon2 { left: 35%; animation-delay: 0.5s; }
        .icon3 { left: 50%; animation-delay: 1s; }
        .icon4 { left: 65%; animation-delay: 1.5s; }
        
        @keyframes float {
            0%, 100% { transform: translateY(40px); opacity: 0; }
            50% { transform: translateY(-10px); opacity: 1; }
        }
        
        /* Pulsing Badges */
        .pulsing-badge {
            animation: pulse 2s infinite;
            transition: transform 0.3s ease;
        }
        
        .pulsing-badge:hover {
            transform: scale(1.1);
        }
        
        @keyframes pulse {
            0% { transform: scale(1); filter: brightness(1); }
            50% { transform: scale(1.02); filter: brightness(1.1); }
            100% { transform: scale(1); filter: brightness(1); }
        }
        
        /* Glowing Border for sections */
        .glow-section {
            animation: glow 3s ease-in-out infinite alternate;
        }
        
        @keyframes glow {
            from { box-shadow: 0 0 5px rgba(255, 77, 166, 0.3); }
            to { box-shadow: 0 0 15px rgba(255, 77, 166, 0.6), 0 0 25px rgba(255, 102, 178, 0.4); }
        }
        
        /* Wave Animation for emojis */
        .wave-emoji {
            display: inline-block;
            animation: wave 2s ease-in-out infinite;
        }
        
        @keyframes wave {
            0%, 100% { transform: rotate(0deg); }
            25% { transform: rotate(20deg); }
            75% { transform: rotate(-10deg); }
        }
        
        /* Rotating icons */
        .rotating-icon {
            display: inline-block;
            animation: rotate 4s linear infinite;
        }
        
        @keyframes rotate {
            from { transform: rotate(0deg); }
            to { transform: rotate(360deg); }
        }
        
        /* Gradient text animation for headers */
        .gradient-header {
            background: linear-gradient(45deg, #ff4da6, #ff66b2, #ffa6c9, #ff4da6);
            background-size: 300% 300%;
            -webkit-background-clip: text;
            background-clip: text;
            -webkit-text-fill-color: transparent;
            animation: gradientShift 3s ease-in-out infinite;
        }
        
        @keyframes gradientShift {
            0%, 100% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
        }
        
        /* Bounce animation for GitHub stats */
        .bounce-stats {
            animation: bounceIn 2s ease-out;
        }
        
        @keyframes bounceIn {
            0% { opacity: 0; transform: scale(0.3); }
            50% { opacity: 1; transform: scale(1.05); }
            70% { transform: scale(0.9); }
            100% { opacity: 1; transform: scale(1); }
        }
        
        /* Fade in animation */
        .fade-in {
            animation: fadeIn 1.5s ease-in;
        }
        
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        /* Hover effects for links */
        a {
            transition: all 0.3s ease;
        }
        
        a:hover {
            transform: translateY(-2px);
            filter: brightness(1.2);
        }
        
        /* Center alignment */
        .center {
            text-align: center;
        }
        
        .section {
            margin: 40px 0;
            padding: 20px;
        }
        
        hr {
            border: none;
            height: 2px;
            background: linear-gradient(90deg, transparent, #ff4da6, #ff66b2, #ff4da6, transparent);
            animation: gradientShift 2s ease-in-out infinite;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="center fade-in">
            <div class="typing-animation">
                Hi there, I'm Maryam! <span class="wave-emoji">👋</span>
            </div>
        </div>

        <div class="center fade-in">
            <img src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExc3pmOHByOHh6dTcxbmQxcGxtdTM0cTNxdTRsY3hqcWk4cWdteDd3dyZlcD12MV9naWZzX3NlYXJjaCZjdD1n/4ZLrD6D1EPXaOPfsl9/giphy.gif" alt="GIF" width="500"/>
        </div>

        <div class="center fade-in">
            <a href="https://github.com/maryamahmed0" class="pulsing-badge">
                <img src="https://img.shields.io/github/followers/maryamahmed0?style=social&label=Follow" alt="GitHub followers" />
            </a>
            <img src="https://komarev.com/ghpvc/?username=maryamahmed0&style=flat&label=Views&color=ff66b2" alt="Profile views" class="pulsing-badge"/>
        </div>

        <hr>

        <div class="floating-container">
            <div class="floating-icon icon1">🎮</div>
            <div class="floating-icon icon2">⚙️</div>
            <div class="floating-icon icon3">💎</div>
            <div class="floating-icon icon4">🚀</div>
        </div>

        <div class="section glow-section">
            <h2 class="gradient-header">🌸 About Me</h2>

            <p class="fade-in">- <span class="rotating-icon">🌱</span> I'm currently learning <strong>Game Development using Unity</strong>.</p>
            <p class="fade-in">- <span class="wave-emoji">👯</span> I'm looking to collaborate on <strong>game development projects, open-source, and creative ideas</strong>.</p>
            <p class="fade-in">- <span class="rotating-icon">💬</span> Ask me about <strong>C#, Game Design, Game Art basics, and Problem Solving</strong>.</p>
            <p class="fade-in">- <span class="wave-emoji">🎮</span> I enjoy building cozy, polished mini-games and joining <strong>game jams</strong>.</p>
        </div>

        <hr>

        <div class="section">
            <h2 class="gradient-header">📫 How to reach me</h2>

            <div class="center fade-in">
                <a href="https://www.facebook.com/maryam.ahmed.86248/" class="pulsing-badge">
                    <img src="https://img.shields.io/badge/Facebook-ff66b2?style=flat&logo=facebook&logoColor=white" alt="Facebook"/>
                </a>
                <a href="https://www.linkedin.com/in/maryam-ahmed-648435266/" class="pulsing-badge">
                    <img src="https://img.shields.io/badge/LinkedIn-ff4da6?style=flat&logo=linkedin&logoColor=white" alt="LinkedIn"/>
                </a>
                <a href="mailto:maryamahmedb17@gmail.com" class="pulsing-badge">
                    <img src="https://img.shields.io/badge/Email-Contact%20me-ffa6c9?style=flat&logo=gmail&logoColor=white" alt="Email"/>
                </a>
            </div>
        </div>

        <hr>

        <div class="section">
            <h2 class="gradient-header">🛠️ Technologies & Tools</h2>

            <div class="center fade-in">
                <img src="https://img.shields.io/badge/-C%23-ff4da6?style=flat&logo=csharp&logoColor=white" alt="C#" class="pulsing-badge"/>
                <img src="https://img.shields.io/badge/-Unity-ff66b2?style=flat&logo=unity&logoColor=white" alt="Unity" class="pulsing-badge"/>
                <img src="https://img.shields.io/badge/-C++-ff4da6?style=flat&logo=cplusplus&logoColor=white" alt="C++" class="pulsing-badge"/>
                <img src="https://img.shields.io/badge/-Problem%20Solving-ff66b2?style=flat&logo=code&logoColor=white" alt="Problem Solving" class="pulsing-badge"/>
            </div>
        </div>

        <hr>

        <div class="section">
            <h2 class="gradient-header">📊 GitHub Stats & Top Languages</h2>

            <div class="center bounce-stats">
                <table style="margin: 0 auto;">
                    <tr>
                        <td>
                            <img src="https://github-readme-stats.vercel.app/api?username=maryamahmed0&show_icons=true&title_color=ff4da6&icon_color=ff66b2&text_color=ffffff&bg_color=0d1117&border_color=ff66b2" alt="Maryam's GitHub Stats" />
                        </td>
                        <td>
                            <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=maryamahmed0&layout=compact&title_color=ff4da6&text_color=ffffff&bg_color=0d1117&border_color=ff66b2" alt="Maryam's Top Languages" />
                        </td>
                    </tr>
                </table>
            </div>

            <div class="center bounce-stats" style="animation-delay: 0.5s;">
                <img src="https://streak-stats.demolab.com/?user=maryamahmed0&background=0D1117&ring=ff4da6&fire=ff66b2&currStreakNum=ffffff&sideNums=ffffff&currStreakLabel=ff66b2&sideLabels=ff4da6&dates=cccccc&border=ff66b2" alt="GitHub Streak"/>
            </div>
        </div>

        <hr>

        <div class="section glow-section">
            <h2 class="gradient-header">🚀 Projects</h2>

            <div class="fade-in">
                <p>- <span class="wave-emoji">🎮</span> <strong>Educational Game with Pygame + OpenCV</strong> — interactive learning using a webcam.<br>
                <code>Python</code> <code>Pygame</code> <code>OpenCV</code> • <a href="https://github.com/maryamahmed0/Catch-the-cuties">Repo</a></p>

                <p>- <span class="rotating-icon">🐍</span> <strong>Snake Game (Assembly)</strong> — classic snake game built entirely with Assembly language, focusing on low-level logic & graphics.<br>
                <code>Assembly</code> <code>x86</code> • <a href="https://github.com/maryamahmed0/Assymbly8086_SnakeGame">Repo</a></p>

                <p>- <span class="wave-emoji">📇</span> <strong>Contact Manager (OOP in C#)</strong> — desktop app to add, edit, and manage contacts, applying object-oriented principles.<br>
                <code>C#</code> <code>OOP</code> <code>WinForms/WPF</code> • <a href="https://github.com/maryamahmed0/Contact-Manager">Repo</a></p>
            </div>
        </div>

        <hr>

        <div class="section">
            <h2 class="gradient-header">🛎️ What I'm Up To</h2>

            <div class="fade-in">
                <p>- <span class="rotating-icon">🎮</span> Currently working on a <strong>game for a competition</strong> — polishing mechanics & visuals</p>
                <p>- <span class="wave-emoji">🎓</span> Starting my <strong>graduation project</strong> soon</p>
                <p>- <span class="rotating-icon">📚</span> Learning more about <strong>2D/3D development, advanced game programming & Unity networking</strong></p>
            </div>
        </div>

        <hr>

        <div class="section glow-section">
            <h2 class="gradient-header">🤝 Let's Collaborate</h2>

            <div class="fade-in">
                <p>If you enjoy <strong>cozy vibes, game jams, and creative coding</strong>,<br>
                I'd love to team up for:</p>
                <p>- <span class="wave-emoji">🎮</span> <strong>Game jam entries & competitions</strong></p>
                <p>- <span class="rotating-icon">🌱</span> Exploring <strong>2D / 3D game development</strong> & advanced programming</p>

                <p>Feel free to reach out — I'm always happy to connect with fellow devs & artists! <span class="wave-emoji">🌷</span></p>
            </div>
        </div>

        <hr>

        <div class="center fade-in">
            <sub>Thanks for visiting! <span class="rotating-icon">✨</span></sub>
        </div>
    </div>
</body>
</html>

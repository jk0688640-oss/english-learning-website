# english-learning-website
A complete English learning website (A1 to C2) with Hindi explanations, vocabulary, grammar, reading, writing, listening, and speaking practice.

english-master/
├── index.html
├── styles/
│   ├── style.css
│   └── responsive.css
├── scripts/
│   ├── main.js
│   ├── vocabulary.js
│   └── progress.js
├── images/
└── videos/
<!DOCTYPE html>
<html lang="hi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>EnglishMaster - Complete English Learning</title>
    <link rel="stylesheet" href="styles/style.css">
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css" rel="stylesheet">
</head>
<body>
    <!-- Navigation -->
    <nav class="navbar">
        <div class="nav-container">
            <div class="nav-logo">
                <i class="fas fa-graduation-cap"></i>
                <span>EnglishMaster</span>
            </div>
            <div class="nav-menu">
                <a href="#home" class="nav-link">Home</a>
                <a href="#levels" class="nav-link">Levels</a>
                <a href="#grammar" class="nav-link">Grammar</a>
                <a href="#vocabulary" class="nav-link">Vocabulary</a>
                <a href="#practice" class="nav-link">Practice</a>
                <a href="#progress" class="nav-link">Progress</a>
            </div>
            <div class="nav-auth">
                <button class="btn-login">Login</button>
                <button class="btn-signup">Sign Up</button>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section id="home" class="hero">
        <div class="hero-container">
            <div class="hero-content">
                <h1>Learn English from A1 to C2 Level</h1>
                <p>Complete English learning with real teacher explanations, vocabulary, and interactive practice</p>
                <div class="hero-buttons">
                    <button class="btn-primary">Start Learning Free</button>
                    <button class="btn-secondary">Take Level Test</button>
                </div>
                <div class="hero-stats">
                    <div class="stat">
                        <h3>10,000+</h3>
                        <p>Students Learning</p>
                    </div>
                    <div class="stat">
                        <h3>500+</h3>
                        <p>Video Lessons</p>
                    </div>
                    <div class="stat">
                        <h3>10,000+</h3>
                        <p>Vocabulary Words</p>
                    </div>
                </div>
            </div>
            <div class="hero-image">
                <img src="images/english-hero.svg" alt="English Learning">
            </div>
        </div>
    </section>

    <!-- Levels Section -->
    <section id="levels" class="levels">
        <div class="container">
            <h2 class="section-title">Learn Step by Step from A1 to C2</h2>
            <div class="levels-grid">
                <!-- A1 Level -->
                <div class="level-card" data-level="A1">
                    <div class="level-header">
                        <h3>A1 Beginner</h3>
                        <span class="level-badge">Starting Point</span>
                    </div>
                    <div class="level-content">
                        <div class="level-stats">
                            <div class="stat-item">
                                <i class="fas fa-book"></i>
                                <span>50+ Lessons</span>
                            </div>
                            <div class="stat-item">
                                <i class="fas fa-microphone"></i>
                                <span>1000+ Words</span>
                            </div>
                            <div class="stat-item">
                                <i class="fas fa-play-circle"></i>
                                <span>40+ Videos</span>
                            </div>
                        </div>
                        <ul class="level-features">
                            <li>Basic Grammar Rules</li>
                            <li>Essential Vocabulary</li>
                            <li>Simple Conversations</li>
                            <li>Pronunciation Basics</li>
                        </ul>
                        <button class="btn-level" onclick="startLevel('A1')">Start A1 Level</button>
                    </div>
                </div>

                <!-- A2 Level -->
                <div class="level-card" data-level="A2">
                    <div class="level-header">
                        <h3>A2 Elementary</h3>
                        <span class="level-badge">Next Step</span>
                    </div>
                    <div class="level-content">
                        <div class="level-stats">
                            <div class="stat-item">
                                <i class="fas fa-book"></i>
                                <span>60+ Lessons</span>
                            </div>
                            <div class="stat-item">
                                <i class="fas fa-microphone"></i>
                                <span>1200+ Words</span>
                            </div>
                            <div class="stat-item">
                                <i class="fas fa-play-circle"></i>
                                <span>50+ Videos</span>
                            </div>
                        </div>
                        <ul class="level-features">
                            <li>Intermediate Grammar</li>
                            <li>Daily Use Sentences</li>
                            <li>Better Pronunciation</li>
                            <li>Reading Practice</li>
                        </ul>
                        <button class="btn-level" onclick="startLevel('A2')">Start A2 Level</button>
                    </div>
                </div>

                <!-- B1 Level -->
                <div class="level-card" data-level="B1">
                    <div class="level-header">
                        <h3>B1 Intermediate</h3>
                        <span class="level-badge">Conversational</span>
                    </div>
                    <div class="level-content">
                        <div class="level-stats">
                            <div class="stat-item">
                                <i class="fas fa-book"></i>
                                <span>70+ Lessons</span>
                            </div>
                            <div class="stat-item">
                                <i class="fas fa-microphone"></i>
                                <span>1500+ Words</span>
                            </div>
                            <div class="stat-item">
                                <i class="fas fa-play-circle"></i>
                                <span>60+ Videos</span>
                            </div>
                        </div>
                        <ul class="level-features">
                            <li>Advanced Grammar</li>
                            <li>Fluency Building</li>
                            <li>Writing Skills</li>
                            <li>Business English</li>
                        </ul>
                        <button class="btn-level" onclick="startLevel('B1')">Start B1 Level</button>
                    </div>
                </div>

                <!-- B2 Level -->
                <div class="level-card" data-level="B2">
                    <div class="level-header">
                        <h3>B2 Upper-Intermediate</h3>
                        <span class="level-badge">Advanced</span>
                    </div>
                    <div class="level-content">
                        <div class="level-stats">
                            <div class="stat-item">
                                <i class="fas fa-book"></i>
                                <span>80+ Lessons</span>
                            </div>
                            <div class="stat-item">
                                <i class="fas fa-microphone"></i>
                                <span>1800+ Words</span>
                            </div>
                            <div class="stat-item">
                                <i class="fas fa-play-circle"></i>
                                <span>70+ Videos</span>
                            </div>
                        </div>
                        <ul class="level-features">
                            <li>Complex Grammar</li>
                            <li>Academic Writing</li>
                            <li>Professional Communication</li>
                            <li>Presentation Skills</li>
                        </ul>
                        <button class="btn-level" onclick="startLevel('B2')">Start B2 Level</button>
                    </div>
                </div>

                <!-- C1 Level -->
                <div class="level-card" data-level="C1">
                    <div class="level-header">
                        <h3>C1 Advanced</h3>
                        <span class="level-badge">Expert</span>
                    </div>
                    <div class="level-content">
                        <div class="level-stats">
                            <div class="stat-item">
                                <i class="fas fa-book"></i>
                                <span>90+ Lessons</span>
                            </div>
                            <div class="stat-item">
                                <i class="fas fa-microphone"></i>
                                <span>2000+ Words</span>
                            </div>
                            <div class="stat-item">
                                <i class="fas fa-play-circle"></i>
                                <span>80+ Videos</span>
                            </div>
                        </div>
                        <ul class="level-features">
                            <li>Master Grammar</li>
                            <li>Native Expressions</li>
                            <li>Advanced Writing</li>
                            <li>Cultural Context</li>
                        </ul>
                        <button class="btn-level" onclick="startLevel('C1')">Start C1 Level</button>
                    </div>
                </div>

                <!-- C2 Level -->
                <div class="level-card" data-level="C2">
                    <div class="level-header">
                        <h3>C2 Proficient</h3>
                        <span class="level-badge">Master</span>
                    </div>
                    <div class="level-content">
                        <div class="level-stats">
                            <div class="stat-item">
                                <i class="fas fa-book"></i>
                                <span>100+ Lessons</span>
                            </div>
                            <div class="stat-item">
                                <i class="fas fa-microphone"></i>
                                <span>2500+ Words</span>
                            </div>
                            <div class="stat-item">
                                <i class="fas fa-play-circle"></i>
                                <span>90+ Videos</span>
                            </div>
                        </div>
                        <ul class="level-features">
                            <li>Native Level Fluency</li>
                            <li>Professional Mastery</li>
                            <li>Academic Excellence</li>
                            <li>Cultural Nuances</li>
                        </ul>
                        <button class="btn-level" onclick="startLevel('C2')">Start C2 Level</button>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Grammar Section -->
    <section id="grammar" class="grammar">
        <div class="container">
            <h2 class="section-title">Learn Grammar with Real Teacher Videos</h2>
            <div class="grammar-container">
                <div class="grammar-sidebar">
                    <h3>Grammar Topics</h3>
                    <div class="grammar-topics">
                        <div class="topic-category">
                            <h4>A1 Level Grammar</h4>
                            <div class="topic-list">
                                <button class="topic-btn active" data-topic="tenses">Tenses</button>
                                <button class="topic-btn" data-topic="articles">Articles</button>
                                <button class="topic-btn" data-topic="prepositions">Prepositions</button>
                                <button class="topic-btn" data-topic="verbs">Basic Verbs</button>
                            </div>
                        </div>
                        <div class="topic-category">
                            <h4>A2 Level Grammar</h4>
                            <div class="topic-list">
                                <button class="topic-btn" data-topic="modals">Modal Verbs</button>
                                <button class="topic-btn" data-topic="conditionals">Conditionals</button>
                                <button class="topic-btn" data-topic="passive">Passive Voice</button>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="grammar-content">
                    <div class="video-player">
                        <div class="video-placeholder">
                            <i class="fas fa-play-circle"></i>
                            <p>Select a grammar topic to start learning</p>
                        </div>
                    </div>
                    <div class="grammar-explanation">
                        <h3 id="topic-title">Grammar Topic</h3>
                        <div class="explanation-content">
                            <div class="hindi-explanation">
                                <h4>Hindi Explanation</h4>
                                <p id="hindi-desc">Select a topic to see Hindi explanation</p>
                            </div>
                            <div class="examples">
                                <h4>Examples</h4>
                                <div id="examples-list">
                                    <div class="example-item">
                                        <span class="english">I go to school every day.</span>
                                        <span class="hindi">मैं रोज स्कूल जाता हूं।</span>
                                    </div>
                                </div>
                            </div>
                            <div class="practice-section">
                                <h4>Practice Exercise</h4>
                                <div class="exercise" id="current-exercise">
                                    <p>Complete the sentence: She ___ to market every day.</p>
                                    <div class="options">
                                        <button class="option-btn">go</button>
                                        <button class="option-btn">goes</button>
                                        <button class="option-btn">going</button>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Vocabulary Section -->
    <section id="vocabulary" class="vocabulary">
        <div class="container">
            <h2 class="section-title">Build Your Vocabulary</h2>
            <div class="vocabulary-controls">
                <select id="level-select" onchange="loadVocabulary()">
                    <option value="A1">A1 Level (1000+ Words)</option>
                    <option value="A2">A2 Level (1200+ Words)</option>
                    <option value="B1">B1 Level (1500+ Words)</option>
                    <option value="B2">B2 Level (1800+ Words)</option>
                    <option value="C1">C1 Level (2000+ Words)</option>
                    <option value="C2">C2 Level (2500+ Words)</option>
                </select>
                <div class="search-box">
                    <input type="text" id="vocab-search" placeholder="Search vocabulary...">
                    <i class="fas fa-search"></i>
                </div>
            </div>
            <div class="vocabulary-grid" id="vocabulary-grid">
                <!-- Vocabulary cards will be loaded here -->
            </div>
            <div class="vocabulary-pagination">
                <button id="prev-page">Previous</button>
                <span id="page-info">Page 1 of 10</span>
                <button id="next-page">Next</button>
            </div>
        </div>
    </section>

    <!-- Practice Section -->
    <section id="practice" class="practice">
        <div class="container">
            <h2 class="section-title">Practice All Skills</h2>
            <div class="practice-grid">
                <div class="practice-card listening">
                    <div class="practice-icon">
                        <i class="fas fa-headphones"></i>
                    </div>
                    <h3>Listening</h3>
                    <p>Improve your listening skills with audio exercises</p>
                    <button class="btn-practice" onclick="startPractice('listening')">Start Practice</button>
                </div>
                <div class="practice-card speaking">
                    <div class="practice-icon">
                        <i class="fas fa-microphone"></i>
                    </div>
                    <h3>Speaking</h3>
                    <p>Practice pronunciation and speaking</p>
                    <button class="btn-practice" onclick="startPractice('speaking')">Start Practice</button>
                </div>
                <div class="practice-card reading">
                    <div class="practice-icon">
                        <i class="fas fa-book-open"></i>
                    </div>
                    <h3>Reading</h3>
                    <p>Read and comprehend English texts</p>
                    <button class="btn-practice" onclick="startPractice('reading')">Start Practice</button>
                </div>
                <div class="practice-card writing">
                    <div class="practice-icon">
                        <i class="fas fa-pencil-alt"></i>
                    </div>
                    <h3>Writing</h3>
                    <p>Improve your writing skills</p>
                    <button class="btn-practice" onclick="startPractice('writing')">Start Practice</button>
                </div>
            </div>
        </div>
    </section>

    <!-- Progress Section -->
    <section id="progress" class="progress">
        <div class="container">
            <h2 class="section-title">Track Your Progress</h2>
            <div class="progress-dashboard">
                <div class="progress-stats">
                    <div class="progress-card">
                        <h3>Current Level</h3>
                        <div class="level-display">A1</div>
                        <p>Beginner</p>
                    </div>
                    <div class="progress-card">
                        <h3>Vocabulary Learned</h3>
                        <div class="progress-number">150</div>
                        <p>out of 1000 words</p>
                    </div>
                    <div class="progress-card">
                        <h3>Grammar Completed</h3>
                        <div class="progress-number">45%</div>
                        <p>20/50 topics</p>
                    </div>
                    <div class="progress-card">
                        <h3>Learning Streak</h3>
                        <div class="progress-number">7 days</div>
                        <p>Keep going!</p>
                    </div>
                </div>
                <div class="progress-chart">
                    <canvas id="progressChart"></canvas>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="footer">
        <div class="container">
            <div class="footer-content">
                <div class="footer-section">
                    <h3>EnglishMaster</h3>
                    <p>Complete English learning platform from basic to advanced levels with real teacher guidance.</p>
                </div>
                <div class="footer-section">
                    <h4>Quick Links</h4>
                    <a href="#home">Home</a>
                    <a href="#levels">Levels</a>
                    <a href="#grammar">Grammar</a>
                    <a href="#vocabulary">Vocabulary</a>
                </div>
                <div class="footer-section">
                    <h4>Support</h4>
                    <a href="#">Help Center</a>
                    <a href="#">Contact Us</a>
                    <a href="#">Privacy Policy</a>
                    <a href="#">Terms of Service</a>
                </div>
            </div>
            <div class="footer-bottom">
                <p>&copy; 2024 EnglishMaster. All rights reserved.</p>
            </div>
        </div>
    </footer>

    <script src="scripts/vocabulary.js"></script>
    <script src="scripts/progress.js"></script>
    <script src="scripts/main.js"></script>
</body>
</html>
/* Reset and Base Styles */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

:root {
    --primary-color: #4f46e5;
    --primary-dark: #4338ca;
    --secondary-color: #10b981;
    --accent-color: #f59e0b;
    --text-primary: #1f2937;
    --text-secondary: #6b7280;
    --bg-light: #f9fafb;
    --bg-white: #ffffff;
    --border-color: #e5e7eb;
    --shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1);
    --shadow-lg: 0 10px 15px -3px rgba(0, 0, 0, 0.1);
}

body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    line-height: 1.6;
    color: var(--text-primary);
    background-color: var(--bg-light);
}

.container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 20px;
}

/* Navigation */
.navbar {
    background: var(--bg-white);
    box-shadow: var(--shadow);
    position: fixed;
    top: 0;
    width: 100%;
    z-index: 1000;
}

.nav-container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 20px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 70px;
}

.nav-logo {
    display: flex;
    align-items: center;
    font-size: 1.5rem;
    font-weight: bold;
    color: var(--primary-color);
}

.nav-logo i {
    margin-right: 10px;
    font-size: 2rem;
}

.nav-menu {
    display: flex;
    gap: 2rem;
}

.nav-link {
    text-decoration: none;
    color: var(--text-primary);
    font-weight: 500;
    transition: color 0.3s;
}

.nav-link:hover {
    color: var(--primary-color);
}

.nav-auth {
    display: flex;
    gap: 1rem;
}

.btn-login, .btn-signup {
    padding: 8px 20px;
    border: none;
    border-radius: 6px;
    font-weight: 500;
    cursor: pointer;
    transition: all 0.3s;
}

.btn-login {
    background: transparent;
    color: var(--primary-color);
    border: 2px solid var(--primary-color);
}

.btn-signup {
    background: var(--primary-color);
    color: white;
}

.btn-login:hover {
    background: var(--primary-color);
    color: white;
}

.btn-signup:hover {
    background: var(--primary-dark);
}

/* Hero Section */
.hero {
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    color: white;
    padding: 120px 0 80px;
    margin-top: 70px;
}

.hero-container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 20px;
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 4rem;
    align-items: center;
}

.hero-content h1 {
    font-size: 3rem;
    margin-bottom: 1rem;
    line-height: 1.2;
}

.hero-content p {
    font-size: 1.2rem;
    margin-bottom: 2rem;
    opacity: 0.9;
}

.hero-buttons {
    display: flex;
    gap: 1rem;
    margin-bottom: 3rem;
}

.btn-primary, .btn-secondary {
    padding: 12px 30px;
    border: none;
    border-radius: 8px;
    font-size: 1.1rem;
    font-weight: 600;
    cursor: pointer;
    transition: all 0.3s;
}

.btn-primary {
    background: var(--accent-color);
    color: white;
}

.btn-secondary {
    background: transparent;
    color: white;
    border: 2px solid white;
}

.btn-primary:hover {
    background: #e59a0b;
    transform: translateY(-2px);
}

.btn-secondary:hover {
    background: white;
    color: var(--primary-color);
}

.hero-stats {
    display: flex;
    gap: 2rem;
}

.stat h3 {
    font-size: 2rem;
    margin-bottom: 0.5rem;
}

.stat p {
    font-size: 1rem;
    opacity: 0.8;
}

.hero-image img {
    width: 100%;
    max-width: 500px;
    animation: float 3s ease-in-out infinite;
}

@keyframes float {
    0%, 100% { transform: translateY(0px); }
    50% { transform: translateY(-20px); }
}

/* Levels Section */
.levels {
    padding: 80px 0;
    background: var(--bg-white);
}

.section-title {
    text-align: center;
    font-size: 2.5rem;
    margin-bottom: 3rem;
    color: var(--text-primary);
}

.levels-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
    gap: 2rem;
}

.level-card {
    background: var(--bg-white);
    border-radius: 12px;
    box-shadow: var(--shadow);
    overflow: hidden;
    transition: transform 0.3s, box-shadow 0.3s;
    border: 1px solid var(--border-color);
}

.level-card:hover {
    transform: translateY(-5px);
    box-shadow: var(--shadow-lg);
}

.level-header {
    background: linear-gradient(135deg, var(--primary-color), var(--primary-dark));
    color: white;
    padding: 1.5rem;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.level-header h3 {
    font-size: 1.5rem;
}

.level-badge {
    background: var(--accent-color);
    padding: 4px 12px;
    border-radius: 20px;
    font-size: 0.8rem;
    font-weight: 600;
}

.level-content {
    padding: 1.5rem;
}

.level-stats {
    display: flex;
    justify-content: space-between;
    margin-bottom: 1.5rem;
}

.stat-item {
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
}

.stat-item i {
    font-size: 1.5rem;
    color: var(--primary-color);
    margin-bottom: 0.5rem;
}

.stat-item span {
    font-size: 0.9rem;
    color: var(--text-secondary);
}

.level-features {
    list-style: none;
    margin-bottom: 2rem;
}

.level-features li {
    padding: 0.5rem 0;
    border-bottom: 1px solid var(--border-color);
    position: relative;
    padding-left: 1.5rem;
}

.level-features li:before {
    content: '✓';
    position: absolute;
    left: 0;
    color: var(--secondary-color);
    font-weight: bold;
}

.level-features li:last-child {
    border-bottom: none;
}

.btn-level {
    width: 100%;
    padding: 12px;
    background: var(--primary-color);
    color: white;
    border: none;
    border-radius: 8px;
    font-size: 1rem;
    font-weight: 600;
    cursor: pointer;
    transition: background 0.3s;
}

.btn-level:hover {
    background: var(--primary-dark);
}

/* Grammar Section */
.grammar {
    padding: 80px 0;
    background: var(--bg-light);
}

.grammar-container {
    display: grid;
    grid-template-columns: 300px 1fr;
    gap: 2rem;
}

.grammar-sidebar {
    background: var(--bg-white);
    border-radius: 12px;
    padding: 1.5rem;
    box-shadow: var(--shadow);
    height: fit-content;
}

.grammar-sidebar h3 {
    margin-bottom: 1rem;
    color: var(--text-primary);
}

.topic-category {
    margin-bottom: 2rem;
}

.topic-category h4 {
    color: var(--text-secondary);
    margin-bottom: 1rem;
    font-size: 1rem;
}

.topic-list {
    display: flex;
    flex-direction: column;
    gap: 0.5rem;
}

.topic-btn {
    padding: 10px 15px;
    background: transparent;
    border: 1px solid var(--border-color);
    border-radius: 6px;
    text-align: left;
    cursor: pointer;
    transition: all 0.3s;
}

.topic-btn:hover {
    background: var(--bg-light);
}

.topic-btn.active {
    background: var(--primary-color);
    color: white;
    border-color: var(--primary-color);
}

.grammar-content {
    background: var(--bg-white);
    border-radius: 12px;
    padding: 2rem;
    box-shadow: var(--shadow);
}

.video-player {
    background: #1f2937;
    border-radius: 8px;
    height: 400px;
    display: flex;
    align-items: center;
    justify-content: center;
    margin-bottom: 2rem;
    position: relative;
}

.video-placeholder {
    text-align: center;
    color: white;
}

.video-placeholder i {
    font-size: 4rem;
    margin-bottom: 1rem;
    opacity: 0.7;
}

.grammar-explanation h3 {
    margin-bottom: 1.5rem;
    color: var(--text-primary);
}

.explanation-content {
    display: grid;
    gap: 2rem;
}

.hindi-explanation, .examples, .practice-section {
    background: var(--bg-light);
    padding: 1.5rem;
    border-radius: 8px;
}

.hindi-explanation h4, .examples h4, .practice-section h4 {
    margin-bottom: 1rem;
    color: var(--text-primary);
}

.example-item {
    display: flex;
    justify-content: space-between;
    padding: 0.5rem 0;
    border-bottom: 1px solid var(--border-color);
}

.example-item:last-child {
    border-bottom: none;
}

.english {
    font-weight: 500;
}

.hindi {
    color: var(--text-secondary);
}

.options {
    display: flex;
    gap: 1rem;
    margin-top: 1rem;
}

.option-btn {
    padding: 8px 16px;
    background: var(--bg-white);
    border: 1px solid var(--border-color);
    border-radius: 6px;
    cursor: pointer;
    transition: all 0.3s;
}

.option-btn:hover {
    background: var(--primary-color);
    color: white;
}

/* Vocabulary Section */
.vocabulary {
    padding: 80px 0;
    background: var(--bg-white);
}

.vocabulary-controls {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 2rem;
    gap: 1rem;
}

#level-select {
    padding: 10px 15px;
    border: 1px solid var(--border-color);
    border-radius: 6px;
    font-size: 1rem;
    background: var(--bg-white);
}

.search-box {
    position: relative;
    flex: 1;
    max-width: 400px;
}

#vocab-search {
    width: 100%;
    padding: 10px 15px 10px 40px;
    border: 1px solid var(--border-color);
    border-radius: 6px;
    font-size: 1rem;
}

.search-box i {
    position: absolute;
    left: 15px;
    top: 50%;
    transform: translateY(-50%);
    color: var(--text-secondary);
}

.vocabulary-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
    gap: 1.5rem;
    margin-bottom: 2rem;
}

.vocab-card {
    background: var(--bg-white);
    border: 1px solid var(--border-color);
    border-radius: 8px;
    padding: 1.5rem;
    transition: all 0.3s;
}

.vocab-card:hover {
    box-shadow: var(--shadow);
    transform: translateY(-2px);
}

.vocab-word {
    font-size: 1.2rem;
    font-weight: 600;
    color: var(--text-primary);
    margin-bottom: 0.5rem;
}

.vocab-meaning {
    color: var(--text-secondary);
    margin-bottom: 1rem;
}

.vocab-example {
    font-style: italic;
    color: var(--text-primary);
    margin-bottom: 1rem;
    border-left: 3px solid var(--primary-color);
    padding-left: 1rem;
}

.vocab-actions {
    display: flex;
    gap: 0.5rem;
}

.vocab-btn {
    padding: 5px 10px;
    border: none;
    border-radius: 4px;
    font-size: 0.8rem;
    cursor: pointer;
    transition: background 0.3s;
}

.btn-audio {
    background: var(--secondary-color);
    color: white;
}

.btn-bookmark {
    background: var(--accent-color);
    color: white;
}

.vocabulary-pagination {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 1rem;
}

#prev-page, #next-page {
    padding: 8px 16px;
    border: 1px solid var(--border-color);
    background: var(--bg-white);
    border-radius: 6px;
    cursor: pointer;
    transition: all 0.3s;
}

#prev-page:hover, #next-page:hover {
    background: var(--primary-color);
    color: white;
}

/* Practice Section */
.practice {
    padding: 80px 0;
    background: var(--bg-light);
}

.practice-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 2rem;
}

.practice-card {
    background: var(--bg-white);
    padding: 2rem;
    border-radius: 12px;
    text-align: center;
    box-shadow: var(--shadow);
    transition: transform 0.3s;
}

.practice-card:hover {
    transform: translateY(-5px);
}

.practice-icon {
    width: 80px;
    height: 80px;
    background: var(--primary-color);
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    margin: 0 auto 1.5rem;
}

.practice-icon i {
    font-size: 2rem;
    color: white;
}

.practice-card h3 {
    margin-bottom: 1rem;
    color: var(--text-primary);
}

.practice-card p {
    color: var(--text-secondary);
    margin-bottom: 1.5rem;
}

.btn-practice {
    padding: 10px 20px;
    background: var(--primary-color);
    color: white;
    border: none;
    border-radius: 6px;
    cursor: pointer;
    transition: background 0.3s;
}

.btn-practice:hover {
    background: var(--primary-dark);
}

/* Progress Section */
.progress {
    padding: 80px 0;
    background: var(--bg-white);
}

.progress-dashboard {
    display: grid;
    grid-template-columns: 1fr 2fr;
    gap: 3rem;
}

.progress-stats {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 1.5rem;
}

.progress-card {
    background: var(--bg-light);
    padding: 1.5rem;
    border-radius: 12px;
    text-align: center;
    box-shadow: var(--shadow);
}

.progress-card h3 {
    color: var(--text-secondary);
    font-size: 0.9rem;
    margin-bottom: 1rem;
}

.level-display, .progress-number {
    font-size: 2rem;
    font-weight: bold;
    color: var(--primary-color);
    margin-bottom: 0.5rem;
}

.progress-card p {
    color: var(--text-secondary);
    font-size: 0.9rem;
}

.progress-chart {
    background: var(--bg-light);
    padding: 2rem;
    border-radius: 12px;
    box-shadow: var(--shadow);
}

/* Footer */
.footer {
    background: var(--text-primary);
    color: white;
    padding: 50px 0 20px;
}

.footer-content {
    display: grid;
    grid-template-columns: 2fr 1fr 1fr;
    gap: 3rem;
    margin-bottom: 2rem;
}

.footer-section h3, .footer-section h4 {
    margin-bottom: 1rem;
}

.footer-section a {
    display: block;
    color: #d1d5db;
    text-decoration: none;
    margin-bottom: 0.5rem;
    transition: color 0.3s;
}

.footer-section a:hover {
    color: white;
}

.footer-bottom {
    text-align: center;
    padding-top: 2rem;
    border-top: 1px solid #374151;
    color: #9ca3af;
}

/* Responsive Design */
@media (max-width: 768px) {
    .nav-menu {
        display: none;
    }
    
    .hero-container {
        grid-template-columns: 1fr;
        text-align: center;
    }
    
    .hero-content h1 {
        font-size: 2rem;
    }
    
    .hero-buttons {
        flex-direction: column;
        align-items: center;
    }
    
    .hero-stats {
        justify-content: center;
    }
    
    .levels-grid {
        grid-template-columns: 1fr;
    }
    
    .grammar-container {
        grid-template-columns: 1fr;
    }
    
    .vocabulary-controls {
        flex-direction: column;
    }
    
    .search-box {
        max-width: 100%;
    }
    
    .practice-grid {
        grid-template-columns: 1fr;
    }
    
    .progress-dashboard {
        grid-template-columns: 1fr;
    }
    
    .progress-stats {
        grid-template-columns: 1fr;
    }
    
    .footer-content {
        grid-template-columns: 1fr;
    }
}
// Main JavaScript for EnglishMaster Website

// Initialize the application
document.addEventListener('DOMContentLoaded', function() {
    initializeApp();
    loadVocabulary();
    setupEventListeners();
});

// Initialize application
function initializeApp() {
    // Check if user is logged in
    const user = JSON.parse(localStorage.getItem('englishMasterUser'));
    if (user) {
        updateUIForLoggedInUser(user);
    }
    
    // Initialize progress chart
    initializeProgressChart();
    
    // Load initial grammar topic
    loadGrammarTopic('tenses');
}

// Setup event listeners
function setupEventListeners() {
    // Grammar topic buttons
    const topicButtons = document.querySelectorAll('.topic-btn');
    topicButtons.forEach(button => {
        button.addEventListener('click', function() {
            const topic = this.getAttribute('data-topic');
            loadGrammarTopic(topic);
            
            // Update active state
            topicButtons.forEach(btn => btn.classList.remove('active'));
            this.classList.add('active');
        });
    });
    
    // Vocabulary pagination
    document.getElementById('prev-page').addEventListener('click', previousVocabularyPage);
    document.getElementById('next-page').addEventListener('click', nextVocabularyPage);
    
    // Vocabulary search
    document.getElementById('vocab-search').addEventListener('input', searchVocabulary);
    
    // Level selection
    document.getElementById('level-select').addEventListener('change', loadVocabulary);
}

// Start a learning level
function startLevel(level) {
    const user = JSON.parse(localStorage.getItem('englishMasterUser')) || {};
    user.currentLevel = level;
    user.progress = user.progress || {};
    user.progress[level] = user.progress[level] || { started: true, startDate: new Date().toISOString() };
    
    localStorage.setItem('englishMasterUser', JSON.stringify(user));
    
    // Show confirmation message
    showNotification(`Started ${level} level successfully!`, 'success');
    
    // Update progress display
    updateProgressDisplay();
}

// Load grammar topic
function loadGrammarTopic(topic) {
    const grammarData = {
        tenses: {
            title: "English Tenses - काल",
            hindiDesc: "इंग्लिश में टेंस्सेस (काल) समय को दर्शाते हैं। यह बताते हैं कि कार्य कब हुआ - वर्तमान, भूत या भविष्य में।",
            examples: [
                { english: "I play cricket every day.", hindi: "मैं रोज क्रिकेट खेलता हूं।" },
                { english: "She is reading a book now.", hindi: "वह अभी एक किताब पढ़ रही है।" },
                { english: "They have completed their work.", hindi: "उन्होंने अपना काम पूरा कर लिया है।" },
                { english: "We will go to market tomorrow.", hindi: "हम कल बाजार जाएंगे।" }
            ],
            exercise: {
                question: "Complete the sentence: He ___ football every evening.",
                options: ["play", "plays", "playing", "played"],
                correct: "plays"
            }
        },
        articles: {
            title: "Articles - A, An, The",
            hindiDesc: "Articles (उपपद) संज्ञा के पहले आते हैं। A और An indefinite articles हैं, The definite article है।",
            examples: [
                { english: "A boy is playing outside.", hindi: "एक लड़का बाहर खेल रहा है।" },
                { english: "An apple a day keeps doctor away.", hindi: "रोज एक सेब डॉक्टर को दूर रखता है।" },
                { english: "The sun rises in the east.", hindi: "सूरज पूर्व में उगता है।" }
            ],
            exercise: {
                question: "Choose the correct article: She is ___ honest person.",
                options: ["a", "an", "the", "no article"],
                correct: "an"
            }
        },
        prepositions: {
            title: "Prepositions - संबंधसूचक अव्यय",
            hindiDesc: "Prepositions दो शब्दों के बीच संबंध दर्शाते हैं, जैसे स्थान, समय, दिशा आदि।",
            examples: [
                { english: "The book is on the table.", hindi: "किताब मेज पर है।" },
                { english: "We will meet at 5 PM.", hindi: "हम 5 बजे मिलेंगे।" },
                { english: "She comes from Delhi.", hindi: "वह दिल्ली से आती है।" }
            ],
            exercise: {
                question: "Fill in the blank: The cat jumped ___ the wall.",
                options: ["on", "over", "in", "at"],
                correct: "over"
            }
        }
    };
    
    const data = grammarData[topic] || grammarData.tenses;
    
    // Update UI
    document.getElementById('topic-title').textContent = data.title;
    document.getElementById('hindi-desc').textContent = data.hindiDesc;
    
    // Update examples
    const examplesList = document.getElementById('examples-list');
    examplesList.innerHTML = '';
    data.examples.forEach(example => {
        const exampleItem = document.createElement('div');
        exampleItem.className = 'example-item';
        exampleItem.innerHTML = `
            <span class="english">${example.english}</span>
            <span class="hindi">${example.hindi}</span>
        `;
        examplesList.appendChild(exampleItem);
    });
    
    // Update exercise
    const exercise = document.getElementById('current-exercise');
    exercise.innerHTML = `
        <p>${data.exercise.question}</p>
        <div class="options">
            ${data.exercise.options.map(option => 
                `<button class="option-btn" onclick="checkAnswer('${option}', '${data.exercise.correct}')">${option}</button>`
            ).join('')}
        </div>
    `;
}

// Check exercise answer
function checkAnswer(selected, correct) {
    const buttons = document.querySelectorAll('.option-btn');
    buttons.forEach(button => {
        button.disabled = true;
        if (button.textContent === correct) {
            button.style.background = '#10b981';
            button.style.color = 'white';
        } else if (button.textContent === selected) {
            button.style.background = '#ef4444';
            button.style.color = 'white';
        }
    });
    
    if (selected === correct) {
        showNotification('Correct answer! Well done!', 'success');
        updateUserProgress('grammar', 1);
    } else {
        showNotification(`Incorrect. The right answer is: ${correct}`, 'error');
    }
}

// Show notification
function showNotification(message, type) {
    const notification = document.createElement('div');
    notification.className = `notification ${type}`;
    notification.textContent = message;
    notification.style.cssText = `
        position: fixed;
        top: 100px;
        right: 20px;
        padding: 15px 20px;
        background: ${type === 'success' ? '#10b981' : '#ef4444'};
        color: white;
        border-radius: 8px;
        box-shadow: 0 4px 6px rgba(0,0,0,0.1);
        z-index: 1000;
        animation: slideIn 0.3s ease;
    `;
    
    document.body.appendChild(notification);
    
    setTimeout(() => {
        notification.remove();
    }, 3000);
}

// Update user progress
function updateUserProgress(category, points) {
    const user = JSON.parse(localStorage.getItem('englishMasterUser')) || {};
    user.progress = user.progress || {};
    user.progress[category] = (user.progress[category] || 0) + points;
    
    localStorage.setItem('englishMasterUser', JSON.stringify(user));
    updateProgressDisplay();
}

// Update progress display
function updateProgressDisplay() {
    const user = JSON.parse(localStorage.getItem('englishMasterUser')) || {};
    const progress = user.progress || {};
    
    // Update progress cards
    const levelDisplay = document.querySelector('.level-display');
    const vocabProgress = document.querySelector('.progress-number:nth-child(2)');
    const grammarProgress = document.querySelector('.progress-number:nth-child(3)');
    const streakDisplay = document.querySelector('.progress-number:nth-child(4)');
    
    if (levelDisplay) {
        levelDisplay.textContent = user.currentLevel || 'A1';
    }
    
    if (vocabProgress) {
        const vocabLearned = progress.vocabulary || 150;
        vocabProgress.textContent = vocabLearned;
        vocabProgress.nextElementSibling.textContent = `out of ${getLevelWordCount(user.currentLevel || 'A1')} words`;
    }
    
    if (grammarProgress) {
        const grammarCompleted = progress.grammar || 20;
        const totalTopics = 50;
        const percentage = Math.round((grammarCompleted / totalTopics) * 100);
        grammarProgress.textContent = `${percentage}%`;
        grammarProgress.nextElementSibling.textContent = `${grammarCompleted}/${totalTopics} topics`;
    }
    
    if (streakDisplay) {
        streakDisplay.textContent = progress.streak || '7';
    }
}

// Get word count for level
function getLevelWordCount(level) {
    const wordCounts = {
        'A1': 1000,
        'A2': 1200,
        'B1': 1500,
        'B2': 1800,
        'C1': 2000,
        'C2': 2500
    };
    return wordCounts[level] || 1000;
}

// Initialize progress chart
function initializeProgressChart() {
    const ctx = document.getElementById('progressChart').getContext('2d');
    
    // Simple chart implementation (in real app, use Chart.js)
    const canvas = document.getElementById('progressChart');
    const context = canvas.getContext('2d');
    
    // Set canvas size
    canvas.width = canvas.offsetWidth;
    canvas.height = canvas.offsetHeight;
    
    // Draw simple chart
    context.fillStyle = '#f3f4f6';
    context.fillRect(0, 0, canvas.width, canvas.height);
    
    context.fillStyle = '#4f46e5';
    context.font = '16px Arial';
    context.textAlign = 'center';
    context.fillText('Progress Chart - Coming Soon', canvas.width/2, canvas.height/2);
}

// Update UI for logged in user
function updateUIForLoggedInUser(user) {
    const navAuth = document.querySelector('.nav-auth');
    if (navAuth) {
        navAuth.innerHTML = `
            <span style="margin-right: 1rem;">Hello, ${user.name || 'User'}</span>
            <button class="btn-logout" onclick="logout()">Logout</button>
        `;
    }
}

// Logout function
function logout() {
    localStorage.removeItem('englishMasterUser');
    location.reload();
}

// Start practice session
function startPractice(type) {
    const practiceTypes = {
        listening: "Listening Practice",
        speaking: "Speaking Practice", 
        reading: "Reading Practice",
        writing: "Writing Practice"
    };
    
    showNotification(`Starting ${practiceTypes[type]}...`, 'success');
    
    // In real implementation, redirect to practice page
    setTimeout(() => {
        alert(`${practiceTypes[type]} feature will be implemented in the next version!`);
    }, 1000);
}

// Vocabulary Management

let currentVocabularyPage = 1;
const wordsPerPage = 12;
let currentVocabulary = [];
let filteredVocabulary = [];

// Sample vocabulary data for A1 level
const vocabularyData = {
    A1: [
        { word: "Hello", meaning: "नमस्ते", example: "Hello, how are you?" },
        { word: "Goodbye", meaning: "अलविदा", example: "Goodbye, see you tomorrow!" },
        { word: "Please", meaning: "कृपया", example: "Please help me." },
        { word: "Thank you", meaning: "धन्यवाद", example: "Thank you for your help." },
        { word: "Yes", meaning: "हाँ", example: "Yes, I understand." },
        { word: "No", meaning: "नहीं", example: "No, thank you." },
        { word: "Sorry", meaning: "माफ़ कीजिए", example: "Sorry, I am late." },
        { word: "Excuse me", meaning: "माफ़ कीजिए", example: "Excuse me, where is the station?" },
        { word: "Water", meaning: "पानी", example: "I need some water." },
        { word: "Food", meaning: "खाना", example: "The food is delicious." },
        { word: "House", meaning: "घर", example: "This is my house." },
        { word: "Family", meaning: "परिवार", example: "I love my family." },
        { word: "Friend", meaning: "दोस्त", example: "He is my best friend." },
        { word: "School", meaning: "स्कूल", example: "I go to school every day." },
        { word: "Teacher", meaning: "शिक्षक", example: "Our teacher is very kind." },
        { word: "Student", meaning: "छात्र", example: "She is a good student." },
        { word: "Book", meaning: "किताब", example: "This book is interesting." },
        { word: "Pen", meaning: "कलम", example: "Can I borrow your pen?" },
        { word: "Paper", meaning: "कागज़", example: "I need a piece of paper." },
        { word: "Computer", meaning: "कंप्यूटर", example: "I work on computer." },
        { word: "Phone", meaning: "फ़ोन", example: "My phone is ringing." },
        { word: "Car", meaning: "गाड़ी", example: "We have a new car." },
        { word: "Bus", meaning: "बस", example: "I take bus to office." },
        { word: "Train", meaning: "ट्रेन", example: "The train is late today." },
        { word: "Time", meaning: "समय", example: "What time is it?" },
        { word: "Day", meaning: "दिन", example: "Have a nice day!" },
        { word: "Night", meaning: "रात", example: "Good night!" },
        { word: "Morning", meaning: "सुबह", example: "Good morning!" },
        { word: "Evening", meaning: "शाम", example: "Good evening!" },
        { word: "Today", meaning: "आज", example: "Today is Monday." },
        { word: "Tomorrow", meaning: "कल", example: "See you tomorrow." },
        { word: "Yesterday", meaning: "कल", example: "I met him yesterday." },
        { word: "Now", meaning: "अब", example: "I am busy now." },
        { word: "Later", meaning: "बाद में", example: "We will talk later." },
        { word: "Big", meaning: "बड़ा", example: "This is a big house." },
        { word: "Small", meaning: "छोटा", example: "I have a small car." },
        { word: "Good", meaning: "अच्छा", example: "She is a good person." },
        { word: "Bad", meaning: "बुरा", example: "This is a bad idea." },
        { word: "Hot", meaning: "गर्म", example: "The tea is hot." },
        { word: "Cold", meaning: "ठंडा", example: "The water is cold." },
        { word: "Happy", meaning: "खुश", example: "I am very happy today." },
        { word: "Sad", meaning: "उदास", example: "Why are you sad?" },
        { word: "Beautiful", meaning: "सुंदर", example: "She is beautiful." },
        { word: "Ugly", meaning: "बदसूरत", example: "This building is ugly." },
        { word: "Easy", meaning: "आसान", example: "This question is easy." },
        { word: "Difficult", meaning: "मुश्किल", example: "Math is difficult for me." },
        { word: "Fast", meaning: "तेज़", example: "He runs very fast." },
        { word: "Slow", meaning: "धीमा", example: "The computer is slow today." },
        { word: "New", meaning: "नया", example: "I bought a new phone." },
        { word: "Old", meaning: "पुराना", example: "This is an old book." }
        // ... more words up to 1000
    ],
    A2: [
        { word: "Actually", meaning: "वास्तव में", example: "Actually, I don't know." },
        { word: "Adventure", meaning: "साहसिक कार्य", example: "We love adventure trips." },
        { word: "Agree", meaning: "सहमत होना", example: "I agree with you." },
        { word: "Allow", meaning: "अनुमति देना", example: "My parents allow me to go." },
        { word: "Amazing", meaning: "अद्भुत", example: "The view is amazing." },
        { word: "Angry", meaning: "गुस्सा", example: "Don't be angry with me." },
        { word: "Annoy", meaning: "परेशान करना", example: "Loud noise annoys me." },
        { word: "Answer", meaning: "जवाब", example: "Please answer my question." },
        { word: "Anxious", meaning: "चिंतित", example: "I am anxious about exam." },
        { word: "Apologize", meaning: "माफी मांगना", example: "You should apologize." },
        { word: "Appear", meaning: "दिखाई देना", example: "He appeared suddenly." },
        { word: "Arrange", meaning: "व्यवस्थित करना", example: "Let's arrange a meeting." },
        { word: "Arrive", meaning: "पहुंचना", example: "When will you arrive?" },
        { word: "Ask", meaning: "पूछना", example: "Can I ask you something?" },
        { word: "Avoid", meaning: "टालना", example: "Try to avoid mistakes." }
        // ... more words up to 1200
    ]
    // ... similar data for other levels
};

// Load vocabulary based on selected level
function loadVocabulary() {
    const level = document.getElementById('level-select').value;
    currentVocabulary = vocabularyData[level] || vocabularyData.A1;
    filteredVocabulary = [...currentVocabulary];
    currentVocabularyPage = 1;
    renderVocabulary();
    updatePagination();
}

// Render vocabulary cards
function renderVocabulary() {
    const grid = document.getElementById('vocabulary-grid');
    const startIndex = (currentVocabularyPage - 1) * wordsPerPage;
    const endIndex = startIndex + wordsPerPage;
    const wordsToShow = filteredVocabulary.slice(startIndex, endIndex);
    
    grid.innerHTML = '';
    
    wordsToShow.forEach((wordObj, index) => {
        const card = document.createElement('div');
        card.className = 'vocab-card';
        card.innerHTML = `
            <div class="vocab-word">${wordObj.word}</div>
            <div class="vocab-meaning">${wordObj.meaning}</div>
            <div class="vocab-example">${wordObj.example}</div>
            <div class="vocab-actions">
                <button class="vocab-btn btn-audio" onclick="playAudio('${wordObj.word}')">
                    <i class="fas fa-volume-up"></i> Audio
                </button>
                <button class="vocab-btn btn-bookmark" onclick="bookmarkWord('${wordObj.word}')">
                    <i class="fas fa-bookmark"></i> Save
                </button>
            </div>
        `;
        grid.appendChild(card);
    });
}

// Search vocabulary
function searchVocabulary() {
    const searchTerm = document.getElementById('vocab-search').value.toLowerCase();
    
    if (searchTerm.trim() === '') {
        filteredVocabulary = [...currentVocabulary];
    } else {
        filteredVocabulary = currentVocabulary.filter(wordObj => 
            wordObj.word.toLowerCase().includes(searchTerm) ||
            wordObj.meaning.toLowerCase().includes(searchTerm) ||
            wordObj.example.toLowerCase().includes(searchTerm)
        );
    }
    
    currentVocabularyPage = 1;
    renderVocabulary();
    updatePagination();
}

// Pagination functions
function previousVocabularyPage() {
    if (currentVocabularyPage > 1) {
        currentVocabularyPage--;
        renderVocabulary();
        updatePagination();
    }
}

function nextVocabularyPage() {
    const totalPages = Math.ceil(filteredVocabulary.length / wordsPerPage);
    if (currentVocabularyPage < totalPages) {
        currentVocabularyPage++;
        renderVocabulary();
        updatePagination();
    }
}

function updatePagination() {
    const totalPages = Math.ceil(filteredVocabulary.length / wordsPerPage);
    document.getElementById('page-info').textContent = `Page ${currentVocabularyPage} of ${totalPages}`;
    
    document.getElementById('prev-page').disabled = currentVocabularyPage === 1;
    document.getElementById('next-page').disabled = currentVocabularyPage === totalPages;
}

// Play word audio
function playAudio(word) {
    // In real implementation, use Web Speech API or pre-recorded audio
    const utterance = new SpeechSynthesisUtterance(word);
    utterance.lang = 'en-US';
    utterance.rate = 0.8;
    speechSynthesis.speak(utterance);
    
    showNotification(`Playing audio for: ${word}`, 'success');
}

// Bookmark word
function bookmarkWord(word) {
    const user = JSON.parse(localStorage.getItem('englishMasterUser')) || {};
    user.bookmarks = user.bookmarks || [];
    
    if (!user.bookmarks.includes(word)) {
        user.bookmarks.push(word);
        localStorage.setItem('englishMasterUser', JSON.stringify(user));
        showNotification(`"${word}" added to bookmarks!`, 'success');
    } else {
        showNotification(`"${word}" is already bookmarked!`, 'error');
    }
}
// Progress Tracking System

// Initialize progress tracking
function initializeProgressTracking() {
    const user = JSON.parse(localStorage.getItem('englishMasterUser')) || {};
    
    if (!user.progress) {
        user.progress = {
            vocabulary: 0,
            grammar: 0,
            listening: 0,
            speaking: 0,
            reading: 0,
            writing: 0,
            streak: 0,
            lastActive: new Date().toISOString()
        };
        localStorage.setItem('englishMasterUser', JSON.stringify(user));
    }
    
    updateStreak();
    updateProgressDisplay();
}

// Update learning streak
function updateStreak() {
    const user = JSON.parse(localStorage.getItem('englishMasterUser')) || {};
    const today = new Date().toDateString();
    const lastActive = user.progress ? new Date(user.progress.lastActive).toDateString() : null;
    
    if (lastActive === today) {
        return; // Already updated today
    }
    
    const yesterday = new Date();
    yesterday.setDate(yesterday.getDate() - 1);
    
    if (lastActive === yesterday.toDateString()) {
        user.progress.streak = (user.progress.streak || 0) + 1;
    } else if (lastActive !== today) {
        user.progress.streak = 1; // Reset streak
    }
    
    user.progress.lastActive = new Date().toISOString();
    localStorage.setItem('englishMasterUser', JSON.stringify(user));
}

// Track vocabulary learning
function trackVocabularyProgress(wordsLearned) {
    const user = JSON.parse(localStorage.getItem('englishMasterUser')) || {};
    user.progress = user.progress || {};
    user.progress.vocabulary = (user.progress.vocabulary || 0) + wordsLearned;
    localStorage.setItem('englishMasterUser', JSON.stringify(user));
    updateProgressDisplay();
}

// Track grammar progress
function trackGrammarProgress(topicsCompleted) {
    const user = JSON.parse(localStorage.getItem('englishMasterUser')) || {};
    user.progress = user.progress || {};
    user.progress.grammar = (user.progress.grammar || 0) + topicsCompleted;
    localStorage.setItem('englishMasterUser', JSON.stringify(user));
    updateProgressDisplay();
}

// Get level progress
function getLevelProgress(level) {
    const user = JSON.parse(localStorage.getItem('englishMasterUser')) || {};
    const progress = user.progress || {};
    
    const levelRequirements = {
        A1: { vocabulary: 200, grammar: 10 },
        A2: { vocabulary: 400, grammar: 20 },
        B1: { vocabulary: 600, grammar: 30 },
        B2: { vocabulary: 800, grammar: 40 },
        C1: { vocabulary: 1000, grammar: 50 },
        C2: { vocabulary: 1200, grammar: 60 }
    };
    
    const requirements = levelRequirements[level] || levelRequirements.A1;
    const vocabProgress = Math.min(100, Math.round((progress.vocabulary || 0) / requirements.vocabulary * 100));
    const grammarProgress = Math.min(100, Math.round((progress.grammar || 0) / requirements.grammar * 100));
    
    return {
        vocabulary: vocabProgress,
        grammar: grammarProgress,
        overall: Math.round((vocabProgress + grammarProgress) / 2)
    };
}

// Generate progress report
function generateProgressReport() {
    const user = JSON.parse(localStorage.getItem('englishMasterUser')) || {};
    const progress = user.progress || {};
    const currentLevel = user.currentLevel || 'A1';
    
    const levelProgress = getLevelProgress(currentLevel);
    
    return {
        currentLevel: currentLevel,
        vocabulary: {
            learned: progress.vocabulary || 0,
            progress: levelProgress.vocabulary
        },
        grammar: {
            completed: progress.grammar || 0,
            progress: levelProgress.grammar
        },
        streak: progress.streak || 0,
        overallProgress: levelProgress.overall,
        nextLevel: getNextLevel(currentLevel)
    };
}

// Get next level
function getNextLevel(currentLevel) {
    const levels = ['A1', 'A2', 'B1', 'B2', 'C1', 'C2'];
    const currentIndex = levels.indexOf(currentLevel);
    return currentIndex < levels.length - 1 ? levels[currentIndex + 1] : null;
}

// Check level up
function checkLevelUp() {
    const user = JSON.parse(localStorage.getItem('englishMasterUser')) || {};
    const currentLevel = user.currentLevel || 'A1';
    const progress = getLevelProgress(currentLevel);
    
    if (progress.overall >= 80) {
        const nextLevel = getNextLevel(currentLevel);
        if (nextLevel) {
            showNotification(`Congratulations! You're ready for ${nextLevel} level!`, 'success');
            return true;
        }
    }
    return false;
}

// Export progress data
function exportProgressData() {
    const report = generateProgressReport();
    const dataStr = JSON.stringify(report, null, 2);
    const dataBlob = new Blob([dataStr], { type: 'application/json' });
    
    const link = document.createElement('a');
    link.href = URL.createObjectURL(dataBlob);
    link.download = 'english-progress-report.json';
    link.click();
}

// Initialize when page loads
document.addEventListener('DOMContentLoaded', function() {
    initializeProgressTracking();
    
    // Check for level up every 5 minutes
    setInterval(checkLevelUp, 300000);
});
/* Additional Responsive Styles */

@media (max-width: 1024px) {
    .hero-content h1 {
        font-size: 2.5rem;
    }
    
    .levels-grid {
        grid-template-columns: repeat(2, 1fr);
    }
    
    .grammar-container {
        grid-template-columns: 250px 1fr;
    }
    
    .progress-dashboard {
        grid-template-columns: 1fr;
    }
}

@media (max-width: 768px) {
    .nav-container {
        padding: 0 15px;
    }
    
    .hero {
        padding: 100px 0 60px;
    }
    
    .hero-content h1 {
        font-size: 2rem;
    }
    
    .hero-stats {
        flex-direction: column;
        gap: 1rem;
    }
    
    .levels-grid {
        grid-template-columns: 1fr;
    }
    
    .grammar-container {
        grid-template-columns: 1fr;
    }
    
    .vocabulary-grid {
        grid-template-columns: 1fr;
    }
    
    .practice-grid {
        grid-template-columns: 1fr;
    }
    
    .footer-content {
        grid-template-columns: 1fr;
        gap: 2rem;
    }
    
    .level-stats {
        flex-direction: column;
        gap: 1rem;
    }
    
    .stat-item {
        flex-direction: row;
        justify-content: flex-start;
        gap: 10px;
    }
}

@media (max-width: 480px) {
    .container {
        padding: 0 15px;
    }
    
    .hero-container {
        padding: 0 15px;
    }
    
    .hero-content h1 {
        font-size: 1.8rem;
    }
    
    .hero-content p {
        font-size: 1rem;
    }
    
    .section-title {
        font-size: 2rem;
    }
    
    .level-header {
        flex-direction: column;
        gap: 1rem;
        text-align: center;
    }
    
    .vocabulary-controls {
        flex-direction: column;
    }
    
    .search-box {
        width: 100%;
    }
    
    .progress-stats {
        grid-template-columns: 1fr;
    }
    
    .example-item {
        flex-direction: column;
        gap: 5px;
    }
    
    .options {
        flex-direction: column;
    }
    
    .btn-primary, .btn-secondary {
        padding: 10px 20px;
        font-size: 1rem;
    }
}

/* Mobile Navigation */
.mobile-menu-btn {
    display: none;
    background: none;
    border: none;
    font-size: 1.5rem;
    cursor: pointer;
    color: var(--text-primary);
}

@media (max-width: 768px) {
    .mobile-menu-btn {
        display: block;
    }
    
    .nav-menu {
        position: fixed;
        top: 70px;
        left: -100%;
        width: 100%;
        height: calc(100vh - 70px);
        background: var(--bg-white);
        flex-direction: column;
        align-items: center;
        justify-content: flex-start;
        padding-top: 2rem;
        transition: left 0.3s ease;
        box-shadow: var(--shadow-lg);
    }
    
    .nav-menu.active {
        left: 0;
    }
    
    .nav-link {
        padding: 1rem 0;
        font-size: 1.1rem;
    }
}

/* Touch device improvements */
@media (hover: none) and (pointer: coarse) {
    .btn-level, .btn-practice, .option-btn {
        min-height: 44px;
        min-width: 44px;
    }
    
    .vocab-card {
        padding: 1rem;
    }
    
    .level-card {
        margin: 0.5rem;
    }
}

/* High contrast mode support */
@media (prefers-contrast: high) {
    :root {
        --primary-color: #0000ff;
        --text-primary: #000000;
        --border-color: #000000;
    }
    
    .level-card, .grammar-sidebar, .vocab-card {
        border: 2px solid var(--border-color);
    }
}

/* Reduced motion support */
@media (prefers-reduced-motion: reduce) {
    * {
        animation-duration: 0.01ms !important;
        animation-iteration-count: 1 !important;
        transition-duration: 0.01ms !important;
    }
    
    .hero-image img {
        animation: none;
    }
}

/* Dark mode support */
@media (prefers-color-scheme: dark) {
    :root {
        --text-primary: #f9fafb;
        --text-secondary: #d1d5db;
        --bg-light: #1f2937;
        --bg-white: #374151;
        --border-color: #4b5563;
    }
    
    body {
        background: #111827;
        color: var(--text-primary);
    }
    
    .level-card, .grammar-sidebar, .grammar-content, 
    .vocab-card, .practice-card, .progress-card {
        background: var(--bg-white);
        border-color: var(--border-color);
    }
    
    .hindi-explanation, .examples, .practice-section {
        background: var(--bg-light);
    }
}

/* Print styles */
@media print {
    .navbar, .hero, .footer, .btn-level, .btn-practice {
        display: none !important;
    }
    
    .levels, .grammar, .vocabulary, .practice, .progress {
        padding: 20px 0 !important;
    }
    
    .level-card, .vocab-card {
        break-inside: avoid;
        box-shadow: none !important;
        border: 1px solid #000 !important;
    }
}
# Using Python
python -m http.server 8000

# Using Node.js
npx http-server

# Using PHP
php -S localhost:8000 

# Sanjuonlinetool
Online Tools 2025
<style>
    /* Base Styles */
    * {
        margin: 0;
        padding: 0;
        box-sizing: border-box;
        font-family: 'Segoe UI', sans-serif;
    }

    body {
        background: #0B0C10;
        color: #C5C6C7;
        line-height: 1.6;
    }

    /* Header Styles */
    .header {
        background: rgba(31, 40, 51, 0.9); /* Transparent background */
        padding: 1.5rem;
        display: flex;
        justify-content: space-between;
        align-items: center;
        animation: fadeInDown 1s;
    }

    .logo {
        display: flex;
        align-items: center;
        cursor: pointer;
        transition: transform 0.3s ease;
    }

    .logo:hover {
        transform: scale(1.05);
    }

    .logo-circle {
        width: 50px;
        height: 50px;
        background: linear-gradient(135deg, rgba(102, 252, 241, 0.9), rgba(69, 162, 158, 0.9)); /* Transparent gradient */
        border-radius: 50%;
        display: flex;
        justify-content: center;
        align-items: center;
        margin-right: 1rem;
    }

    .logo-circle span {
        font-size: 1.5rem;
        font-weight: bold;
        color: #1F2833;
    }

    .header h1 {
        color: #66FCF1;
        font-size: 2rem;
        text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
    }

    /* Navigation Styles */
    .toolbar {
        display: flex;
        align-items: center;
        gap: 1rem;
    }

    .nav-links {
        display: flex;
        gap: 1.5rem;
        list-style: none;
    }

    .nav-links a {
        color: #C5C6C7;
        text-decoration: none;
        padding: 0.5rem 1rem;
        border-radius: 25px;
        transition: all 0.3s ease;
        background: rgba(31, 40, 51, 0.7); /* Transparent background */
    }

    .nav-links a:hover {
        background: rgba(102, 252, 241, 0.9); /* Transparent hover background */
        color: #1F2833;
        transform: translateY(-2px);
    }

    /* Toggle Button */
    .toggle-button {
        background: rgba(102, 252, 241, 0.9); /* Transparent background */
        color: #1F2833;
        border: none;
        padding: 0.5rem 1rem;
        border-radius: 25px;
        cursor: pointer;
        font-size: 0.9rem;
        transition: all 0.3s ease;
    }

    .toggle-button:hover {
        background: rgba(69, 162, 158, 0.9); /* Transparent hover background */
        transform: translateY(-2px);
    }

    /* Hero Section */
    .hero {
        background: rgba(31, 40, 51, 0.8); /* Transparent background */
        padding: 4rem 2rem;
        text-align: center;
        color: #C5C6C7;
        border-radius: 10px;
        margin: 2rem auto;
        max-width: 1200px;
        animation: fadeIn 1.5s ease;
    }

    .hero h2 {
        font-size: 2.5rem;
        margin-bottom: 1rem;
        color: #66FCF1;
    }

    .hero p {
        font-size: 1.2rem;
        margin-bottom: 2rem;
    }

    .hero .cta-button {
        background: rgba(102, 252, 241, 0.9); /* Transparent background */
        color: #1F2833;
        border: none;
        padding: 1rem 2rem;
        border-radius: 25px;
        font-size: 1rem;
        cursor: pointer;
        transition: all 0.3s ease;
    }

    .hero .cta-button:hover {
        background: rgba(69, 162, 158, 0.9); /* Transparent hover background */
        transform: translateY(-2px);
    }

    /* Button Grid */
    .button-grid {
        display: grid;
        grid-template-columns: repeat(2, 1fr);
        gap: 1.5rem;
        padding: 2rem 0;
    }

    .design-button {
        background: rgba(31, 40, 51, 0.8); /* Transparent background */
        border: 2px solid #66FCF1;
        padding: 1.5rem;
        border-radius: 10px;
        color: #C5C6C7;
        font-size: 1.1rem;
        cursor: pointer;
        transition: all 0.3s ease;
        position: relative;
        overflow: hidden;
    }

    .design-button:hover {
        background: rgba(102, 252, 241, 0.9); /* Transparent hover background */
        color: #1F2833;
        transform: translateY(-5px);
        box-shadow: 0 10px 20px rgba(102, 252, 241, 0.3);
    }

    /* Footer Styles */
    .footer {
        background: rgba(31, 40, 51, 0.9); /* Transparent background */
        padding: 2rem 1rem;
        margin-top: 2rem;
        text-align: center;
        color: #C5C6C7;
        border-top: 2px solid #66FCF1;
    }

    .footer-links {
        display: flex;
        justify-content: center;
        gap: 1.5rem;
        margin-bottom: 1rem;
    }

    .footer-links a {
        color: #C5C6C7;
        text-decoration: none;
        transition: all 0.3s ease;
    }

    .footer-links a:hover {
        color: #66FCF1;
        transform: translateY(-2px);
    }

    .social-icons {
        display: flex;
        justify-content: center;
        gap: 1rem;
        margin-top: 1rem;
    }

    .social-icons a {
        color: #C5C6C7;
        font-size: 1.5rem;
        transition: all 0.3s ease;
    }

    .social-icons a:hover {
        color: #66FCF1;
        transform: translateY(-2px);
    }

    /* Animations */
    @keyframes fadeInDown {
        from {
            opacity: 0;
            transform: translateY(-20px);
        }
        to {
            opacity: 1;
            transform: translateY(0);
        }
    }

    @keyframes fadeIn {
        from { opacity: 0; }
        to { opacity: 1; }
    }

    @keyframes fadeInUp {
        from {
            opacity: 0;
            transform: translateY(20px);
        }
        to {
            opacity: 1;
            transform: translateY(0);
        }
    }

    /* Responsive Design */
    @media (max-width: 768px) {
        .button-grid {
            grid-template-columns: 1fr;
        }

        .header {
            flex-direction: column;
            align-items: flex-start;
        }

        .toolbar {
            flex-direction: column;
            align-items: flex-start;
            width: 100%;
            margin-top: 1rem;
        }

        .nav-links {
            flex-direction: column;
            gap: 1rem;
            width: 100%;
        }

        .nav-links a {
            width: 100%;
            text-align: center;
        }

        .toggle-button {
            width: 100%;
            margin-top: 1rem;
        }

        .hero {
            padding: 2rem 1rem;
        }

        .hero h2 {
            font-size: 2rem;
        }

        .hero p {
            font-size: 1rem;
        }

        .footer-links {
            flex-direction: column;
            gap: 1rem;
        }
    }
</style>

<div class="header">
    <div class="logo">
        <div class="logo-circle">
            <span>SO</span>
        </div>
        <h1>Sanju Online Tool</h1>
    </div>
    <div class="toolbar">
        <ul class="nav-links">
            <li><a href="#home">Home</a></li>
            <li><a href="#about">About</a></li>
            <li><a href="#services">Services</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
        <button class="toggle-button">Toggle Dark Mode</button>
    </div>
</div>

<!-- Hero Section -->
<div class="hero">
    <h2>Welcome to Sanju Online Tool</h2>
    <p>Your All-in-One Online Tool Hub for Productivity and Creativity!</p>
    <button class="cta-button">Explore Tools</button>
</div>

<div class="container">
    <div class="button-grid" id="buttonContainer">
        <!-- Buttons will be generated dynamically -->
    </div>
</div>

<!-- Footer -->
<div class="footer">
    <div class="footer-links">
        <a href="#home">Home</a>
        <a href="#about">About</a>
        <a href="#services">Services</a>
        <a href="#contact">Contact</a>
    </div>
    <div class="social-icons">
        <a href="https://facebook.com" target="_blank">&#xf09a;</a> <!-- Facebook Icon -->
        <a href="https://twitter.com" target="_blank">&#xf099;</a> <!-- Twitter Icon -->
        <a href="https://linkedin.com" target="_blank">&#xf0e1;</a> <!-- LinkedIn Icon -->
        <a href="https://instagram.com" target="_blank">&#xf16d;</a> <!-- Instagram Icon -->
    </div>
    <p>&copy; 2025 Sanju Online Tool. All rights reserved.</p>
</div>

<script>
    // Generate dynamic buttons with links
    const buttonContainer = document.getElementById('buttonContainer');
    const buttonNames = [
        "Design 1", "Design 2", "Design 3", "Design 4", "Design 5",
        "Design 6", "Design 7", "Design 8", "Design 9", "Design 10",
        "Design 11", "Design 12", "Design 13", "Design 14", "Design 15",
        "Design 16", "Design 17", "Design 18", "Design 19", "Design 20"
    ];
    const buttonLinks = [
        "#", "#", "#", "#", "#", "#", "#", "#", "#", "#",
        "#", "#", "#", "#", "#", "#", "#", "#", "#", "#"
    ]; // Add your links here

    buttonNames.forEach((name, index) => {
        const button = document.createElement('button');
        button.className = 'design-button';
        button.innerHTML = name;
        button.style.animation = `fadeInUp 0.5s ease ${index * 0.1}s forwards`;
        button.addEventListener('click', () => {
            window.open(buttonLinks[index], '_blank');
        });
        buttonContainer.appendChild(button);
    });

    // Dark/Light Mode Toggle
    const toggleButton = document.querySelector('.toggle-button');
    toggleButton.addEventListener('click', () => {
        document.body.classList.toggle('light-mode');
        toggleButton.textContent = document.body.classList.contains('light-mode') ? 'Toggle Dark Mode' : 'Toggle Light Mode';
    });

    // Smooth scrolling
    document.querySelectorAll('a[href^="#"]').forEach(anchor => {
        anchor.addEventListener('click', function (e) {
            e.preventDefault();
            document.querySelector(this.getAttribute('href')).scrollIntoView({
                behavior: 'smooth'
            });
        });
    });
</script>

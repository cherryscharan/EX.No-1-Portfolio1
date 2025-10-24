# Name: Charan kumar s
# Reg.no: 212223220015


# Ex01 Portfolio
## Date:

## AIM
To create a Portfolio using HTML and CSS.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for introduction, about, projects, and contact details.

### STEP 5
Define global styles for fonts, colors, and layout.

### STEP 6
Style the header, navigation bar, and sections.

### STEP 7
Use Flexbox or CSS Grid for layout design.

### STEP 8
Add hover effects and transitions for interactivity.

### STEP 9
Add Images and Media.

### STEP 10
Use optimized images for a professional look.

### STEP 11
Open the HTML file in a browser to check layout and functionality.

### STEP 12
Fix styling issues and refine content placement.

### STEP 13
Deploy the Portfolio.

### STEP 14
Upload to GitHub Pages for free hosting.

## PROGRAM

HTML
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>charan kumar  | Portfolio</title>
    <link rel="stylesheet" href="style.css">

</head>
<body>
    <!-- Header / Navigation -->
    <header>
        <nav>
            <div class="logo">charan kumar</div>
            <ul id="nav-links">
                <li><a href="#about">About</a></li>
                <li><a href="#skills">Skills</a></li>
                <li><a href="#projects">Projects</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
            <div class="hamburger" onclick="toggleMenu()">☰</div>
        </nav>
    </header>

    <!-- Hero Section -->
    <section class="hero">
        <img src="c:\Users\admin\AppData\Local\Packages\5319275A.WhatsAppDesktop_cv1g1gvanyjgm\TempState\0771FC6F0F4B1D7D1BB73BBBE14E0E31\WhatsApp Image 2025-10-24 at 15.35.52_2c9a3dbb.jpg" alt="charan kumar" class="hero-img">
        <h1>Hello, I'm <span>charan kumar</span></h1>
        <p>Web Developer | Designer | Programmer</p>
        <a href="#contact" class="btn">Hire Me</a>
    </section>

    <!-- About Section -->
    <section id="about" class="about">
        <h2>About Me</h2>
        <p>Hello! I'm charan kumar, a passionate web developer who loves creating colorful, interactive, and modern websites. I focus on clean design and smooth user experience.</p>
    </section>

    <!-- Skills Section -->
    <section id="skills" class="skills">
        <h2>My Skills</h2>
        <div class="skill-container">
            <div class="skill">
                <h3>HTML</h3>
                <div class="bar"><div class="progress" style="width: 95%;">95%</div></div>
            </div>
            <div class="skill">
                <h3>CSS</h3>
                <div class="bar"><div class="progress" style="width: 90%;">90%</div></div>
            </div>
            <div class="skill">
                <h3>JavaScript</h3>
                <div class="bar"><div class="progress" style="width: 85%;">85%</div></div>
            </div>
            <div class="skill">
                <h3>React</h3>
                <div class="bar"><div class="progress" style="width: 75%;">75%</div></div>
            </div>
        </div>
    </section>

    <!-- Projects Section -->
    <section id="projects" class="projects">
        <h2>My Projects</h2>
        <div class="project-container">
            <div class="project-card">
                <h3>Portfolio Website</h3>
                <p>My personal portfolio project with colorful design.</p>
                <a href="#">View Project</a>
            </div>
            <div class="project-card">
                <h3>Weather App</h3>
                <p>Interactive weather app using JavaScript and APIs.</p>
                <a href="#">View Project</a>
            </div>
            <div class="project-card">
                <h3>Todo App</h3>
                <p>Task management app with animations and colorful UI.</p>
                <a href="#">View Project</a>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="contact">
        <h2>Contact Me</h2>
        <form id="contactForm">
            <input type="text" name="name" placeholder="Your Name" required>
            <input type="email" name="email" placeholder="Your Email" required>
            <textarea name="message" placeholder="Your Message" required></textarea>
            <button type="submit">Send Message</button>
        </form>
        <p id="success-msg">Message sent successfully!</p>
    </section>

    <!-- Footer -->
    <footer>
        <p>&copy; 2025 charan kumar. All Rights Reserved.</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>
```
## css
```
/* Global Reset */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Poppins', sans-serif;
}

/* Body */
body {
    background: linear-gradient(120deg, #860cf1, #f5576c);
    color: #fff;
    scroll-behavior: smooth;
}

/* Header */
header {
    background: rgba(0,0,0,0.6);
    position: sticky;
    top: 0;
    z-index: 100;
}

nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    max-width: 1000px;
    margin: auto;
    padding: 15px 20px;
}

nav .logo {
    font-size: 24px;
    font-weight: bold;
    color: #fff;
}

nav ul {
    list-style: none;
    display: flex;
}

nav ul li {
    margin-left: 20px;
}

nav ul li a {
    text-decoration: none;
    color: #fff;
    font-weight: 500;
    transition: 0.3s;
}

nav ul li a:hover {
    color: #ffeb3b;
}

.hamburger {
    display: none;
    font-size: 28px;
    cursor: pointer;
}

/* Hero Section */
.hero {
    text-align: center;
    padding: 120px 20px;
}

.hero-img {
    width: 160px;
    border-radius: 50%;
    border: 5px solid #fff;
    margin-bottom: 20px;
    box-shadow: 0px 0px 20px rgba(0,0,0,0.5);
    transition: transform 0.3s;
}

.hero-img:hover {
    transform: scale(1.1);
}

.hero h1 span {
    color: #ffeb3b;
}

.hero .btn {
    display: inline-block;
    margin-top: 20px;
    padding: 12px 30px;
    background: #ffeb3b;
    color: #333;
    font-weight: bold;
    text-decoration: none;
    border-radius: 30px;
    box-shadow: 0px 5px 15px rgba(0,0,0,0.3);
    transition: transform 0.3s;
}

.hero .btn:hover {
    transform: translateY(-5px);
}

/* Sections */
section {
    padding: 60px 20px;
    max-width: 1000px;
    margin: auto;
}

section h2 {
    text-align: center;
    margin-bottom: 40px;
    font-size: 32px;
    text-shadow: 2px 2px rgba(0,0,0,0.3);
}

/* Skills */
.skill-container {
    display: flex;
    flex-direction: column;
    gap: 25px;
    max-width: 600px;
    margin: auto;
}

.skill h3 {
    margin-bottom: 8px;
}

.bar {
    background: rgba(255,255,255,0.2);
    border-radius: 30px;
    overflow: hidden;
}

.progress {
    background: #fff;
    color: #333;
    padding: 5px;
    text-align: right;
    border-radius: 30px;
    font-weight: bold;
    transition: width 1s ease-in-out;
}

/* Projects */
.project-container {
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
    justify-content: center;
}

.project-card {
    background: rgba(255,255,255,0.2);
    padding: 20px;
    border-radius: 15px;
    flex: 1 1 250px;
    max-width: 300px;
    text-align: center;
    transition: transform 0.3s, background 0.3s;
    backdrop-filter: blur(10px);
}

.project-card:hover {
    transform: translateY(-10px);
    background: rgba(255,255,255,0.4);
}

.project-card a {
    display: inline-block;
    margin-top: 12px;
    text-decoration: none;
    color: #ffeb3b;
    font-weight: bold;
}

/* Contact Form */
.contact form {
    display: flex;
    flex-direction: column;
    gap: 15px;
    max-width: 500px;
    margin: auto;
}

.contact input, 
.contact textarea {
    padding: 12px;
    border-radius: 15px;
    border: none;
    outline: none;
    font-size: 16px;
}

.contact button {
    padding: 12px;
    border-radius: 30px;
    border: none;
    background: #ffeb3b;
    color: #333;
    font-weight: bold;
    cursor: pointer;
    transition: transform 0.3s;
}

.contact button:hover {
    transform: translateY(-5px);
}

/* Success Message */
#success-msg {
    text-align: center;
    margin-top: 15px;
    display: none;
}

/* Footer */
footer {
    text-align: center;
    padding: 20px;
    background: rgba(0,0,0,0.6);
}

/* Responsive */
@media(max-width:768px){
    nav ul {
        display: none;
        flex-direction: column;
        gap: 10px;
        background: rgba(0,0,0,0.8);
        position: absolute;
        top: 60px;
        right: 20px;
        padding: 20px;
        border-radius: 10px;
    }
    nav ul.show {
        display: flex;
    }
    .hamburger {
        display: block;
    }
}
```


## OUTPUT
<img width="1822" height="1015" alt="Screenshot 2025-10-24 154031" src="https://github.com/user-attachments/assets/4305cfbd-5a33-40ed-b90b-aeab905984f2" />
<img width="1818" height="964" alt="Screenshot 2025-10-24 154125" src="https://github.com/user-attachments/assets/258c7711-711f-47cd-8f96-053704348156" />
<img width="1833" height="967" alt="Screenshot 2025-10-24 154106" src="https://github.com/user-attachments/assets/0a981fee-3a80-4bec-b9cb-7dbfaf21acdd" />




## RESULT
The program for creating Portfolio using HTML and CSS is executed successfully.

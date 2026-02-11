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
```
index.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Maleni M- Portfolio</title>
    <link rel="stylesheet" href="css/style.css">
</head>
<body>
    <header>
        <nav>
            <ul>
                <li><a href="index.html">Home</a></li>
                <li><a href="about.html">About</a></li>
                <li><a href="projects.html">Projects</a></li>
                <li><a href="contact.html">Contact</a></li>
            </ul>
        </nav>
    </header>
    <main>
        <section class="hero">
             <h1>Maleni M</h1>
            <p>3rd Year B.E. CSE | Web Dev & UI/UX | Chennai</p>
        </section>
    </main>
    <footer>&copy; 2026 Maleni Murugan. All rights reserved.</footer>
</body>
</html>

about.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>About - Maleni M</title>
    <link rel="stylesheet" href="css/style.css">
</head>
<body>
    <nav>
        <ul>
            <li><a href="index.html">Home</a></li>
            <li><a href="about.html">About</a></li>
            <li><a href="projects.html">Projects</a></li>
            <li><a href="contact.html">Contact</a></li>
        </ul>
    </nav>

    <section class="hero" style="background: var(--secondary-gradient); padding: 120px 20px 80px;">
        <h1>About Me</h1>
        <p>3rd Year B.E. CSE | Passionate Full-Stack Developer & UI/UX Designer</p>
    </section>

    <section class="container">
        <div style="max-width: 800px; margin: 0 auto; text-align: center;">
            <h2 style="background: var(--purple-gradient); -webkit-background-clip: text; -webkit-text-fill-color: transparent;">My Journey</h2>
            <p style="font-size: 1.2rem; color: #666; margin-bottom: 2rem;">
                Computer Science student from Chennai building modern web apps, IoT healthcare solutions, and pixel-perfect UI/UX designs. 
                Currently mastering React/Next.js, Tailwind CSS, Figma, and AWS Cloud.
            </p>
        </div>

        <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 2rem; margin-top: 4rem;">
            <div class="project-card" style="background: var(--dark-gradient); color: white; text-align: center; padding: 2rem;">
                <h3 style="color: #A8D5BA;">🎓 Education</h3>  <!-- Changed from #FFD93D -->
                <p>B.E. Computer Science & Engineering<br>Saveetha Engineering College<br>Expected 2027</p>
            </div>
            <div class="project-card" style="background: var(--primary-gradient); color: white; text-align: center; padding: 2rem;">
                <h3 style="color: #A8D5BA;">💻 Skills</h3>     <!-- Changed from #FFD93D -->
                <p>React, Next.js, Tailwind CSS<br>Figma, Firebase, AWS<br>GitHub, Netlify, VS Code</p>
            </div>
            <div class="project-card" style="background: var(--purple-gradient); color: white; text-align: center; padding: 2rem;">
                <h3 style="color: #A8D5BA;">🚀 Goals</h3>      <!-- Changed from #FFD93D -->
                <p>Frontend Developer Internships<br>Google, Microsoft, Startups<br>Full-Stack & UI/UX Roles</p>
            </div>
        </div>
    </section>

    <script>
        window.addEventListener('scroll', () => {
            document.querySelector('nav').classList.toggle('scrolled', window.scrollY > 50);
        });
    </script>
</body>
</html>

contact.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contact - Maleni Murugan</title>
    <link rel="stylesheet" href="css/style.css">
</head>
<body>
    <nav>
        <ul>
            <li><a href="index.html">Home</a></li>
            <li><a href="about.html">About</a></li>
            <li><a href="projects.html">Projects</a></li>
            <li><a href="contact.html">Contact</a></li>
        </ul>
    </nav>

    <section class="hero" style="background: var(--dark-gradient);">
        <h1>Get In Touch</h1>
        <p>Ready for internships & collaboration opportunities</p>
    </section>

    <section class="container">
        <div class="contact-form">
            <h2 style="text-align: center; margin-bottom: 2rem; color: #2c3e50;">Send Message</h2>
            <form>
                <div class="form-group">
                    <input type="text" placeholder="Your Name" required>
                </div>
                <div class="form-group">
                    <input type="email" placeholder="your@email.com" required>
                </div>
                <div class="form-group">
                    <textarea rows="6" placeholder="Tell me about your project or opportunity..." required></textarea>
                </div>
                <button type="submit" class="btn">Send Message</button>
            </form>
        </div>

        <div style="margin-top: 4rem; text-align: center;">
            <h3 style="color: #2c3e50; margin-bottom: 1rem;">Or Reach Me Directly</h3>
            <p style="font-size: 1.1rem; color: #666;">
                📧 malenimurugan@email.com<br>
                💼 LinkedIn: <a href="#" style="color: #4ECDC4;">MALENIMURUGAN</a><br>
                💻 GitHub: <a href="#" style="color: #4ECDC4;">MALENIMURUGAN</a><br>
                📍 Chennai, Tamil Nadu, India.
            </p>
        </div>
    </section>

    <script>
        window.addEventListener('scroll', () => {
            document.querySelector('nav').classList.toggle('scrolled', window.scrollY > 50);
        });
    </script>
</body>
</html>

projects.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Projects - Maleni M</title>
    <link rel="stylesheet" href="css/style.css">
</head>
<body>
    <nav>
        <ul>
            <li><a href="index.html">Home</a></li>
            <li><a href="about.html">About</a></li>
            <li><a href="projects.html">Projects</a></li>
            <li><a href="contact.html">Contact</a></li>
        </ul>
    </nav>

    <section class="hero" style="background: var(--purple-gradient);">
        <h1>My Projects</h1>
        <p>Real-world applications built with modern technologies</p>
    </section>

    <section class="container">
        <h2 style="text-align: center; margin-bottom: 4rem;">Featured Work</h2>
        <div class="projects-grid">
            <div class="project-card">
                <div class="card-content">
                    <h3>E-Commerce Website</h3>
                    <p>Full-stack Next.js application with responsive design, cart functionality, and Netlify deployment.</p>
                    <a href="#" class="btn" style="margin-top: 1rem; display: inline-block;">Live Demo →</a>
                </div>
            </div>

            <div class="project-card">
                <div class="card-content">
                    <h3>Online Notes App</h3>
                    <p>React + Firebase real-time notes application with user authentication and CRUD operations.</p>
                    <a href="#" class="btn" style="margin-top: 1rem; display: inline-block;">Live Demo →</a>
                </div>
            </div>

            <div class="project-card">
                <div class="card-content">
                    <h3>Healthcare IoT System</h3>
                    <p>IoT sensors monitoring vital signs with AWS cloud integration and real-time data dashboard.</p>
                    <a href="#" class="btn" style="margin-top: 1rem; display: inline-block;">View Project →</a>
                </div>
            </div>
        </div>
    </section>

    <script>
        window.addEventListener('scroll', () => {
            document.querySelector('nav').classList.toggle('scrolled', window.scrollY > 50);
        });
    </script>
</body>
</html>

style.css
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap');

* { margin: 0; padding: 0; box-sizing: border-box; }
body { 
    font-family: 'Poppins', sans-serif; 
    line-height: 1.6; 
    color: #333; 
    overflow-x: hidden;
}

:root {
    --primary-gradient: linear-gradient(45deg, #FF6B6B, #4ECDC4);
    --secondary-gradient: linear-gradient(45deg, #FFD93D, #FF8E8E);
    --dark-gradient: linear-gradient(45deg, #2C3E50, #3498DB);
    --purple-gradient: linear-gradient(45deg, #8E44AD, #E91E63);
}

/* Navigation */
nav { 
    background: rgba(255,255,255,0.95); 
    backdrop-filter: blur(10px); 
    position: fixed; 
    width: 100%; 
    top: 0; 
    z-index: 1000; 
    box-shadow: 0 2px 20px rgba(0,0,0,0.1);
    transition: all 0.3s ease;
}
nav.scrolled { background: rgba(255,255,255,0.98); box-shadow: 0 4px 30px rgba(0,0,0,0.2); }
nav ul { 
    display: flex; 
    justify-content: center; 
    list-style: none; 
    padding: 1rem 0; 
}
nav li { margin: 0 1.5rem; }
nav a { 
    color: #333; 
    text-decoration: none; 
    padding: 0.8rem 1.5rem; 
    border-radius: 50px; 
    font-weight: 500; 
    transition: all 0.3s ease;
    position: relative;
    overflow: hidden;
}
nav a::before {
    content: ''; 
    position: absolute; 
    top: 0; left: -100%; 
    width: 100%; height: 100%; 
    background: var(--primary-gradient); 
    transition: left 0.3s;
    z-index: -1;
}
nav a:hover::before { left: 0; }
nav a:hover { color: white; transform: translateY(-2px); }

/* Hero Section */
.hero { 
    background: var(--primary-gradient); 
    color: white; 
    text-align: center; 
    padding: 150px 20px 100px; 
    clip-path: polygon(0 0, 100% 0, 100% 85%, 0 100%);
}
.hero h1 { 
    font-size: clamp(2.5rem, 5vw, 4rem); 
    margin-bottom: 1rem; 
    animation: fadeInUp 1s ease;
}
.hero p { 
    font-size: 1.3rem; 
    margin-bottom: 2rem; 
    opacity: 0.9;
    animation: fadeInUp 1s ease 0.2s both;
}
.profile-img { 
    width: 200px; height: 200px; 
    border-radius: 50%; 
    border: 5px solid rgba(255,255,255,0.3); 
    box-shadow: 0 20px 40px rgba(0,0,0,0.3);
    animation: float 3s ease-in-out infinite;
}

/* Sections */
.container { max-width: 1200px; margin: 0 auto; padding: 0 20px; }
section { padding: 100px 0; }
h2 { 
    font-size: 2.5rem; 
    text-align: center; 
    margin-bottom: 3rem; 
    background: var(--secondary-gradient); 
    -webkit-background-clip: text; 
    -webkit-text-fill-color: transparent; 
    background-clip: text;
}

/* Projects Grid */
.projects-grid { 
    display: grid; 
    grid-template-columns: repeat(auto-fit, minmax(350px, 1fr)); 
    gap: 2rem; 
}
.project-card { 
    background: white; 
    border-radius: 20px; 
    overflow: hidden; 
    box-shadow: 0 20px 40px rgba(0,0,0,0.1); 
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    position: relative;
}
.project-card::before {
    content: ''; 
    position: absolute; 
    top: 0; left: 0; 
    right: 0; height: 4px; 
    background: var(--purple-gradient);
}
.project-card:hover { 
    transform: translateY(-15px) scale(1.02); 
    box-shadow: 0 30px 60px rgba(0,0,0,0.2);
}
.project-img { 
    width: 100%; 
    height: 220px; 
    object-fit: cover; 
    transition: transform 0.4s ease;
}
.project-card:hover .project-img { transform: scale(1.1); }
.card-content { padding: 2rem; }
.card-content h3 { color: #2c3e50; margin-bottom: 1rem; font-size: 1.4rem; }

/* Contact Form */
.contact-form { 
    max-width: 700px; 
    margin: 0 auto; 
    background: white; 
    padding: 3rem; 
    border-radius: 20px; 
    box-shadow: 0 20px 40px rgba(0,0,0,0.1);
}
.form-group { margin-bottom: 1.5rem; }
.form-group input, .form-group textarea { 
    width: 100%; 
    padding: 1rem 1.5rem; 
    border: 2px solid #e1e8ed; 
    border-radius: 12px; 
    font-family: inherit; 
    transition: all 0.3s ease;
    font-size: 1rem;
}
.form-group input:focus, .form-group textarea:focus { 
    outline: none; 
    border-color: #4ECDC4; 
    box-shadow: 0 0 0 3px rgba(78, 205, 196, 0.1);
}
.btn { 
    background: var(--primary-gradient); 
    color: white; 
    padding: 1rem 3rem; 
    border: none; 
    border-radius: 50px; 
    font-size: 1.1rem; 
    font-weight: 600; 
    cursor: pointer; 
    transition: all 0.3s ease;
    display: block; margin: 0 auto;
}
.btn:hover { transform: translateY(-3px); box-shadow: 0 10px 25px rgba(255,107,107,0.4); }

/* Animations */
@keyframes fadeInUp { from { opacity: 0; transform: translateY(30px); } to { opacity: 1; transform: translateY(0); } }
@keyframes float { 0%, 100% { transform: translateY(0px); } 50% { transform: translateY(-10px); } }

/* Responsive */
@media (max-width: 768px) { 
    nav ul { flex-direction: column; padding: 1.5rem 0; } 
    .hero { padding: 120px 20px 80px; } 
}

```


## OUTPUT
![alt text](<Screenshot 2026-02-11 160752.png>) ![alt text](<Screenshot 2026-02-11 161123.png>) ![alt text](<Screenshot 2026-02-11 161140.png>) ![alt text](<Screenshot 2026-02-11 161212.png>)
## RESULT
The program for creating Portfolio using HTML and CSS is executed successfully.

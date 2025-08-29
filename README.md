# Ex01 Portfolio
## Date:29-08-2025

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
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Portfolio | Mukesh Raj</title>
  <link rel="stylesheet" href="4.css">
</head>
<body>
  
  <header>
    <h1>Mukesh Raj</h1>
    <nav>
      <ul>
        <li><a href="#about">About</a></li>
        <li><a href="#projects">Projects</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </header>

  
  <section class="hero">
    <h2>Hi, I’m Mukesh Raj 👋</h2>
    <p>Web Developer | Designer | Problem Solver</p>
    <a href="#projects" class="btn">View My Work</a>
  </section>

  
  <section id="about" class="about">
    <h2>About Me</h2>
    <p>
      I'm a passionate web developer who enjoys building elegant, user-friendly,
      and responsive websites. Skilled in HTML, CSS, JavaScript, and exploring
      backend technologies. Always eager to learn and contribute to impactful projects.
    </p>
  </section>

  
  <section id="projects">
    <h2>Projects</h2>
    <div class="projects">
      <div class="project">
        <div class="content">
          <h3>Project One</h3>
          <p>A responsive portfolio site built with modern HTML, CSS, and JavaScript.</p>
        </div>
      </div>
      <div class="project">
        <div class="content">
          <h3>Project Two</h3>
          <p>A clean landing page design showcasing UI/UX best practices.</p>
        </div>
      </div>
      <div class="project">
        <div class="content">
          <h3>Project Three</h3>
          <p>A basic web app with interactive components and animations.</p>
        </div>
      </div>
    </div>
  </section>

  
  <section id="contact" class="contact">
    <h2>Contact Me</h2>
    <p>Let’s collaborate on your next project. Reach me here:</p>
    <a href="mailto:mukeshrajdhayanidhi2006@gmailcom">Email</a>
    <a href="#">LinkedIn</a>
    <a href="#">GitHub</a>
  </section>

  
  <footer>
    <p>&copy; 2025 Mukesh Raj | All Rights Reserved</p>
  </footer>
</body>
</html>

```
CSS
```

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: "Poppins", Arial, sans-serif;
  background: #f9f9f9;
  color: #333;
  line-height: 1.6;
}

a {
  text-decoration: none;
  color: inherit;
}

h1, h2, h3 {
  font-weight: 600;
  color: #222;
}


header {
  background: #111;
  color: #fff;
  padding: 20px 60px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  position: sticky;
  top: 0;
  z-index: 1000;
}

header h1 {
  font-size: 1.4rem;
  letter-spacing: 1px;
  color: #ff9800;
}

nav ul {
  list-style: none;
  display: flex;
  gap: 25px;
}

nav ul li a {
  color: #fff;
  font-weight: 500;
  transition: 0.3s;
}

nav ul li a:hover {
  color: #ff9800;
}


.hero {
  height: 70vh;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  background: linear-gradient(135deg, #ff9800, #e67e22);
  color: white;
  text-align: center;
  padding: 0 20px;
}

.hero h2 {
  font-size: 2.5rem;
  margin-bottom: 10px;
}

.hero p {
  font-size: 1.2rem;
  color: #f3f3f3;
}

.btn {
  display: inline-block;
  margin-top: 20px;
  padding: 12px 30px;
  border-radius: 30px;
  background: #fff;
  color: #ff9800;
  font-weight: 600;
  transition: background 0.3s, color 0.3s;
}

.btn:hover {
  background: #ff9800;
  color: white;
}


section {
  padding: 80px 60px;
  max-width: 1000px;
  margin: auto;
}

section h2 {
  text-align: center;
  margin-bottom: 40px;
  font-size: 2rem;
  color: #222;
  position: relative;
}

section h2::after {
  content: "";
  width: 80px;
  height: 3px;
  background: #ff9800;
  display: block;
  margin: 10px auto 0;
}


.about {
  text-align: center;
}

.about p {
  max-width: 700px;
  margin: auto;
  font-size: 1.05rem;
  color: #555;
}


.projects {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
  gap: 25px;
}

.project {
  background: white;
  border-radius: 12px;
  overflow: hidden;
  box-shadow: 0 4px 15px rgba(0,0,0,0.08);
  transition: transform 0.3s, box-shadow 0.3s;
}

.project:hover {
  transform: translateY(-8px);
  box-shadow: 0 6px 18px rgba(0,0,0,0.12);
}

.project .content {
  padding: 25px;
}

.project h3 {
  margin-bottom: 10px;
  color: #ff9800;
}

.project p {
  color: #555;
  font-size: 0.95rem;
}


.contact {
  text-align: center;
}

.contact p {
  margin-bottom: 20px;
  color: #555;
}

.contact a {
  display: inline-block;
  margin: 10px;
  padding: 12px 25px;
  border: 2px solid #ff9800;
  color: #ff9800;
  border-radius: 25px;
  transition: 0.3s;
  font-weight: 500;
}

.contact a:hover {
  background: #ff9800;
  color: white;
}


footer {
  background: #111;
  color: #aaa;
  text-align: center;
  padding: 25px;
  font-size: 0.9rem;
}

```

## OUTPUT
<img width="1920" height="1080" alt="Screenshot 2025-08-29 162544" src="https://github.com/user-attachments/assets/739528ce-6550-4442-a6ab-b4c6d69a3b69" />

<img width="1920" height="1080" alt="Screenshot 2025-08-29 162601" src="https://github.com/user-attachments/assets/11b5057b-42a8-490e-8ef8-2e53ec36a599" />
<img width="1920" height="1080" alt="Screenshot 2025-08-29 162612" src="https://github.com/user-attachments/assets/480fa63b-a850-4afe-b68a-5e763fdd7cba" />


## RESULT
The program for creating Portfolio using HTML and CSS is executed successfully.

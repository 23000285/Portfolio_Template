# PORTFOLIO

## AIM:
    To Create a Portfolio that exemplifies your beliefs, skills, qualifications, education, training, and experiences.

## WEBSITE REVIEW:

### Home Page:
#### HTML CODE:
```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Business Agency</title>
    <link rel="stylesheet" href="navigation.css">
</head>

<body>
    <header>
        <nav>
            <div class="logo">VENKAT</div>
            <ul class="nav-links">
                <li><a href="/Project/Portfolio_New/education/education.html">EDUCATION</a></li>
                <li><a href="/Project/Portfolio_New/skills/skills.html">SKILLS</a></li>
                <li><a href="/Project/Portfolio_New/experience/experience.html">EXPERIENCE</a></li>
                <li><a href="/Project/Portfolio_New/profile/profile.html">PROFILE</a></li>
                <li><a href="/Project/Portfolio_New/portfolio/portfolio.html">PORTFOLIO</a></li>
                <li><a href="/Project/Portfolio_New/client/clientsection.html">CLIENTS</a></li>
                <li><a href="/Project/Portfolio_New/contact/contactme.html">CONTACT</a></li>
            </ul>
            <div class="menu-toggle">&#9776;</div>
        </nav>
    </header>

    <section id="home">
        <div class="hero">
            <div class="overlay"></div>
            <div class="hero-text">
                <h1>HI, I AM <br> VENKAT</h1>
                <p>UI/UX DESIGNER AND WEB DEVELOPER</p>
                <a href="/Project/Portfolio_New/about/aboutme.html" class="btn">Download Resume</a>
            </div>
        </div>
    </section>

    <script>
        const menuToggle = document.querySelector('.menu-toggle');
        const navLinks = document.querySelector('.nav-links');

        menuToggle.addEventListener('click', () => {
            navLinks.classList.toggle('active');
        });
    </script>
</body>

</html>
```
#### CSS CODE:
```CSS
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Poppins', sans-serif;
}

body {
    background-color: #f8f9fc;
    text-align: center;
}

/* Navbar */
header nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px;
    background: #ffffff;
    color: black;
}

.nav-links {
    list-style: none;
    display: flex;
    gap: 30px;
}

.nav-links li a {
    color: #8c959f;
    text-decoration: none;
    font-weight: 600;
}

.logo {
    font-size: 24px;
    color: #b636ff;
    font-weight: bold;
}

/* Mobile Menu */
.menu-toggle {
    font-size: 30px;
    cursor: pointer;
    display: none;
}

/* Hero Section */
.hero {
    position: relative;
    height: 100vh;
    background: url('/Project/Portfolio_New/navigation/My profile 1.webp') no-repeat center center/cover;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    color: white;
}

.overlay {
    position: absolute;
    width: 100%;
    height: 100%;
    background: rgba(0, 0, 0, 0.6);
}

.hero-text {
    position: relative;
    z-index: 1;
}

.hero h1 {
    font-size: 3rem;
    margin-bottom: 10px;
    font-weight: bold;
}

.hero p {
    font-size: 1.2rem;
    margin-bottom: 20px;
}

.btn {
    padding: 10px 20px;
    background: #8c52ff;
    color: white;
    text-decoration: none;
    border-radius: 5px;
    font-weight: bold;
}

/* Responsive Design */
@media (max-width: 992px) {
    .nav-links {
        gap: 20px;
    }

    .hero h1 {
        font-size: 2.5rem;
    }

    .hero p {
        font-size: 1rem;
    }
}

@media (max-width: 768px) {
    nav {
        flex-direction: row;
        justify-content: space-between;
        align-items: center;
    }

    .menu-toggle {
        display: block;
    }

    .nav-links {
        display: none;
        flex-direction: column;
        position: absolute;
        top: 70px;
        right: 0;
        width: 100%;
        background: white;
        padding: 20px;
        text-align: center;
        box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.1);
    }

    .nav-links.active {
        display: flex;
    }

    .hero h1 {
        font-size: 2rem;
    }

    .hero p {
        font-size: 0.9rem;
    }

    .btn {
        padding: 8px 16px;
        font-size: 14px;
    }
}

@media (max-width: 480px) {
    .hero h1 {
        font-size: 1.8rem;
    }

    .hero p {
        font-size: 0.8rem;
    }

    .btn {
        padding: 6px 12px;
        font-size: 12px;
    }
}
```

### About me Page:
#### HTML CODE:
```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Business Agency</title>
    <link href="aboutme.css" rel="stylesheet">
</head>
<body>
    <h2>ABOUT ME</h2>
        <div class="about-container">
            <div class="about-content">
                <p class="bold-text">
                    I am a Professional UI/UX Designer and Web Developer.
                    <span class="highlight">Consectetur an adipisci elita, sed do eiusmod tempor incididunt ut labore et
                        dolore magna aliqua.</span>
                    Ut enim ad minim veniam quis nostrud.
                </p>
                <p>
                    Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla
                    pariatur.
                    Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id
                    est laborum.
                </p>
                <div class="about-info">
                    <span>Phone: 987-123-6547</span>
                    <span>Email: browny@info.com</span>
                    <span>Website: www.brownnine.com</span>
                </div>
            </div>

            <div class="profile-card">
                <img src="/about/My profile.jpg" alt="Profile Picture">
            </div>
        </div>
</body>
```

### CSS CODE:
```CSS
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Poppins', sans-serif;
}

body {
    background-color: #f8f9fc;
    text-align: center;
}

.about-container {
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 50px;
}

.about-content {
    width: 50%;
    padding-right: 50px;
}

.about-content h2 {
    text-transform: uppercase;
    text-align: left;
    margin-bottom: 10px;
    color: #333;
}

.about-content p {
    color: #555;
    line-height: 1.6;
}

.bold-text {
    font-weight: bold;
    color: #222;
}

.highlight {
    font-weight: bold;
    color: #2b2d42;
}

.about-info {
    margin-top: 20px;
    border-top: 1px solid #ccc;
    padding-top: 15px;
    display: flex;
    justify-content: space-between;
    color: #666;
    font-size: 14px;
}

.profile-card {
    width: 30%;
    background: white;
    text-align: center;
    box-shadow: 0px 5px 15px rgba(0, 0, 0, 0.1);
    border-radius: 10px;
    overflow: hidden;
}

.profile-card img {
    width: 100%;
    height: auto;
    display: block;
}
```
### OUTPUT:

### EDUCATION:
#### HTML CODE:
```HTML
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Business Agency</title>
    <link href="education.css" rel="stylesheet">
</head>

<body>
    <section>
        <h2>EDUCATION</h2>
        <div class="timeline">
            <div class="timeline-item1">
                <div class="top1">
                    <h3>2008 - 2010</h3>
                    <h4>Master of Computer Science</h4>
                </div>
            </div>
            <div class="timeline-item1">
                <div class="top1">
                    <h3>2004 - 2008</h3>
                    <h4>Bachelor of Computer Science</h4>
                </div>
            </div>
            <div class="timeline-item1">
                <div class="top1">
                    <h3>2004 - 2008</h3>
                    <h4>Bachelor of Creative Design</h4>
                </div>
            </div>
        </div>
            <div class="timeline">
                <div class="timeline-item">
                <div class="dot"></div>
                <div class="bottom">
                    <h4>UNIVERSITY OF NORTH CAROLINA</h4>
                    <p>North Carolina, USA</p>
                    <p>Pain itself is pain in being reprimanded in pleasure, wanting to be a hair of pain in the hope of nothing.</p>
                </div>
            </div>
            <div class="timeline-item">
                
                <div class="dot"></div>
                <div class="bottom">
                    <h4>UNIVERSITY OF NORTH CAROLINA</h4>
                    <p>North Carolina, USA</p>
                    <p>Pain itself is pain in being reprimanded in pleasure, wanting to be a hair of pain in the hope of nothing.</p>
                </div>
            </div>
            <div class="timeline-item">
            
                <div class="dot"></div>
                <div class="bottom">
                    <h4>UNIVERSITY OF BOLTON</h4>
                    <p>Bolton, United Kingdom</p>
                    <p>Pain itself is pain in being reprimanded in pleasure, wanting to be a hair of pain in the hope of nothing.</p>
                </div>
            </div>
    </section>
    
</body>
</html>
```
#### CSS CODE:
```CSS
body {
    margin: 0;
    font-family: Arial, sans-serif;
    scroll-behavior: smooth;
}

section {
    padding: 30px;
    text-align: center;
}

h2 {
    font-size: 22px;
    font-weight: bold;
    text-transform: uppercase;
    margin-bottom: 40px;
}

.timeline {
    display: flex;
    justify-content: space-between;
    align-items: flex-start;
    position: relative;
    border-top: 3px solid #ddd;
}

.timeline-item {
    width: 30%;
    position: relative;
    text-align: center;
    display: flex;
    flex-direction: column;
    align-items: center;
}

.timeline-item1 {
    width: 30%;
    position: relative;
    text-align: center;
    display: flex;
    flex-direction: column;
    align-items: center;
}

.timeline-item .dot {
    width: 10px;
    height: 10px;
    background-color: #d87ff3;
    border-radius: 50%;
    position: absolute;
    top: -5px; /* Adjusted to align with the line */
    left: 50%;
    transform: translateX(-50%);
    z-index: 1;
}

.timeline-item .top {
    font-weight: bold;
    margin-bottom: 10px;
}

.timeline-item1 .top1 {
    font-weight: bold;
    margin-bottom: 10px;
}

.timeline-item .bottom {
    margin-top: 15px;
}

.timeline-item1 h3 {
    font-size: 16px;
    font-weight: 600;
    color: #333;
}

.timeline-item h3 {
    font-size: 16px;
    font-weight: 600;
    color: #333;
}

.timeline-item1 h4 {
    font-size: 14px;
    font-weight: 400;
    color: #777;
    margin: 5px 0;
}

.timeline-item h4 {
    font-size: 14px;
    font-weight: 400;
    color: #777;
    margin: 5px 0;
}

.timeline-item p {
    font-size: 12px;
    color: #777;
    line-height: 1.6;
}
```
### OUTPUT:


### SKILLS:
#### HTML CODE:
```HTML
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Business Agency</title>
    <link href="skills.css" rel="stylesheet">
</head>

<body>
    <div class="container">
        <h2>SKILLS</h2>
        <div class="skills">
            <div class="skill">
                <span class="skill-name">ADOBE PHOTOSHOP</span>
                <div class="skill-bar"><span style="width: 90%;"></span></div>
                <span class="skill-percent">90%</span>
            </div>
            <div class="skill">
                <span class="skill-name">HTML 5</span>
                <div class="skill-bar"><span style="width: 90%;"></span></div>
                <span class="skill-percent">90%</span>
            </div>
            <div class="skill">
                <span class="skill-name">ADOBE ILLUSTRATOR</span>
                <div class="skill-bar"><span style="width: 85%;"></span></div>
                <span class="skill-percent">85%</span>
            </div>
            <div class="skill">
                <span class="skill-name">CSS 3 ANIMATION</span>
                <div class="skill-bar"><span style="width: 85%;"></span></div>
                <span class="skill-percent">85%</span>
            </div>
            <div class="skill">
                <span class="skill-name">ADOBE AFTER EFFECTS</span>
                <div class="skill-bar"><span style="width: 97%;"></span></div>
                <span class="skill-percent">97%</span>
            </div>
            <div class="skill">
                <span class="skill-name">COMMUNICATION</span>
                <div class="skill-bar"><span style="width: 97%;"></span></div>
                <span class="skill-percent">97%</span>
            </div>
            <div class="skill">
                <span class="skill-name">SKETCH</span>
                <div class="skill-bar"><span style="width: 90%;"></span></div>
                <span class="skill-percent">90%</span>
            </div>
            <div class="skill">
                <span class="skill-name">CREATIVITY</span>
                <div class="skill-bar"><span style="width: 90%;"></span></div>
                <span class="skill-percent">90%</span>
            </div>
        </div>
    </div>
</body>
</html>
```

#### CSS CODE:
```CSS
.container {
    max-width: 900px;
    margin: 50px auto;
    padding: 20px;
    background: white;
    border-radius: 10px;
    box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
}

h2 {
    text-align: center;
    margin-bottom: 20px;
    font-size: 24px;
    font-weight: bold;
}

.skills {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 15px 30px;
    padding: 0 20px;
}

.skill {
    display: flex;
    align-items: center;
    width: 100%;
}

.skill-name {
    width: 150px;
    font-size: 14px;
    font-weight: 600;
    color: #333;
    text-align: left;
}

.skill-bar {
    flex: 1;
    height: 8px;
    background: #ddd;
    border-radius: 5px;
    position: relative;
    overflow: hidden;
}

.skill-bar span {
    display: block;
    height: 100%;
    border-radius: 5px;
    background: linear-gradient(to right, #d946ef, #9333ea);
}

.skill-percent {
    width: 50px;
    text-align: right;
    font-size: 14px;
    font-weight: 600;
    color: #333;
}
```

### EXPERIENCE:
#### HTML CODE:
```HTML
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Business Agency</title>
    <link href="experience.css" rel="stylesheet">
</head>

<body>
    <div class="experience-container">
        <h2 class="experience-heading">Experience</h2>
        <div class="career-timeline">
            <div class="career-entry left-align">
                <div class="career-content">
                    <span class="career-date">2018 - Present</span>
                    <div class="career-position">Creative Director</div>
                    <div class="career-company">HOPLONY TECH LIMITED</div>
                    <div class="career-description">Newyork, USA</div>
                    <div class="career-description">Pain itself is pain in being reprimanded in pleasure, wanting to be a hair of pain in the hope of nothing.</div>
                </div>
            </div>
            <div class="career-entry right-align">
                <div class="career-content">
                    <span class="career-date">2016 - 2018</span>
                    <div class="career-position">Associate Design Director</div>
                    <div class="career-company">HOPLONY TECH LIMITED</div>
                    <div class="career-description">Newyork, USA</div>
                    <div class="career-description">Pain itself is pain in being reprimanded in pleasure, wanting to be a hair of pain in the hope of nothing.</div>
                </div>
            </div>
            <div class="career-entry left-align">
                <div class="career-content">
                    <span class="career-date">2013 - 2016</span>
                    <div class="career-position">Senior UI/UX Designer</div>
                    <div class="career-company">HOPLONY TECH LIMITED</div>
                    <div class="career-description">Newyork, USA</div>
                    <div class="career-description">Pain itself is pain in being reprimanded in pleasure, wanting to be a hair of pain in the hope of nothing.</div>
                </div>
            </div>
            <div class="career-entry right-align">
                <div class="career-content">
                    <span class="career-date">2012 - 2013</span>
                    <div class="career-position">UI/UX Designer</div>
                    <div class="career-company">HOPLONY TECH LIMITED</div>
                    <div class="career-description">Newyork, USA</div>
                    <div class="career-description">Pain itself is pain in being reprimanded in pleasure, wanting to be a hair of pain in the hope of nothing.</div>
                </div>
            </div>
            <div class="career-entry left-align">
                <div class="career-content">
                    <span class="career-date">2010 - 2012</span>
                    <div class="career-position">Frontend Developer</div>
                    <div class="career-company">HOPLONY TECH LIMITED</div>
                    <div class="career-description">Newyork, USA</div>
                    <div class="career-description">Pain itself is pain in being reprimanded in pleasure, wanting to be a hair of pain in the hope of nothing</div>
                </div>
            </div>
        </div>
    </div>
</body>
</html>
```

#### CSS CODE:
```CSS
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Poppins', sans-serif;
}

body {
    background-color: #f8f9fc;
    text-align: center;
}

.experience-container {
    width: 100%;
    max-width: 1200px;
    margin: 50px auto;
    text-align: center;
}
.experience-heading {
    font-size: 24px;
    font-weight: 600;
    color: #333;
    margin-bottom: 50px;
    text-transform: uppercase;
}

/* Timeline */
.career-timeline {
    position: relative;
    max-width: 1000px;
    margin: auto;
}
.career-timeline::after {
    content: '';
    position: absolute;
    width: 4px;
    background: #d946ef;
    top: 0;
    bottom: 0;
    left: 50%;
    transform: translateX(-50%);
}
.career-entry {
    position: relative;
    width: 50%;
    padding: 20px;
}
.career-entry.left-align {
    left: 0;
    text-align: right;
}
.career-entry.right-align {
    left: 50%;
    text-align: left;
}
.career-entry::before {
    content: '';
    position: absolute;
    width: 14px;
    height: 14px;
    background: #d946ef;
    border-radius: 50%;
    top: 30px;
    left: 100%;
    transform: translateX(-50%);
}
.career-entry.right-align::before {
    left: 0;
    transform: translateX(-50%);
}
.career-content {
    display: inline-block;
    background: #fff;
    padding: 15px;
    border-radius: 8px;
    box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1);
    width: 80%;
}
.career-date {
    font-size: 14px;
    font-weight: 600;
    color: #333;
}
.career-position {
    font-size: 18px;
    font-weight: 600;
    color: #111;
    margin: 5px 0;
}
.career-company {
    font-size: 14px;
    font-weight: 600;
    color: #555;
}
.career-description {
    font-size: 13px;
    color: #777;
    margin-top: 10px;
    line-height: 1.5;
}
```

### PROFILE:
#### HTML CODE:
```HTML
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">
    <title>Business Agency</title>
    <link rel="stylesheet" href="profile.css">
</head>

<body>
    <div class="container">
        <h2>PROFILES</h2>
        <div class="grid">
            <div class="profile-item">
                <i class="fas fa-tree"></i>
                <p>Themeforest</p>
            </div>
            <div class="profile-item">
                <i class="fas fa-basketball-ball"></i>
                <p>Dribbble</p>
            </div>
            <div class="profile-item">
                <i class="fab fa-behance"></i>
                <p>Behance</p>
            </div>
            <div class="profile-item">
                <i class="fab fa-github"></i>
                <p>Github</p>
            </div>
            <div class="profile-item">
                <i class="fab fa-flickr"></i>
                <p>Flickr</p>
            </div>
            <div class="profile-item">
                <i class="fas fa-smile"></i>
                <p>SmungMung</p>
            </div>
            <div class="profile-item">
                <i class="fas fa-layer-group"></i>
                <p>SquareSpace</p>
            </div>
            <div class="profile-item">
                <i class="fab fa-bitbucket"></i>
                <p>BitBucket</p>
            </div>
        </div>
    </div>
</body>

</html>
```

#### CSS CODE:
```CSS
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: Arial, sans-serif;
}
body {
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    background-color: #f8f9fa;
}
.container {
    text-align: center;
    width: 80%;
    max-width: 800px;
}
h2 {
    font-size: 22px;
    font-weight: bold;
    margin-bottom: 20px;
}
.grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 30px;
    padding: 20px;
    background: #fff;
    box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.1);
    border-radius: 10px;
}
.profile-item {
    text-align: center;
    color: #666;
}
.profile-item i {
    font-size: 30px;
    margin-bottom: 10px;
    display: block;
    color: #333;
}
```

### PORTFOLIO:
#### HTML CODE:
```HTML
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portfolio Image</title>
    <link rel="stylesheet" href="portfolio.css">
</head>
<body>
    <header>
        <h1>PORTFOLIO</h1>
    </header>
    <div class="portfolio">
        <img src="portfolio.png" alt="Portfolio Image">
    </div>

</body>
</html>
```

#### CSS CODE:
```CSS
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    height: 100vh;
    background-color: #f4f4f4;
    font-family: Arial, sans-serif;
}

header {
    margin-bottom: 20px;
}

h1 {
    font-size: 28px;
    font-weight: bold;
    color: #333;
    text-transform: uppercase;
}

.portfolio img {
    max-width: 100%;
    height: auto;
    border-radius: 10px;
    box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.1);
}
```

### CLIENTS:
#### HTML CODE:
```HTML
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Clients</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">
    <link rel="stylesheet" href="clientsection.css"> <!-- Link to your CSS -->
</head>
<body>

<section class="clients">
    <h2>Clients</h2>
    <div class="clients-container">
        <img src="/Project/Portfolio_New/client/logo/State-Street.jpg" alt="State Street">
        <img src="/Project/Portfolio_New/client/logo/kinder-morgan-1.svg" alt="Kinder Morgan">
        <img src="/Project/Portfolio_New/client/logo/gilead.png" alt="Gilead">
        <img src="/Project/Portfolio_New/client/logo/ubisoft.jpg" alt="Ubisoft">
        <img src="/Project/Portfolio_New/client/logo/disney.jpg" alt="Disney">
        <img src="/Project/Portfolio_New/client/logo/johnson.png" alt="Johnson Controls">
        <img src="/Project/Portfolio_New/client/logo/cisco logo.png" alt="Cisco">
    </div>
</section>

</body>
</html>
```

#### CSS CODE:
```CSS
body {
    margin: 0;
    font-family: Arial, sans-serif;
    text-align: center;
}

.clients {
    padding: 50px 20px;
}

h2 {
    font-size: 22px;
    font-weight: bold;
    text-transform: uppercase;
    margin-bottom: 30px;
}

.clients-container {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 40px;
}

.clients-container img {
    max-width: 120px; /* Adjust size as needed */
    filter: grayscale(100%); /* Optional: Makes logos gray */
    transition: 0.3s ease-in-out;
}

.clients-container img:hover {
    filter: grayscale(0%);
}
```

### CONTACT:
#### HTML CODE:
```HTML
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contact Me Section</title>
    <link rel="stylesheet" href="contactme.css">
</head>

<body>
<section>
    <div class="contact-section">
        <h2>Contact Me</h2>
        <div class="contact-container">
            <div class="contact-form">
                <input type="text" placeholder="Name*" required>
                <input type="email" placeholder="Email*" required>
                <input type="text" placeholder="Subject">
                <textarea rows="4" placeholder="Message"></textarea>
                <button type="submit">Submit</button>
            </div>
            <div class="contact-info">
                <h3>Browny Star</h3>
                <p>UI/UX Designer</p>
                <p><strong>Phone:</strong> 987-123-6547</p>
                <p><strong>Email:</strong> browny@info.com</p>
                <p><strong>Website:</strong> www.brownsnine.com</p>
                <div class="social-icons">
                    <a href="#">🔵</a>
                    <a href="#">🟣</a>
                    <a href="#">⚫</a>
                    <a href="#">🔵</a>
                </div>
            </div>
        </div>
    </div>
</section>
<footer>
    <p>&copy; 2025 Business Agency | All Rights Reserved</p>
</footer>
</body>

</html>
```

#### CSS CODE:
```CSS
body {
    margin: 0;
    font-family: Arial, sans-serif;
    scroll-behavior: smooth;
}


section {
    padding: 30px;
    text-align: center;
}

.section-title {
    font-size: 24px;
    font-weight: 700;
    color: #222;
    text-transform: uppercase;
    margin-bottom: 40px;
}

footer {
    text-align: center;
    padding: 20px;
    background: #333;
    color: white;
}


footer {
    text-align: center;
    padding: 20px;
    background: #333;
    color: white;
}
   
.contact-section {
    width: 80%;
    max-width: 1200px;
    margin: 50px auto;
}

.contact-container {
    display: flex;
    justify-content: space-between;
    background-color: #ffffff;
    padding: 40px;
    border-radius: 10px;
    box-shadow: 0px 5px 15px rgba(0, 0, 0, 0.1);
}

.contact-form {
    width: 50%;
    display: flex;
    flex-direction: column;
    gap: 15px;
}

.contact-form input, .contact-form textarea {
    width: 100%;
    padding: 12px;
    border: 1px solid #ddd;
    border-radius: 5px;
    font-size: 14px;
}

.contact-form button {
    background-color: #7D29E2;
    color: white;
    padding: 12px;
    border: none;
    border-radius: 5px;
    font-size: 16px;
    cursor: pointer;
}

.contact-form button:hover {
    background-color: #5B1DAB;
}

.contact-info {
    width: 40%;
    text-align: left;
}

.contact-info h3 {
    font-size: 18px;
    font-weight: 600;
    color: #333;
    margin-bottom: 10px;
}

.contact-info p {
    font-size: 14px;
    color: #666;
    margin: 5px 0;
}

.social-icons {
    margin-top: 15px;
}

.social-icons a {
    display: inline-block;
    margin-right: 10px;
    text-decoration: none;
    font-size: 18px;
    color: #666;
}

.social-icons a:hover {
    color: #7D29E2;
}
```

### OUTPUTS:

### HOME PAGE:
![alt text](outputs/home1.png)

### ABOUT ME PAGE:


### EDUCATION PAGE:
![alt text](outputs/education.png)

### SKILLS:
![alt text](outputs/skill.png)

### EXPERIENCE:
![alt text](outputs/experience.png)

### PROFILE:
![alt text](outputs/profile.png)

### PORTFOLIO:
![alt text](outputs/portfolio.png)

### CLIENTS:
![alt text](outputs/client.png)

### CONTACTS ME:
![alt text](outputs/contact.png)
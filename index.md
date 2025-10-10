<!-- Responsive Navigation for GitHub Pages (works in Markdown) -->
<style>
  /* Reset */
  * {
    box-sizing: border-box;
  }
  body {
    margin: 0;
    font-family: -apple-system, Segoe UI, Roboto, Helvetica, Arial, sans-serif;
  }

  /* Navbar - Hamburger only */
  .nav {
    position: sticky;
    top: 0;
    z-index: 9999;
    display: flex;
    align-items: center;
    justify-content: flex-end;
    padding: 12px 16px;
    background: #0d1117;
    color: #e6edf3;
    border-bottom: 1px solid #30363d;
  }
  .nav a {
    color: #e6edf3;
    text-decoration: none;
  }
  .nav a:hover {
    color: #58a6ff;
  }
  .menu {
    display: none;
    flex-direction: column;
    padding: 8px 0;
    position: absolute;
    top: 50px;
    right: 16px;
    background: #0d1117;
    border: 1px solid #30363d;
    border-radius: 6px;
    min-width: 150px;
  }
  .menu.open {
    display: flex;
  }
  .menu a {
    padding: 8px 16px;
  }
  .hamb {
    display: inline-flex;
    align-items: center;
    gap: 8px;
    background: transparent;
    border: 1px solid #30363d;
    color: #e6edf3;
    padding: 6px 10px;
    border-radius: 6px;
    cursor: pointer;
  }
  .hamb:focus {
    outline: 2px solid #58a6ff;
    outline-offset: 2px;
  }

  /* Section spacing */
  section {
    scroll-margin-top: 80px;
  }

  /* Project grid and images */
  .section-title {
    margin: 28px 0 10px;
    font-size: 1.6rem;
  }
  .subgroup {
    margin-top: 18px;
  }
  .subgroup h3 {
    font-size: 1.3rem;
    margin: 20px 0 12px;
    color: #0969da;
  }
  .cards {
    display: grid;
    grid-template-columns: repeat(12, 1fr);
    gap: 14px;
  }
  .card {
    grid-column: span 6;
    border: 1px solid #d0d7de;
    border-radius: 10px;
    padding: 14px;
    background: #ffffff;
  }
  .card img {
    width: 100%;
    height: 180px;
    object-fit: cover;
    border-radius: 6px;
    margin-bottom: 10px;
  }
  .card h3 {
    margin: 0 0 6px;
    font-size: 1.05rem;
  }
  .card p {
    margin: 0 0 8px;
    color: #57606a;
  }
  .tags {
    display: flex;
    flex-wrap: wrap;
    gap: 6px;
  }
  .tag {
    font-size: .78rem;
    background: #eaeef2;
    color: #0d1117;
    padding: 3px 8px;
    border-radius: 999px;
    border: 1px solid #d0d7de;
  }

  @media (max-width: 900px) {
    .card {
      grid-column: span 12;
    }
  }

  /* Page container compatibility on GitHub Pages */
  .container-lg {
    max-width: 1012px;
    margin: 0 auto;
    padding: 0 16px;
  }
</style>

<script>
  // Toggle menu on hamburger click
  function toggleMenu() {
    const menu = document.getElementById('nav-menu');
    menu.classList.toggle('open');
  }

  // Close menu when clicking anywhere
  document.addEventListener('click', (e) => {
    const nav = document.querySelector('.nav');
    if (!nav.contains(e.target)) {
      const menu = document.getElementById('nav-menu');
      menu.classList.remove('open');
    }
  });
</script>

<style>
  /* Heading styles */
  h2 {
    font-weight: bold;
    color: #1976d2;
    font-size: 1.8rem;
    margin-top: 40px;
    margin-bottom: 18px;
    border-bottom: 2px solid #1976d2;
    padding-bottom: 10px;
  }

  h3 {
    font-weight: bold;
    color: #2b4580;
    margin-top: 40px;
    margin-bottom: 18px;
  }

  /* Section spacing utility */
  .section-space {
    margin-top: 60px;
  }
</style>

<div class="nav">
  <button class="hamb" onclick="toggleMenu()" aria-label="Menu">
    <svg width="16" height="16" fill="currentColor" viewBox="0 0 16 16">
      <path fill-rule="evenodd" d="M1 2.75A.75.75 0 011.75 2h12.5a.75.75 0 110 1.5H1.75A.75.75 0 011 2.75zm0 5A.75.75 0 011.75 7h12.5a.75.75 0 110 1.5H1.75A.75.75 0 011 7.75zM1.75 12a.75.75 0 100 1.5h12.5a.75.75 0 100-1.5H1.75z"></path>
    </svg>
    Menu
  </button>
  <div class="menu" id="nav-menu">
    <a href="#about">About</a>
    <a href="#accomplishments">Accomplishments</a>
    <a href="#projects">Projects</a>
    <a href="#skills">Skills</a>
    <a href="#education">Education</a>
  </div>
</div>

<div class="section-space"></div>

## About Me

I'm **Shruthi Sree**, an aspiring software engineer passionate about building impactful solutions through code. Currently pursuing my undergraduate degree in **Computer Science and Engineering** at **Velagapudi Ramakrishna Siddhartha Engineering College**, I have developed a strong foundation in algorithms, data structures, and full-stack development.

I enjoy working on projects that challenge me to think critically and creatively. Whether it's developing machine learning models, designing intuitive user interfaces, or optimizing backend systems, I'm always eager to learn and grow. I believe in writing clean, maintainable code and staying updated with the latest technologies.

When I'm not coding, you'll find me exploring new tech trends, participating in hackathons, or contributing to open-source projects. I'm excited to collaborate with like-minded individuals and make meaningful contributions to the tech community!

<div class="section-space"></div>

## Accomplishments

- **Selected among top 55 student ambassadors** at VRSEC from pool of over 500 students
- **Active contributor** to open-source projects on GitHub
- **Completed multiple certifications** in Python, Java, and web development
- **Participated in various hackathons** and coding competitions

<div class="section-space"></div>

## Projects

<div class="cards">
  <div class="card">
    <img src="https://via.placeholder.com/400x180/0969da/ffffff?text=Movie+Recommendation" alt="Movie Recommendation System"/>
    <h3>Movie Recommendation System</h3>
    <p>Developed a content-based recommendation system using cosine similarity and TF-IDF vectorization to suggest movies based on user preferences.</p>
    <div class="tags">
      <span class="tag">Python</span>
      <span class="tag">Pandas</span>
      <span class="tag">Scikit-learn</span>
      <span class="tag">Streamlit</span>
    </div>
  </div>

  <div class="card">
    <img src="https://via.placeholder.com/400x180/2da44e/ffffff?text=Portfolio+Website" alt="Portfolio Website"/>
    <h3>Personal Portfolio Website</h3>
    <p>Designed and deployed a responsive portfolio website showcasing my projects, skills, and achievements.</p>
    <div class="tags">
      <span class="tag">HTML</span>
      <span class="tag">CSS</span>
      <span class="tag">JavaScript</span>
      <span class="tag">GitHub Pages</span>
    </div>
  </div>

  <div class="card">
    <img src="https://via.placeholder.com/400x180/8250df/ffffff?text=Regression+ML" alt="Regression ML"/>
    <h3>Regression Models Comparison</h3>
    <p>Compared various regression techniques to determine the best model for sales forecasting.</p>
    <div class="tags">
      <span class="tag">Python</span>
      <span class="tag">Scikit-learn</span>
      <span class="tag">Seaborn</span>
    </div>
  </div>

  <div class="card">
    <img src="https://via.placeholder.com/400x180/bf3989/ffffff?text=Algorithm+Viz" alt="Algorithm Visualization"/>
    <h3>Algorithm Visualization Tool</h3>
    <p>Developed an interactive tool to visualize sorting and searching algorithms for educational purposes.</p>
    <div class="tags">
      <span class="tag">JavaScript</span>
      <span class="tag">D3.js</span>
      <span class="tag">HTML/CSS</span>
    </div>
  </div>

  <div class="card">
    <img src="https://via.placeholder.com/400x180/fb8500/ffffff?text=Face+Mask+Detection" alt="Face Mask Detection"/>
    <h3>Face Mask Detection System</h3>
    <p>Built a CNN-based system to detect face masks in real-time using OpenCV and TensorFlow.</p>
    <div class="tags">
      <span class="tag">Python</span>
      <span class="tag">TensorFlow</span>
      <span class="tag">OpenCV</span>
    </div>
  </div>
</div>

<div class="section-space"></div>

## Skills

### Programming Languages
- Python, Java, C++, JavaScript

### Web Development
- HTML, CSS, React.js, Node.js, Express.js

### Machine Learning & Data Science
- TensorFlow, Scikit-learn, Pandas, NumPy, Matplotlib

### Tools & Technologies
- Git, GitHub, VS Code, Jupyter Notebook, Postman

### Databases
- MySQL, MongoDB

<div class="section-space"></div>

## Education

**Velagapudi Ramakrishna Siddhartha Engineering College**  
Bachelor of Technology in Computer Science and Engineering  
2022 - 2026 (Expected)

---

**Contact Me:**  
Feel free to reach out via [GitHub](https://github.com/shruthisree1234) or [LinkedIn](https://linkedin.com/in/shruthisree)!

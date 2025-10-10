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

  /* Typography */
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
    color: #333;
    font-size: 1.3rem;
    margin-top: 24px;
    margin-bottom: 14px;
  }
  p, li {
    color: #555;
    line-height: 1.7;
    margin-bottom: 14px;
  }

  /* Cards */
  .card {
    background: #f9f9f9;
    border: 1px solid #ddd;
    border-radius: 8px;
    padding: 16px;
    margin-bottom: 20px;
    box-shadow: 0 1px 3px rgba(0,0,0,0.1);
  }
  .card img {
    width: 100%;
    border-radius: 6px;
    margin-bottom: 10px;
  }
  .card h3 {
    margin-top: 0;
    color: #1976d2;
  }
  .card p {
    margin: 10px 0;
    color: #666;
  }
  .tags {
    display: flex;
    flex-wrap: wrap;
    gap: 8px;
    margin-top: 10px;
  }
  .tag {
    background: #1976d2;
    color: white;
    padding: 4px 10px;
    border-radius: 12px;
    font-size: 0.85rem;
  }

  /* Utilities */
  .section-space {
    height: 30px;
  }

  /* Site description color matching title */
  .project-tagline {
    color: #1976d2 !important;
  }
</style>

<script>
function toggleMenu() {
  const menu = document.querySelector('.menu');
  menu.classList.toggle('open');
}
</script>

<div class="nav">
  <button class="hamb" onclick="toggleMenu()">☰ Menu</button>
  <div class="menu">
    <a href="#about">About</a>
    <a href="#projects">Projects</a>
    <a href="#skills">Skills</a>
    <a href="#education">Education</a>
  </div>
</div>

<div class="section-space"></div>

## About Me

I am a passionate **Computer Science Engineering** student specializing in **Data Analysis and Data Engineering**. With a strong foundation in programming languages such as Python, Java, and JavaScript, I enjoy building data-driven applications and solving real-world problems through technology.

---

## Projects

<div class="card">
  <img src="https://via.placeholder.com/400x180/1976d2/ffffff?text=Data+Pipeline" alt="Data Pipeline"/>
  <h3>Data Pipeline Automation Tool</h3>
  <p>Designed and implemented an automated data pipeline to process and transform large datasets for analytics.</p>
  <div class="tags">
    <span class="tag">Python</span>
    <span class="tag">SQL</span>
    <span class="tag">Apache Airflow</span>
  </div>
</div>

<div class="card">
  <img src="https://via.placeholder.com/400x180/388e3c/ffffff?text=Dashboard" alt="Dashboard"/>
  <h3>Interactive Analytics Dashboard</h3>
  <p>Built an interactive dashboard to visualize key business metrics using real-time data.</p>
  <div class="tags">
    <span class="tag">React.js</span>
    <span class="tag">Chart.js</span>
    <span class="tag">Node.js</span>
  </div>
</div>

<div class="card">
  <img src="https://via.placeholder.com/400x180/d32f2f/ffffff?text=ML+Model" alt="ML Model"/>
  <h3>Customer Churn Prediction Model</h3>
  <p>Developed a machine learning model to predict customer churn with 85% accuracy using logistic regression.</p>
  <div class="tags">
    <span class="tag">Python</span>
    <span class="tag">Scikit-learn</span>
    <span class="tag">Pandas</span>
  </div>
</div>

<div class="card">
  <img src="https://via.placeholder.com/400x180/7b1fa2/ffffff?text=Exploratory+Analysis" alt="Exploratory Analysis"/>
  <h3>Exploratory Data Analysis on COVID-19 Dataset</h3>
  <p>Performed comprehensive EDA on COVID-19 data to uncover trends and patterns in infection rates.</p>
  <div class="tags">
    <span class="tag">Python</span>
    <span class="tag">Pandas</span>
    <span class="tag">Matplotlib</span>
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

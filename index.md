<!-- Responsive Navigation for GitHub Pages (works in Markdown) -->
<style>
  /* Reset */
  * { box-sizing: border-box; }
  body { margin: 0; font-family: -apple-system, Segoe UI, Roboto, Helvetica, Arial, sans-serif; }
  
  /* Navbar - Hamburger only */
  .nav {
    position: sticky; top: 0; z-index: 9999;
    display: flex; align-items: center; justify-content: flex-end;
    padding: 12px 16px; background: #0d1117; color: #e6edf3; border-bottom: 1px solid #30363d;
  }
  .nav a { color: #e6edf3; text-decoration: none; }
  .nav a:hover { color: #58a6ff; }
  .menu { display: none; flex-direction: column; padding: 8px 0; position: absolute; top: 50px; right: 16px; background: #0d1117; border: 1px solid #30363d; border-radius: 6px; min-width: 150px; }
  .menu.open { display: flex; }
  .menu a { padding: 8px 16px; }
  .hamb { display: inline-flex; align-items: center; gap: 8px; background: transparent; border: 1px solid #30363d; color: #e6edf3; padding: 6px 10px; border-radius: 6px; cursor: pointer; }
  .hamb:focus { outline: 2px solid #58a6ff; outline-offset: 2px; }
  
  /* Section spacing */
  section { scroll-margin-top: 80px; }
  
  /* Project grid and images */
  .section-title { margin: 28px 0 10px; font-size: 1.6rem; }
  .subgroup { margin-top: 18px; }
  .subgroup h3 { font-size: 1.3rem; margin: 20px 0 12px; color: #0969da; }
  .cards { display: grid; grid-template-columns: repeat(12, 1fr); gap: 14px; }
  .card { grid-column: span 6; border: 1px solid #d0d7de; border-radius: 10px; padding: 14px; background: #ffffff; }
  .card img { width: 100%; height: 180px; object-fit: cover; border-radius: 6px; margin-bottom: 10px; }
  .card h3 { margin: 0 0 6px; font-size: 1.05rem; }
  .card p { margin: 0 0 8px; color: #57606a; }
  .tags { display: flex; flex-wrap: wrap; gap: 6px; }
  .tag { font-size: .78rem; background: #eaeef2; color: #0d1117; padding: 3px 8px; border-radius: 999px; border: 1px solid #d0d7de; }
  @media (max-width: 900px) { .card { grid-column: span 12; } }
  
  /* Page container compatibility on GitHub Pages */
  .container { max-width: 1000px; margin: 0 auto; padding: 0 16px; }
</style>

<nav class="nav container">
  <button class="hamb" id="hamb" aria-expanded="false" aria-controls="menu">☰</button>
  <div class="menu" id="menu">
    <a href="#about">About</a>
    <a href="#accomplishments">Accomplishments</a>
    <a href="#projects">Projects</a>
    <a href="#skills">Skills</a>
    <a href="#education">Education</a>
  </div>
</nav>

<script>
  (function(){
    const b = document.getElementById('hamb');
    const m = document.getElementById('menu');
    if (b && m) {
      b.addEventListener('click', function(){
        const open = m.classList.toggle('open');
        b.setAttribute('aria-expanded', open ? 'true' : 'false');
      });
    }
  })();
</script>

<div class="container">

<section id="about">

# Shruthi Sree - Data Analyst

Welcome! I am an aspiring data analyst with a strong foundation in statistical analysis, data visualization, and machine learning. I enjoy transforming raw data into actionable insights that drive business decisions.

📧 Email: shruthisree1234@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/shruthi-sree-58b856320/)  
💻 [GitHub](https://github.com/shruthisree1234)

</section>

<section id="accomplishments">

## 🏆 Accomplishments

- **HackerRank SQL Gold Badge**: Demonstrated proficiency in writing complex SQL queries.
- **Certifications**: Completed courses in Data Analysis, Machine Learning, and Python from Coursera and Udemy.
- **University Projects**: Led multiple data-driven projects during my academic tenure.

</section>

<section id="projects">

<h2 class="section-title">📂 Projects</h2>

<div class="subgroup">
  <h3>Product Analytics</h3>
  <div class="cards">
    <div class="card">
      <img src="images/churn-rate-1.jpg" alt="Customer Churn Analysis">
      <h3>Customer Churn Analysis</h3>
      <p>Analyzed customer churn patterns using SQL and visualization tools to identify key factors affecting retention.</p>
      <div class="tags">
        <span class="tag">SQL</span>
        <span class="tag">Power BI</span>
        <span class="tag">Excel</span>
      </div>
    </div>
    
    <div class="card">
      <img src="images/Data pipeline.png" alt="Data Pipeline">
      <h3>Data Pipeline Project</h3>
      <p>Built an automated data pipeline to extract, transform, and load data from multiple sources for analytics.</p>
      <div class="tags">
        <span class="tag">Python</span>
        <span class="tag">ETL</span>
        <span class="tag">PostgreSQL</span>
      </div>
    </div>
  </div>
</div>

<div class="subgroup">
  <h3>Operational Analytics</h3>
  <div class="cards">
    <div class="card">
      <img src="images/operational.jpg" alt="Operational Analytics">
      <h3>Operational Efficiency Analysis</h3>
      <p>Evaluated operational data to optimize resource allocation and reduce costs by 15%.</p>
      <div class="tags">
        <span class="tag">Tableau</span>
        <span class="tag">SQL</span>
        <span class="tag">Excel</span>
      </div>
    </div>
    
    <div class="card">
      <img src="images/sentiment.png" alt="Sentiment Analysis">
      <h3>Sentiment Analysis Dashboard</h3>
      <p>Created a sentiment analysis tool to monitor customer feedback and identify improvement areas.</p>
      <div class="tags">
        <span class="tag">Python</span>
        <span class="tag">NLP</span>
        <span class="tag">Power BI</span>
      </div>
    </div>
  </div>
</div>

<div class="subgroup">
  <h3>Healthcare Analytics</h3>
  <div class="cards">
    <div class="card">
      <img src="images/predictivemodeling.jpg" alt="Predictive Modeling">
      <h3>Healthcare Predictive Modeling</h3>
      <p>Developed predictive models to forecast patient readmission rates using logistic regression.</p>
      <div class="tags">
        <span class="tag">Python</span>
        <span class="tag">Scikit-learn</span>
        <span class="tag">Pandas</span>
      </div>
    </div>
  </div>
</div>

<div class="subgroup">
  <h3>Machine Learning & Visualization</h3>
  <div class="cards">
    <div class="card">
      <img src="images/bikerental.png" alt="Bike Rental Prediction">
      <h3>Bike Rental Demand Prediction</h3>
      <p>Predicted bike rental demand using linear regression and time series analysis.</p>
      <div class="tags">
        <span class="tag">Python</span>
        <span class="tag">Machine Learning</span>
        <span class="tag">Matplotlib</span>
      </div>
    </div>
    
    <div class="card">
      <img src="images/regresssion_ML.png" alt="Regression ML">
      <h3>Regression Models Comparison</h3>
      <p>Compared various regression techniques to determine the best model for sales forecasting.</p>
      <div class="tags">
        <span class="tag">Python</span>
        <span class="tag">Scikit-learn</span>
        <span class="tag">Seaborn</span>
      </div>
    </div>
    
    <div class="card">
      <img src="images/algovisual.png" alt="Algorithm Visualization">
      <h3>Algorithm Visualization Tool</h3>
      <p>Developed an interactive tool to visualize sorting and searching algorithms for educational purposes.</p>
      <div class="tags">
        <span class="tag">JavaScript</span>
        <span class="tag">D3.js</span>
        <span class="tag">HTML/CSS</span>
      </div>
    </div>
    
    <div class="card">
      <img src="images/face mask.png" alt="Face Mask Detection">
      <h3>Face Mask Detection System</h3>
      <p>Built a CNN-based system to detect face masks in real-time using OpenCV and TensorFlow.</p>
      <div class="tags">
        <span class="tag">Python</span>
        <span class="tag">TensorFlow</span>
        <span class="tag">OpenCV</span>
      </div>
    </div>
  </div>
</div>

</section>

<section id="skills">

## 🛠️ Skills

**Programming Languages**: Python, SQL, R  
**Data Visualization**: Tableau, Power BI, Matplotlib, Seaborn  
**Data Analysis**: Excel, Pandas, NumPy  
**Machine Learning**: Scikit-learn, TensorFlow  
**Database**: MySQL, PostgreSQL, MongoDB  
**Tools**: Git, Jupyter Notebook, VS Code

</section>

<section id="education">

## 🎓 Education

**Bachelor of Technology in Computer Science**  
Dayananda Sagar College of Engineering, Bangalore  
Graduation Year: 2026  
CGPA: 8.5/10

</section>

---

© 2024 Shruthi Sree. All rights reserved.

</div>

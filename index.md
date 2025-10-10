<!-- Responsive Navigation for GitHub Pages (works in Markdown) -->
<style>
  /* Reset */
  * { box-sizing: border-box; }
  body { margin: 0; font-family: -apple-system, Segoe UI, Roboto, Helvetica, Arial, sans-serif; }

  /* Navbar */
  .nav {
    position: sticky; top: 0; z-index: 9999;
    display: flex; align-items: center; justify-content: space-between;
    padding: 12px 16px; background: #0d1117; color: #e6edf3; border-bottom: 1px solid #30363d;
  }
  .brand { font-weight: 700; letter-spacing: .2px; }
  .nav a { color: #e6edf3; text-decoration: none; }
  .nav a:hover { color: #58a6ff; }
  .menu { display: flex; gap: 16px; }
  .hamb { display: none; background: transparent; border: 1px solid #30363d; color: #e6edf3; padding: 6px 10px; border-radius: 6px; }
  .hamb:focus { outline: 2px solid #58a6ff; outline-offset: 2px; }

  /* Mobile */
  @media (max-width: 720px) {
    .menu { display: none; flex-direction: column; padding: 8px 0; }
    .menu.open { display: flex; }
    .hamb { display: inline-flex; align-items: center; gap: 8px; }
  }

  /* Section spacing */
  section { scroll-margin-top: 80px; }

  /* Project grid */
  .section-title { margin: 28px 0 10px; font-size: 1.6rem; }
  .subgroup { margin-top: 18px; }
  .cards { display: grid; grid-template-columns: repeat(12, 1fr); gap: 14px; }
  .card { grid-column: span 6; border: 1px solid #d0d7de; border-radius: 10px; padding: 14px; background: #ffffff; }
  .card h3 { margin: 0 0 6px; font-size: 1.05rem; }
  .card p { margin: 0 0 8px; color: #57606a; }
  .tags { display: flex; flex-wrap: wrap; gap: 6px; }
  .tag { font-size: .78rem; background: #eaeef2; color: #0d1117; padding: 3px 8px; border-radius: 999px; border: 1px solid #d0d7de; }
  @media (max-width: 900px) { .card { grid-column: span 12; } }

  /* Page container compatibility on GitHub Pages */
  .container { max-width: 1000px; margin: 0 auto; padding: 0 16px; }
</style>

<nav class="nav container">
  <div class="brand">Shruthi Sree</div>
  <button class="hamb" id="hamb" aria-expanded="false" aria-controls="menu">☰ Menu</button>
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

<!-- Title kept as-is -->
<h1>👋 Hi, I'm Shruthi Sree</h1>

<!-- About (anchor only, content unchanged) -->
<a id="about"></a>
<h2>About Me</h2>
<p>With 3+ years of experience in data analytics, data engineering, business insights, machine learning, and data storytelling, I specialize in designing and optimizing end-to-end solutions that deliver measurable results. My work enables teams to transform raw data into actionable intelligence, solve complex challenges, and drive strategic business decisions.</p>
<ul>
  <li>⚡ Expert in data modeling, analytics, and communicating insights through impactful storytelling</li>
  <li>🛠️ Skilled in Python, SQL, Spark, Tableau, Power BI, and cloud platforms—delivering scalable and reliable solutions</li>
  <li>✨ Proven collaborator and mentor, committed to supporting cross-functional teams and creating a culture of data-driven success</li>
  <li>🚀 Passionate about leveraging technology and analytics to unlock new business opportunities</li>
</ul>
<p>If you're looking for someone who combines deep technical expertise with business acumen and a knack for making data meaningful, let's connect – I thrive on partnering to solve big challenges and deliver measurable results.</p>

<!-- Accomplishments (anchor only, content unchanged) -->
<a id="accomplishments"></a>
<h2>Accomplishments</h2>
<ul>
  <li><strong>Scalable Data Solutions</strong> — Engineered data pipelines using Spark, Kafka, and Azure, automating the flow of over 43 million telemetry events daily. This enabled real-time monitoring, faster decision-making, and supported expanded business capabilities.</li>
  <li><strong>Faster, Smarter Reporting</strong> — Designed and deployed Tableau/Power BI dashboards that cut manual reporting efforts by 40%. This gave business leaders instant access to actionable metrics, accelerating performance reviews and driving better decision making.</li>
  <li><strong>Reliable Data for Confident Decisions</strong> — Led warehouse validation and automated data checks, reducing reporting errors by 20%. Improved clinical data quality allowed teams to trust insights and make regulatory and operational decisions more securely.</li>
  <li><strong>Downtime Slashed, Productivity Up</strong> — Built anomaly detection and forecasting models that helped the field team proactively prevent equipment failures, reducing downtime by 25%.</li>
  <li><strong>Rapid Issue Resolution</strong> — Diagnosed and resolved data integration challenges across analytics and operations, increasing pipeline reliability by 18%.</li>
  <li><strong>Influenced Executive Decision-Making</strong> — Delivered tailored dashboards and predictive models for leadership that improved quarterly strategic planning and resource investment.</li>
  <li><strong>Built a Culture of Shared Success</strong> — Led peer learning and documented best practices, mentoring teammates in SQL, analytics, and reporting workflows.</li>
</ul>

<!-- Projects (refactored by categories) -->
<a id="projects"></a>
<h2 class="section-title">Projects</h2>

<!-- Product Analytics -->
<div class="subgroup">
  <h3>Product Analytics</h3>
  <div class="cards">
    <div class="card">
      <h3><a href="https://github.com/shruthisree1234/SaaS_Churn_Prediction">SaaS Churn Prediction</a></h3>
      <p>Predictive analytics for churn risk in a subscription product; includes cohorting, retention curves, features from usage, and interpretable models to guide lifecycle actions.</p>
      <div class="tags">
        <span class="tag">Python</span><span class="tag">Pandas</span><span class="tag">Scikit-learn</span><span class="tag">Cohort Analysis</span>
      </div>
    </div>
  </div>
</div>

<!-- Operational Analytics -->
<div class="subgroup">
  <h3>Operational Analytics</h3>
  <div class="cards">
    <div class="card">
      <h3><a href="https://github.com/shruthisree1234/End-to-End-Data-Pipeline">End-to-End Data Pipeline</a></h3>
      <p>Batch/stream ETL with quality checks, orchestration, and reporting to deliver reliable data for operations.</p>
      <div class="tags"><span class="tag">Spark</span><span class="tag">Airflow</span><span class="tag">Kafka</span><span class="tag">Azure</span></div>
    </div>
    <div class="card">
      <h3><a href="https://github.com/shruthisree1234/Product-Rental-System-Performance-Monitoring">Performance Monitoring &amp; Visualization</a></h3>
      <p>Operational KPIs and alerting for a product rental platform; dashboards for utilization and SLA tracking.</p>
      <div class="tags"><span class="tag">Power BI</span><span class="tag">Tableau</span><span class="tag">SQL</span></div>
    </div>
    <div class="card">
      <h3><a href="https://github.com/shruthisree1234/Operational-Analytics-Warehouse">Data Warehouse for Operations</a></h3>
      <p>Modeled a star schema and ELT pipelines for operational analytics with conformed dimensions.</p>
      <div class="tags"><span class="tag">Snowflake</span><span class="tag">dbt</span><span class="tag">SQL</span></div>
    </div>
  </div>
</div>

<!-- Healthcare Analytics -->
<div class="subgroup">
  <h3>Healthcare Analytics</h3>
  <div class="cards">
    <div class="card">
      <h3><a href="https://github.com/shruthisree1234/Clinical-Data-Quality">Clinical Data Quality &amp; Validation</a></h3>
      <p>Automated checks for clinical datasets to reduce reporting errors and improve regulatory decision-making.</p>
      <div class="tags"><span class="tag">Python</span><span class="tag">Great Expectations</span><span class="tag">SQL</span></div>
    </div>
  </div>
</div>

<!-- Machine Learning & Visualization -->
<div class="subgroup">
  <h3>Machine Learning &amp; Visualization</h3>
  <div class="cards">
    <div class="card">
      <h3><a href="https://github.com/shruthisree1234/Regression_ML">Regression ML Pipeline</a></h3>
      <p>End-to-end PySpark pipeline for predicting vehicle MPG with feature engineering, model selection, and persistence.</p>
      <div class="tags"><span class="tag">PySpark</span><span class="tag">MLlib</span><span class="tag">Regression</span></div>
    </div>
    <div class="card">
      <h3><a href="https://github.com/shruthisree1234/Airfoil-Noise-Prediction">Airfoil Acoustic Performance</a></h3>
      <p>Predictive modeling of airfoil noise characteristics using regression and error analysis.</p>
      <div class="tags"><span class="tag">Python</span><span class="tag">SciPy</span><span class="tag">Regression</span></div>
    </div>
    <div class="card">
      <h3><a href="https://github.com/shruthisree1234/Sentiment-Analysis">Sentiment Analysis</a></h3>
      <p>Text classification for polarity using embeddings and interpretable features across domains.</p>
      <div class="tags"><span class="tag">NLP</span><span class="tag">Scikit-learn</span><span class="tag">Embeddings</span></div>
    </div>
    <div class="card">
      <h3><a href="https://github.com/shruthisree1234/Face-Mask-Detection">Face Mask Detection</a></h3>
      <p>Computer vision model to detect face-mask usage from images.</p>
      <div class="tags"><span class="tag">CNN</span><span class="tag">OpenCV</span><span class="tag">Keras</span></div>
    </div>
    <div class="card">
      <h3><a href="https://github.com/shruthisree1234/GUI-for-sorting-algorithms">Interactive Sorting Algorithms Visualizer</a></h3>
      <p>Interactive visualization to compare classic sorting algorithms and observe complexity behavior.</p>
      <div class="tags"><span class="tag">Python</span><span class="tag">Visualization</span></div>
    </div>
  </div>
</div>

<!-- Skills (anchor only, content unchanged) -->
<a id="skills"></a>
<h2>Skills</h2>
<p><strong>Data Engineering</strong><br>
Python, SQL, SparkSQL • Apache Spark, Hadoop, Airflow, Kafka • Data pipeline automation, ETL workflows, real-time streaming</p>
<p><strong>Analytics &amp; Business Intelligence</strong><br>
Tableau, Power BI • Data modeling, dashboard development, reporting, exploratory analysis • Machine Learning: LSTM, Bayesian models, anomaly detection, forecasting</p>
<p><strong>Databases</strong><br>
PostgreSQL, MongoDB, Redis • Data warehousing (Snowflake, Delta Lake), OLTP/OLAP systems</p>
<p><strong>Cloud &amp; DevOps</strong><br>
Azure, AWS • Databricks, Docker, Kubernetes • REST APIs, cloud automation, containerization</p>
<p><strong>Other Technical Skills</strong><br>
Git &amp; version control • Jupyter notebooks, SDLC practices • Data storytelling &amp; stakeholder communication</p>

<!-- Education (anchor only, content unchanged) -->
<a id="education"></a>
<h2>Education</h2>
<p><strong>Master of Science in Computer Engineering</strong><br>
University of Texas, Arlington (CGPA: 3.9/4)</p>

</div>

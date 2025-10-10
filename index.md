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

With 3+ years of experience in data analytics, data engineering, business insights, machine learning, and data storytelling, I specialize in designing and optimizing end-to-end solutions that deliver measurable results. My work enables teams to transform raw data into actionable intelligence, solve complex challenges, and drive strategic business decisions.

- ⚡ Expert in data modeling, analytics, and communicating insights through impactful storytelling
- 🛠️ Skilled in Python, SQL, Spark, Tableau, Power BI, and cloud platforms—delivering scalable and reliable solutions
- ✨ Proven collaborator and mentor, committed to supporting cross-functional teams and creating a culture of data-driven success
- 🚀 Passionate about leveraging technology and analytics to unlock new business opportunities


If you're looking for someone who combines deep technical expertise with business acumen and a knack for making data meaningful, let's connect.  I thrive on partnering to solve big challenges and deliver measurable results.

<div class="section-space"></div>

## Accomplishments

- 🚀 **Scalable Data Solutions**
  
  Engineered data pipelines using Spark, Kafka, and Azure, automating the flow of over 43 million telemetry events daily. This enabled real-time monitoring, faster decision-making, and supported expanded business capabilities.

  
- 📊 **Faster, Smarter Reporting**
  
  Designed and deployed Tableau/Power BI dashboards that cut manual reporting efforts by 40%. This gave business leaders instant access to actionable metrics, accelerating performance reviews and driving better decision making.

  
- 💡 **Reliable Data for Confident Decisions**
  
  Led warehouse validation and automated data checks, reducing reporting errors by 20%. Improved clinical data quality allowed teams to trust insights and make regulatory and operational decisions more securely.

  
- 🏆 **Downtime Slashed, Productivity Up**
  
  Built anomaly detection and forecasting models that helped the field team proactively prevent equipment failures, reducing downtime by 25%. This boosted operational reliability and drove cost savings for the company.

  
- 🤝 **Rapid Issue Resolution**

  Diagnosed and resolved data integration challenges across analytics and operations. By increasing pipeline reliability 18%, teams spent less time troubleshooting and more time delivering impactful work, directly supporting company growth.

  
- 🏆 **Influenced Executive Decision-Making**
  
  Designed and delivered tailored dashboards and predictive models for leadership, equipping executives with real-time metrics and actionable insights that directly improved quarterly strategic planning and resource investment.

  
- 🌐 **Built a Culture of Shared Success**
  
  Led peer learning calls and documented best practices, mentoring teammates in SQL, analytics, and reporting workflows. This leadership drove faster problem resolution and boosted team performance.


<div class="section-space"></div>

## Projects
<div style="margin-bottom: 30px;">
  <a href="https://github.com/shruthisree1234/SaaS_Churn_Prediction" style="text-decoration: none; color: inherit; display: block;">
    <div style="border: 1px solid #ddd; border-radius: 8px; overflow: hidden; box-shadow: 0 4px 8px rgba(0,0,0,0.1); transition: transform 0.2s; background-color: #ffffff;">
      <img src="images/churn-rate-1.jpg" alt="SaaS Churn Prediction" style="width: 100%; height:230px; object-fit:cover; display: block;" />
      <div style="padding: 20px; background-color: #f9f9f9;">
        <h3 style="margin: 0 0 10px 0; font-weight: bold;">SaaS Churn Prediction</h3>
        <p style="margin: 0; color: #666;">A deep-dive analytics project on SaaS KPIs: customer segmentation, churn, ARPU, margin, contracts, and marketing spend. Includes business recommendations driven by data and executive-level dashboards.</p>
      </div>
    </div>
  </a>
</div>

<div style="margin-bottom: 30px;">
  <a href="https://github.com/shruthisree1234/Data-Engineering-End-End-Project" style="text-decoration: none; color: inherit; display: block;">
    <div style="border: 1px solid #ddd; border-radius: 8px; overflow: hidden; box-shadow: 0 4px 8px rgba(0,0,0,0.1); transition: transform 0.2s; background-color: #ffffff;">
      <img src="images/Data pipeline.png" alt="End-to-End Data Pipeline" style="width: 100%; display: block;" />
      <div style="padding: 20px; background-color: #f9f9f9;">
        <h3 style="margin: 0 0 10px 0; font-weight: bold;">End-to-End Data Pipeline</h3>
        <p style="margin: 0; color: #666;">A comprehensive, real-world data platform project simulating retail analytics with MySQL, MongoDB, Hadoop, Spark, Airflow, IBM DB2, and more. Includes schema design, ETL automation, and dashboarding.</p>
      </div>
    </div>
  </a>
</div>

<div style="margin-bottom: 30px;">
  <a href="https://github.com/shruthisree1234/Bike_Rental_system" style="text-decoration: none; color: inherit; display: block;">
    <div style="border: 1px solid #ddd; border-radius: 8px; overflow: hidden; box-shadow: 0 4px 8px rgba(0,0,0,0.1); transition: transform 0.2s; background-color: #ffffff;">
      <img src="images/matched_bikerental (1).jpg" alt="Performance Monitoring and Visualization - Product Rental System" style="width: 100%; display: block;" />
      <div style="padding: 20px; background-color: #f9f9f9;">
        <h3 style="margin: 0 0 10px 0; font-weight: bold;">Performance Monitoring and Visualization - Product Rental System </h3>
        <p style="margin: 0; color: #666;">Database-driven bike rental management system designed to mirror the real-world operations of a vehicle rental business</p>
      </div>
    </div>
  </a>
</div>

<div style="margin-bottom: 30px;">
  <a href="https://github.com/shruthisree1234/DW-design-and-MQT" style="text-decoration: none; color: inherit; display: block;">
    <div style="border: 1px solid #ddd; border-radius: 8px; overflow: hidden; box-shadow: 0 4px 8px rgba(0,0,0,0.1); transition: transform 0.2s; background-color: #ffffff;">
      <img src="images/matched_operational.jpg" alt="Data Warehouse Design for Operational Analytics" style="width: 100%; display: block;" />
      <div style="padding: 20px; background-color: #f9f9f9;">
        <h3 style="margin: 0 0 10px 0; font-weight: bold;">Data Warehouse Design for Operational Analytics </h3>
        <p style="margin: 0; color: #666;">End-to-end design and implementation of a Data Warehouse for operation analytics</p>
      </div>
    </div>
  </a>
</div>

<div style="margin-bottom: 30px;">
  <a href="https://github.com/shruthisree1234/Airfoil-Noise-Prediction" style="text-decoration: none; color: inherit; display: block;">
    <div style="border: 1px solid #ddd; border-radius: 8px; overflow: hidden; box-shadow: 0 4px 8px rgba(0,0,0,0.1); transition: transform 0.2s; background-color: #ffffff;">
      <img src="images/matched_predictivemodeling.jpg" alt="Predictive Modeling of Airfoil Acoustic Performance" style="width: 100%; display: block;" />
      <div style="padding: 20px; background-color: #f9f9f9;">
        <h3 style="margin: 0 0 10px 0; font-weight: bold;">Predictive Modeling of Airfoil Acoustic Performance </h3>
        <p style="margin: 0; color: #666;">End-to-end machine learning pipeline for predicting the self-noise generated by airfoils using real-world data and Spark ML.</p>
      </div>
    </div>
  </a>
</div>

<div style="margin-bottom: 30px;">
  <a href="https://github.com/shruthisree1234/Sentiment-Analysis" style="text-decoration: none; color: inherit; display: block;">
    <div style="border: 1px solid #ddd; border-radius: 8px; overflow: hidden; box-shadow: 0 4px 8px rgba(0,0,0,0.1); transition: transform 0.2s; background-color: #ffffff;">
      <img src="images/matched_sentiment (1).jpg" alt="Sentiment Analysis" style="width: 100%; display: block;" />
      <div style="padding: 20px; background-color: #f9f9f9;">
        <h3 style="margin: 0 0 10px 0; font-weight: bold;">Sentiment Analysis </h3>
        <p style="margin: 0; color: #666;">Compares multiple machine learning and deep learning models (SVM, LSTM, and CNN) for automated sentiment classification of text. Each approach highlights different strengths in understanding sentiment from language data.</p>
      </div>
    </div>
  </a>
</div>

<div style="margin-bottom: 30px;">
  <a href="https://github.com/shruthisree1234/Face_mask_detection" style="text-decoration: none; color: inherit; display: block;">
    <div style="border: 1px solid #ddd; border-radius: 8px; overflow: hidden; box-shadow: 0 4px 8px rgba(0,0,0,0.1); transition: transform 0.2s; background-color: #ffffff;">
      <img src="images/matched_face mask.jpg" alt="Face mask detection" style="width: 100%; display: block;" />
      <div style="padding: 20px; background-color: #f9f9f9;">
        <h3 style="margin: 0 0 10px 0; font-weight: bold;">Face mask detection </h3>
        <p style="margin: 0; color: #666;">Implements and compares deep learning models for real-time face mask detection using computer vision. The focus is on building efficient pipelines for recognizing whether individuals in images or video streams are wearing face masks for public health and safety.</p>
      </div>
    </div>
  </a>
</div>


<div style="margin-bottom: 30px;">
  <a href="https://github.com/shruthisree1234/Regression_ML" style="text-decoration: none; color: inherit; display: block;">
    <div style="border: 1px solid #ddd; border-radius: 8px; overflow: hidden; box-shadow: 0 4px 8px rgba(0,0,0,0.1); transition: transform 0.2s; background-color: #ffffff;">
      <img src="images/matched_regresssion_ML.jpg" alt="Regression ML Pipeline" style="width: 100%; display: block;" />
      <div style="padding: 20px; background-color: #f9f9f9;">
        <h3 style="margin: 0 0 10px 0; font-weight: bold;">Regression ML Pipeline </h3>
        <p style="margin: 0; color: #666;">A complete machine learning pipeline using PySpark to predict car mileage (MPG) from multidimensional automotive data. Designed with a focus on real-world data engineering, the workflow bridges robust ETL, advanced regression modeling, performance evaluation, and production model persistence—showing how scalable data science is applied in industry.</p>
      </div>
    </div>
  </a>
</div>

<div style="margin-bottom: 30px;">
  <a href="https://github.com/shruthisree1234/GUI-for-sorting-algorithms" style="text-decoration: none; color: inherit; display: block;">
    <div style="border: 1px solid #ddd; border-radius: 8px; overflow: hidden; box-shadow: 0 4px 8px rgba(0,0,0,0.1); transition: transform 0.2s; background-color: #ffffff;">
      <img src="images/matched_algovisual.jpg" alt="Interactive Sorting Algorithms Visualizer" style="width: 100%; display: block;" />
      <div style="padding: 20px; background-color: #f9f9f9;">
        <h3 style="margin: 0 0 10px 0; font-weight: bold;">Interactive Sorting Algorithms Visualizer </h3>
        <p style="margin: 0; color: #666;">a graphical user interface (GUI) tool for visualizing and comparing classic sorting algorithms in real time. It helps users understand, analyze, and benchmark the inner workings of sorting methods.</p>
      </div>
    </div>
  </a>
</div>


<div class="section-space"></div>

## Skills

**Data Engineering**
- Python, SQL, SparkSQL
- Apache Spark, Hadoop, Airflow, Kafka
- Data pipeline automation, ETL workflows, real-time streaming

**Analytics & Business Intelligence**
- Tableau, Power BI
- Data modeling, dashboard development, reporting, exploratory analysis
- Machine Learning: LSTM, Bayesian models, anomaly detection, forecasting

**Databases**
- PostgreSQL, MongoDB, Redis
- Data warehousing (Snowflake, Delta Lake), OLTP/OLAP systems

**Cloud & DevOps**
- Azure, AWS
- Databricks, Docker, Kubernetes
- REST APIs, cloud automation, containerization

**Other Technical Skills**
- Git & version control
- Jupyter notebooks, SDLC practices
- Data storytelling & stakeholder communication


<div class="section-space"></div>

## Education

**Master of Science in Computer Engineering** 

University of Texas, Arlington  (CGPA : 3.9/4)


<!--
  Profile README for github.com/Arrkkkk
  ─────────────────────────────────────
  Palette   ink #0D1117 · amber #F4B740 (dark) / #9A6700 (light) · text #C9D1D9
  Assets    assets/hero-*.svg     hero banner (dark + light variants, keep in sync)
            assets/icons/*.svg    tech tiles (skillicons.dev style, stored locally)
  Live      GitHub stats, streak and activity graph are fetched on every view.
-->

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/hero-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="assets/hero-light.svg">
  <img src="assets/hero-dark.svg" width="100%" alt="Rajit Agrawal: building dependable software where AI meets finance. B.Tech CSE at VIT Vellore, class of 2027, CGPA 9.74.">
</picture>

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=18&duration=2800&pause=900&color=F4B740&center=true&vCenter=true&width=560&lines=AI+Intern+%C2%B7+Deloitte;Python+%C2%B7+Java+%C2%B7+React+%C2%B7+Flutter;Exploring+cloud+data+with+AWS+%26+Databricks;Open-source+contributor+%C2%B7+GSSoC">
    <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=18&duration=2800&pause=900&color=9A6700&center=true&vCenter=true&width=560&lines=AI+Intern+%C2%B7+Deloitte;Python+%C2%B7+Java+%C2%B7+React+%C2%B7+Flutter;Exploring+cloud+data+with+AWS+%26+Databricks;Open-source+contributor+%C2%B7+GSSoC" alt="AI Intern at Deloitte · Python, Java, React, Flutter · Exploring cloud data with AWS and Databricks · Open-source contributor at GSSoC">
  </picture>
</p>

<p align="center">
  <a href="https://portfolio-fawn-delta-90.vercel.app">Portfolio</a> &nbsp;·&nbsp;
  <a href="https://www.linkedin.com/in/rajit-agrawal-639bab28a/">LinkedIn</a> &nbsp;·&nbsp;
  <a href="mailto:rajitagrawal2005@gmail.com">Email</a>
</p>

## `01` About

I'm a Computer Science undergraduate at **VIT Vellore** (B.Tech, class of 2027, CGPA 9.74). Most of what I build sits where software meets finance: market dashboards, a budgeting assistant, and a decentralised quant-trading fund. Finance is a domain where "mostly works" isn't good enough, and that's exactly why I like building for it.

I care about the parts of engineering that make software trustworthy. **MarketPulse** started as a Streamlit app that turned every failure into an empty result, so a rate-limit error showed up as "no news found". I rebuilt it as a layered FastAPI service with typed errors, circuit breakers and caching, backed by 455 tests.

My internships span AI at **Deloitte**, software testing in the capital-markets domain at **AQM Technologies**, and web development at **ApexPlanet**, and I contribute to open source through **GirlScript Summer of Code**. Right now I'm going deeper into applied AI and cloud data platforms.

## `02` Featured work

<table>
  <tr>
    <td colspan="2" valign="top">
      <h3><a href="https://github.com/Arrkkkk/MarketPulse">MarketPulse</a></h3>
      <p>Real-time stock and crypto dashboard with news aggregation and AI-generated sentiment analysis, built as a FastAPI service behind a thin Streamlit client.</p>
      <ul>
        <li><b>Fails loudly, not silently.</b> Providers raise typed errors (<code>RateLimited</code>, <code>SymbolNotFound</code>, …) that map onto proper HTTP status codes, so an outage is never shown to users as "no data".</li>
        <li><b>Resilient data layer.</b> Retries, a circuit breaker, rate limiting and a memory → SQLite cache that only stores successful responses.</li>
        <li><b>Architecture that can't quietly rot.</b> <code>import-linter</code> contracts enforce the layering in CI; 455 tests at 92% coverage.</li>
      </ul>
      <p>
        <code>Python</code> <code>FastAPI</code> <code>Streamlit</code> <code>Gemini API</code> <code>SQLite</code> <code>Docker</code>
        &nbsp;&nbsp;→&nbsp;<a href="https://github.com/Arrkkkk/MarketPulse"><b>Repository</b></a>
      </p>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3>QuantChain</h3>
      <p>A decentralised, AI-driven quant-trading fund that combines machine-learning trading models with blockchain-based fund management.</p>
      <p><code>Machine Learning</code> <code>Blockchain</code></p>
      <!-- TODO: replace with the real link once the repository is public:
           <a href="https://github.com/Arrkkkk/REPO_NAME"><b>Repository</b></a> -->
      <p><sub>Repository coming soon</sub></p>
    </td>
    <td width="50%" valign="top">
      <h3><a href="https://github.com/Arrkkkk/Multi-AI-Chatbot">Multi AI Chatbot</a></h3>
      <p>One chat interface for four model providers (Claude, OpenAI, Gemini and Groq). Pick a provider, bring your own API key, and chat.</p>
      <p><code>Python</code> <code>Streamlit</code> <code>LLM APIs</code></p>
      <p>→&nbsp;<a href="https://github.com/Arrkkkk/Multi-AI-Chatbot"><b>Repository</b></a></p>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3><a href="https://github.com/Arrkkkk/Personal-Finance-Tip-Generator-by-Axtech">Personal Finance Tip Generator</a></h3>
      <p>Enter your monthly income, expenses and savings goal, and Gemini turns them into tailored budgeting advice. Runs entirely in the browser.</p>
      <p><code>HTML</code> <code>CSS</code> <code>JavaScript</code> <code>Gemini API</code></p>
      <p>→&nbsp;<a href="https://arrkkkk.github.io/Personal-Finance-Tip-Generator-by-Axtech/"><b>Live demo</b></a> &nbsp;·&nbsp; <a href="https://github.com/Arrkkkk/Personal-Finance-Tip-Generator-by-Axtech"><b>Repository</b></a></p>
    </td>
    <td width="50%" valign="top">
      <h3><a href="https://github.com/Arrkkkk/schedsim">SchedSim</a></h3>
      <p>Interactive CPU-scheduling simulator: FCFS through MLFQ, with Gantt charts, step-by-step traces, side-by-side comparison and PDF/CSV export.</p>
      <p><code>Flutter</code> <code>Dart</code> <code>Riverpod</code></p>
      <p>→&nbsp;<a href="https://github.com/Arrkkkk/schedsim"><b>Repository</b></a></p>
    </td>
  </tr>
</table>

## `03` Tech stack

<table>
  <tr>
    <td width="150"><b>Languages</b></td>
    <td>
      <img src="assets/icons/c.svg" width="40" height="40" alt="C" title="C">
      <img src="assets/icons/cpp.svg" width="40" height="40" alt="C++" title="C++">
      <img src="assets/icons/java.svg" width="40" height="40" alt="Java" title="Java">
      <img src="assets/icons/py.svg" width="40" height="40" alt="Python" title="Python">
      <img src="assets/icons/js.svg" width="40" height="40" alt="JavaScript" title="JavaScript">
      <img src="assets/icons/dart.svg" width="40" height="40" alt="Dart" title="Dart">
    </td>
  </tr>
  <tr>
    <td><b>Frontend &amp; mobile</b></td>
    <td>
      <img src="assets/icons/html.svg" width="40" height="40" alt="HTML" title="HTML">
      <img src="assets/icons/css.svg" width="40" height="40" alt="CSS" title="CSS">
      <img src="assets/icons/react.svg" width="40" height="40" alt="React" title="React">
      <img src="assets/icons/flutter.svg" width="40" height="40" alt="Flutter" title="Flutter">
    </td>
  </tr>
  <tr>
    <td><b>Backend &amp; APIs</b></td>
    <td>
      <img src="assets/icons/fastapi.svg" width="40" height="40" alt="FastAPI" title="FastAPI">
      <img src="assets/icons/streamlit.svg" width="40" height="40" alt="Streamlit" title="Streamlit">
      <img src="assets/icons/postman.svg" width="40" height="40" alt="Postman" title="Postman">
      &nbsp;<sub>REST APIs</sub>
    </td>
  </tr>
  <tr>
    <td><b>AI &amp; data science</b></td>
    <td>
      <img src="assets/icons/numpy.svg" width="40" height="40" alt="NumPy" title="NumPy">
      <img src="assets/icons/pandas.svg" width="40" height="40" alt="Pandas" title="Pandas">
      <img src="assets/icons/matplotlib.svg" width="40" height="40" alt="Matplotlib" title="Matplotlib">
      <img src="assets/icons/gemini.svg" width="40" height="40" alt="Google Gemini" title="Google Gemini API">
      &nbsp;<sub>Generative AI · LLM APIs</sub>
    </td>
  </tr>
  <tr>
    <td><b>Cloud &amp; data</b></td>
    <td>
      <img src="assets/icons/aws.svg" width="40" height="40" alt="AWS" title="AWS">
      <img src="assets/icons/databricks.svg" width="40" height="40" alt="Databricks" title="Databricks">
      &nbsp;<sub>Delta Lake · Unity Catalog</sub>
    </td>
  </tr>
  <tr>
    <td><b>Databases &amp; tools</b></td>
    <td>
      <img src="assets/icons/mysql.svg" width="40" height="40" alt="MySQL" title="MySQL">
      <img src="assets/icons/git.svg" width="40" height="40" alt="Git" title="Git">
      <img src="assets/icons/github.svg" width="40" height="40" alt="GitHub" title="GitHub">
    </td>
  </tr>
</table>

## `04` Experience & credentials

<table>
  <tr>
    <th width="50%" align="left">Experience</th>
    <th width="50%" align="left">Certifications</th>
  </tr>
  <tr>
    <td valign="top">
      <b>AI Intern</b><br>
      <sub>Deloitte</sub><br><br>
      <b>Software Testing Intern</b><br>
      <sub>AQM Technologies · Capital-markets domain</sub><br><br>
      <b>Web Development Intern</b><br>
      <sub>ApexPlanet Software Pvt. Ltd.</sub><br><br>
      <b>Open Source Contributor</b><br>
      <sub>GirlScript Summer of Code</sub>
    </td>
    <td valign="top">
      <b>Generative AI Professional (2025)</b><br>
      <sub>Oracle Cloud Infrastructure</sub><br><br>
      <b>API Fundamentals Student Expert</b><br>
      <sub>Postman</sub><br><br>
      <b>Generative AI using IBM watsonx</b> · <b>Agile Explorer</b><br>
      <sub>IBM</sub><br><br>
      <b>Databricks Fundamentals</b> · <b>AWS Cloud Essentials</b><br>
      <sub>Databricks · Amazon Web Services</sub>
    </td>
  </tr>
  <tr>
    <td colspan="2">
      <b>Honours</b>&nbsp;&nbsp;National Space Hackathon 2025 &nbsp;·&nbsp; VIT Merit Awards &nbsp;·&nbsp; CGPA 9.74 / 10
    </td>
  </tr>
</table>

## `05` GitHub activity

<p align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=Arrkkkk&show_icons=true&include_all_commits=true&hide_rank=true&custom_title=GitHub%20Stats&bg_color=0D1117&title_color=F4B740&icon_color=F4B740&text_color=C9D1D9&hide_border=true&border_radius=10" alt="Rajit's GitHub stats">
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Arrkkkk&layout=compact&langs_count=6&hide=cmake,shell,makefile,ruby,swift,kotlin,objective-c,dockerfile&custom_title=Most%20Used%20Languages&bg_color=0D1117&title_color=F4B740&icon_color=F4B740&text_color=C9D1D9&hide_border=true&border_radius=10" alt="Most used languages">
</p>

<p align="center">
  <img src="https://streak-stats.demolab.com?user=Arrkkkk&hide_border=true&border_radius=10&background=0D1117&stroke=30363D&ring=F4B740&fire=F4B740&currStreakNum=F4B740&currStreakLabel=F4B740&sideNums=E6EDF3&sideLabels=C9D1D9&dates=8B949E" alt="GitHub contribution streak">
</p>

<p align="center">
  <img width="100%" src="https://github-readme-activity-graph.vercel.app/graph?username=Arrkkkk&bg_color=0D1117&color=C9D1D9&title_color=F4B740&line=F4B740&point=E6EDF3&area=true&area_color=F4B740&hide_border=true&radius=10&custom_title=Contribution%20activity" alt="Contribution activity graph">
</p>

## `06` Connect

<p>
  <a href="https://portfolio-fawn-delta-90.vercel.app"><img src="https://img.shields.io/badge/Portfolio-0D1117?style=for-the-badge&logo=vercel&logoColor=F4B740" alt="Portfolio"></a>
  <a href="https://www.linkedin.com/in/rajit-agrawal-639bab28a/"><img src="https://img.shields.io/badge/LinkedIn-0D1117?style=for-the-badge&logo=data:image/svg%2bxml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI+PHBhdGggZmlsbD0iI0Y0Qjc0MCIgZD0iTTIwLjQ0NyAyMC40NTJoLTMuNTU0di01LjU2OWMwLTEuMzI4LS4wMjctMy4wMzctMS44NTItMy4wMzctMS44NTMgMC0yLjEzNiAxLjQ0NS0yLjEzNiAyLjkzOXY1LjY2N0g5LjM1MVY5aDMuNDE0djEuNTYxaC4wNDZjLjQ3Ny0uOSAxLjYzNy0xLjg1IDMuMzctMS44NSAzLjYwMSAwIDQuMjY3IDIuMzcgNC4yNjcgNS40NTV2Ni4yODZ6TTUuMzM3IDcuNDMzYy0xLjE0NCAwLTIuMDYzLS45MjYtMi4wNjMtMi4wNjUgMC0xLjEzOC45Mi0yLjA2MyAyLjA2My0yLjA2MyAxLjE0IDAgMi4wNjQuOTI1IDIuMDY0IDIuMDYzIDAgMS4xMzktLjkyNSAyLjA2NS0yLjA2NCAyLjA2NXptMS43ODIgMTMuMDE5SDMuNTU1VjloMy41NjR2MTEuNDUyek0yMi4yMjUgMEgxLjc3MUMuNzkyIDAgMCAuNzc0IDAgMS43Mjl2MjAuNTQyQzAgMjMuMjI3Ljc5MiAyNCAxLjc3MSAyNGgyMC40NTFDMjMuMiAyNCAyNCAyMy4yMjcgMjQgMjIuMjcxVjEuNzI5QzI0IC43NzQgMjMuMiAwIDIyLjIyMiAwaC4wMDN6Ii8+PC9zdmc+" alt="LinkedIn"></a>
  <a href="mailto:rajitagrawal2005@gmail.com"><img src="https://img.shields.io/badge/Email-0D1117?style=for-the-badge&logo=gmail&logoColor=F4B740" alt="Email"></a>
  <a href="https://github.com/Arrkkkk"><img src="https://img.shields.io/badge/GitHub-0D1117?style=for-the-badge&logo=github&logoColor=F4B740" alt="GitHub"></a>
  <a href="https://leetcode.com/u/RA_Ark/"><img src="https://img.shields.io/badge/LeetCode-0D1117?style=for-the-badge&logo=leetcode&logoColor=F4B740" alt="LeetCode"></a>
</p>

Email or LinkedIn is the quickest way to reach me. I'm always glad to talk about software, AI and fintech.

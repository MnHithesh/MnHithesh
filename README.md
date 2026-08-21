<h1 align="center">Hithesh M N</h1>

<p align="center">
  <b>Senior Frontend Engineer</b> · Angular · React · Micro Frontends<br/>
  8+ years building and scaling production web applications.<br/>
  Currently leading frontend architecture on a live crypto trading platform.
</p>

<p align="center">
  <a href="https://hitheshmn.prehinix.com/"><img src="https://img.shields.io/badge/Portfolio-hitheshmn.prehinix.com-000000?style=for-the-badge&logo=vercel&logoColor=white" alt="Portfolio"/></a>
  <a href="https://linkedin.com/in/hithesh-nandeesh"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="mailto:m.n.hithesh26@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
  <a href="https://stackoverflow.com/users/8815586"><img src="https://img.shields.io/badge/Stack%20Overflow-FE7A16?style=for-the-badge&logo=stackoverflow&logoColor=white" alt="Stack Overflow"/></a>
</p>

---

### 👨‍💻 About

I own features end to end — interface through backend services to deployment. Most of my depth is in **Angular (v6 → v22)** and **RxJS-driven real-time systems**: WebSocket market data pipelines, TradingView chart integrations, custom HTML5 Canvas visualisations, and change-detection tuning on data-heavy screens.

- 🏗️ Architecting a cross-platform **Ionic** trading app as sole frontend developer
- 🧬 Building **micro frontend** systems with Module Federation across mismatched bundlers
- 📱 Shipping offline-first mobile apps with **Angular 22 + Capacitor**
- 🤖 Building AI automation pipelines with **n8n** and LLM APIs outside client work
- 🌱 Currently learning **RabbitMQ** and **React Native**
- 📍 Bengaluru, India · 📫 **m.n.hithesh26@gmail.com**

---

### 🚀 Projects

#### 🔷 [Personal Portfolio — Micro Frontend Architecture](https://hitheshmn.prehinix.com/)

Not a template. Built from scratch as a **micro frontend system**: an Angular shell owns routing, layout, and lifecycle, while a React remote is built independently in Vite and loaded at runtime via **Module Federation**.

The interesting part is the bundler bridge — a Webpack-based Angular host consuming a pure-ESM Vite bundle, with explicit mount/unmount boundaries and no shared global state. Motion and smooth scroll handled with GSAP and Lenis.

`Angular` `React` `Vite` `Webpack Module Federation` `GSAP` `Lenis`

#### 👕 [Dresscode — Offline-First Wardrobe App](https://github.com/MnHithesh/dresscode-mobile)

An Android wardrobe manager built on **Angular 22 and Capacitor 8**, running entirely on-device. Catalogue your closet from camera captures, inspiration shots, tag scans, or receipts; build and save looks; get outfit suggestions and wear-pattern insights.

Fully local persistence via SQLite (`@capacitor-community/sqlite` on device, `sql.js` + `jeep-sqlite` in the browser), bootstrapped through Angular's `provideAppInitializer` so the database and preferences are ready before the first route resolves. Standalone components with lazy-loaded routes throughout.

`Angular 22` `Capacitor 8` `SQLite` `TypeScript` `RxJS` `Vitest`

#### 🎯 [JobFit AI — Automated Resume Tailor Agent](https://github.com/MnHithesh/ai-resume-tailor-agent)

An end-to-end automation pipeline that watches Gmail for recruiter emails, extracts the job description with Gemini, and produces a tailored ATS-optimised resume in under 60 seconds — then pushes an ATS match score, matched/missing skills, and improvement notes to Discord.

Three-stage pipeline (JD extraction → tailoring → ATS scoring) with prompt constraints that let the model reorder and reprioritise existing content but never invent experience.

`n8n` `Google Gemini API` `Node.js` `Gmail IMAP` `Discord Webhooks`

#### ⏰ [Task Reminder — Self-Hosted Reminder Service](https://github.com/MnHithesh/task-remainder)

A reminder service that actually reaches you. Browser notifications die when the browser closes, so delivery runs through a Discord bot on the server instead — an outbound WebSocket that needs no public URL, no open port, and no TLS, so it works behind a home router. Reminders arrive as interactive embeds with action buttons, routed to separate work and personal channels, with follow-up chasing for anything left unacknowledged.

Persistence uses Node's built-in `node:sqlite` rather than `better-sqlite3`, deliberately avoiding native compilation and the ABI breakage that comes with every Node release. Discord delivery degrades gracefully — drop the token and the rest of the service runs unchanged.

`Node.js 24` `node:sqlite` `discord.js` `ESM`

#### 💰 DuoBudget — Shared Budget Tracker for Couples

Shared expense tracking, cost splitting, and joint financial goals, with an OpenAI-powered assistant that analyses spending patterns and returns personalised suggestions.

[Frontend](https://github.com/MnHithesh/duobudget_frontend) · [Backend](https://github.com/MnHithesh/duobudget_backend)

`React` `Node.js` `Express` `OpenAI API`

---

### 🛠️ Tech Stack

**Frontend**

![Angular](https://img.shields.io/badge/Angular-DD0031?style=flat-square&logo=angular&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=flat-square&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-323330?style=flat-square&logo=javascript&logoColor=F7DF1E)
![RxJS](https://img.shields.io/badge/RxJS-B7178C?style=flat-square&logo=reactivex&logoColor=white)
![SCSS](https://img.shields.io/badge/SCSS-CC6699?style=flat-square&logo=sass&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![Bootstrap](https://img.shields.io/badge/Bootstrap-7952B3?style=flat-square&logo=bootstrap&logoColor=white)

**Architecture**

![Module Federation](https://img.shields.io/badge/Module_Federation-1B73BA?style=flat-square&logo=webpack&logoColor=white)
![Webpack](https://img.shields.io/badge/Webpack-8DD6F9?style=flat-square&logo=webpack&logoColor=black)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white)
![Micro Frontends](https://img.shields.io/badge/Micro_Frontends-4B32C3?style=flat-square)

**Charting & Visualisation**

![TradingView](https://img.shields.io/badge/TradingView-131722?style=flat-square&logo=tradingview&logoColor=white)
![Highcharts](https://img.shields.io/badge/Highcharts-8087E8?style=flat-square&logo=highcharts&logoColor=white)
![Plotly](https://img.shields.io/badge/Plotly-3F4F75?style=flat-square&logo=plotly&logoColor=white)
![Canvas](https://img.shields.io/badge/HTML5_Canvas-E34F26?style=flat-square&logo=html5&logoColor=white)

**Backend & Data**

![Node.js](https://img.shields.io/badge/Node.js-6DA55F?style=flat-square&logo=node.js&logoColor=white)
![Express](https://img.shields.io/badge/Express-404D59?style=flat-square&logo=express&logoColor=61DAFB)
![MongoDB](https://img.shields.io/badge/MongoDB-4EA94B?style=flat-square&logo=mongodb&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)
![WebSockets](https://img.shields.io/badge/WebSockets-010101?style=flat-square&logo=socketdotio&logoColor=white)
![Puppeteer](https://img.shields.io/badge/Puppeteer-40B5A4?style=flat-square&logo=puppeteer&logoColor=white)

**Mobile, Cloud & Tools**

![Capacitor](https://img.shields.io/badge/Capacitor-119EFF?style=flat-square&logo=capacitor&logoColor=white)
![Ionic](https://img.shields.io/badge/Ionic-3880FF?style=flat-square&logo=ionic&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-FF9900?style=flat-square&logo=amazonwebservices&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![n8n](https://img.shields.io/badge/n8n-EA4B71?style=flat-square&logo=n8n&logoColor=white)
![Figma](https://img.shields.io/badge/Figma-F24E1E?style=flat-square&logo=figma&logoColor=white)

---

### 📊 GitHub Stats

<p align="center">
  <img width="49%" src="https://github-readme-stats.vercel.app/api?username=MnHithesh&show_icons=true&theme=shadow_blue&hide_border=true&include_all_commits=true&count_private=true" alt="GitHub Stats"/>
  <img width="41%" src="https://github-readme-stats.vercel.app/api/top-langs/?username=MnHithesh&theme=shadow_blue&hide_border=true&include_all_commits=true&count_private=true&layout=compact" alt="Top Languages"/>
</p>

<p align="center">
  <img width="60%" src="https://streak-stats.demolab.com?user=MnHithesh&theme=shadow_blue&hide_border=true" alt="GitHub Streak"/>
</p>

---

<p align="center">
  <i>Open to conversations about frontend architecture, real-time systems, and micro frontends.</i><br/>
  <a href="https://hitheshmn.prehinix.com/"><b>hitheshmn.prehinix.com</b></a>
</p>

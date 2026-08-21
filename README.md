<!-- ══════════════════════ HEADER ══════════════════════ -->

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:0F2027,50:203A43,100:2C5364&height=200&section=header&text=Hithesh%20M%20N&fontColor=ffffff&fontSize=52&fontAlignY=34&desc=Senior%20Frontend%20Engineer%20%C2%B7%20Angular%20%C2%B7%20Micro%20Frontends&descAlignY=54&descSize=16&animation=fadeIn" alt="header"/>

<p align="center">
  <a href="https://hitheshmn.prehinix.com/">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=20&duration=3000&pause=900&color=64B5F6&center=true&vCenter=true&width=800&height=45&lines=8%2B+years+shipping+production+web+applications;Real-time+trading+platforms+%26+WebSocket+pipelines;Module+Federation+across+mismatched+bundlers;Angular+v6+%E2%86%92+v22+%C2%B7+migrations%2C+architecture%2C+performance" alt="Typing SVG"/>
  </a>
</p>

<p align="center">
  <a href="https://hitheshmn.prehinix.com/"><img src="https://img.shields.io/badge/Portfolio-0F2027?style=for-the-badge&logo=vercel&logoColor=64B5F6" alt="Portfolio"/></a>
  <a href="https://linkedin.com/in/hithesh-nandeesh"><img src="https://img.shields.io/badge/LinkedIn-0F2027?style=for-the-badge&logo=linkedin&logoColor=0A66C2" alt="LinkedIn"/></a>
  <a href="mailto:m.n.hithesh26@gmail.com"><img src="https://img.shields.io/badge/Email-0F2027?style=for-the-badge&logo=gmail&logoColor=EA4335" alt="Email"/></a>
  <a href="https://stackoverflow.com/users/8815586"><img src="https://img.shields.io/badge/Stack_Overflow-0F2027?style=for-the-badge&logo=stackoverflow&logoColor=F48024" alt="Stack Overflow"/></a>
  <img src="https://komarev.com/ghpvc/?username=MnHithesh&style=for-the-badge&color=203A43&label=PROFILE+VIEWS" alt="views"/>
</p>

<br/>

<!-- ══════════════════════ ABOUT ══════════════════════ -->

## About

<table>
<tr>
<td width="30%" align="center" valign="middle">
  <img src="hithesh-avatar-circle.png" width="190" alt="Hithesh M N"/>
  <br/><br/>
  <b>Hithesh M N</b><br/>
  <sub>Bengaluru, India 🇮🇳</sub>
</td>
<td width="70%" valign="middle">

```ts
const hithesh: Engineer = {
  role:      'Senior Frontend Developer & Tech Lead',
  focus:     ['Angular v6 → v22', 'RxJS', 'Micro Frontends'],
  building:  'a cross-platform Ionic trading app — sole dev',
  ownership: 'interface → backend services → deployment',
};
```

I work on production systems where the frontend is the hard part — live market data, charts that redraw many times a second, and trading logic that has to be exactly right.

I own features end to end rather than handing off at the API boundary, which means the backend services, the deployment and the mobile shell too when that's what the feature needs.

</td>
</tr>
</table>

<br/>

<!-- ══════════════════════ FEATURES ══════════════════════ -->

## ⚡ Features I've Built

<table>
<tr>
<td width="50%" valign="top">

### 📈 TradingView Chart Integration

Wired the TradingView Charting Library into a live crypto exchange — implementing the datafeed adapter so historical bars, real-time ticks and resolution changes all resolve from the same source of truth.

The difficult part was **feed synchronisation**: reconciling REST history with a WebSocket stream that keeps arriving during the fetch, so bars don't duplicate or gap at the seam when a user switches symbol or timeframe.

`TradingView` `WebSockets` `RxJS` `Angular`

</td>
<td width="50%" valign="top">

### 🫧 HTML5 Canvas Bubble Visualisation

Built a crypto market-overview bubble chart from scratch on raw Canvas — no charting library — because nothing off the shelf handled hundreds of continuously resizing, repositioning bubbles at an acceptable frame rate.

Bubble radius is driven by a **dynamic sizing algorithm** over live market data, with RxJS streams feeding updates into the render loop and drawing decoupled from data arrival so the canvas stays smooth under bursty feeds.

`Canvas API` `RxJS` `TypeScript`

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🔁 Copy Trading Module

Owned end to end: the system that mirrors one trader's positions into follower accounts automatically.

Designed the **shared service architecture** and reactive data flows behind it, plus trade configuration management and the business-rule validation layer that decides whether a mirrored order is allowed to execute — sizing limits, instrument eligibility and account state, evaluated before anything reaches the exchange.

`Angular` `RxJS` `Node.js`

</td>
<td width="50%" valign="top">

### 📊 Real-Time Market Trend Analytics

A module turning raw market movement into readable trading signals, combining custom **sentiment-analysis logic** with Highcharts visualisations.

The engineering constraint was render cost: data arrives continuously, so I used **OnPush change detection** with RxJS-driven orchestration to keep Angular from re-checking the whole component tree on every tick.

`Highcharts` `RxJS` `OnPush` `Angular`

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🔔 Full-Stack Alerting System

Users configure price and percentage-based alerts on any instrument; the backend evaluates trigger conditions against live data and dispatches **email and SMS** notifications when they fire.

Built both halves — the configuration UI and the server-side evaluation and dispatch logic, including the conditions that decide when an alert has genuinely triggered rather than flickered across a threshold.

`Node.js` `Express` `MongoDB` `Angular`

</td>
<td width="50%" valign="top">

### ⚙️ Futures Execution Engine

Re-engineered the futures order engine after breaking upstream **IIFL API changes**, preserving custom order-generation logic that the business depended on.

That logic covers price calculation, quantity distribution across legs, and generating **single-leg, double-leg and four-leg** orders — strategies where every leg must be priced and sized correctly relative to the others or the position is wrong.

`Node.js` `REST APIs` `TypeScript`

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🧬 Micro Frontend Architecture

An Angular shell owning routing, layout and lifecycle, with a React remote built independently in Vite and loaded at runtime through **Module Federation**.

The interesting problem is the bundler bridge — a Webpack-based host consuming a pure-ESM Vite bundle — solved with explicit mount/unmount boundaries and no shared global state, so either side can be rebuilt and deployed without touching the other.

`Module Federation` `Webpack` `Vite` `Angular` `React`

</td>
<td width="50%" valign="top">

### 🔄 Angular 6 → 12 Migration

Planned and executed a phased migration across **20+ modules and screens**, solo, on a platform that had to stay live throughout.

Beyond the version bump: upgrading Angular Material, untangling third-party dependency conflicts, then modernising the architecture underneath — lazy loading, modular restructuring and reusable component design, so the codebase was better afterwards rather than merely newer.

`Angular` `Angular Material` `Webpack`

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🕸️ Puppeteer Price Pipeline

Backend service for limit-order processing that retrieves **live NSE pricing** via Puppeteer where no API was available, and generates broker-ready trading orders from it.

Headless scraping in a trading path means handling stale reads and page-structure changes carefully — a wrong price here produces a real order.

`Puppeteer` `Node.js`

</td>
<td width="50%" valign="top">

### 🎯 Canvas for Computer Vision

On an AI/ML platform, built Canvas components rendering **spatial data, object positions and coordinate overlays** on top of model output, so clients could visually interpret detection and tracking results in real time.

Paired with Plotly.js analytics dashboards for monitoring model performance and prediction results.

`Canvas API` `Plotly.js` `Angular` `RxJS`

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🔐 RBAC & Permission Workflows

Role-based access control across recruiters, managers, sales and leadership on a CRM platform — with role-specific data visibility, so the same screen shows different records depending on who's looking.

Backed by **RxJS state management** tracking recruitment workflow state, and frontend caching to cut redundant API calls on data-heavy modules.

`Angular` `RxJS` `Node.js` `MongoDB`

</td>
<td width="50%" valign="top">

### 📱 Offline-First Mobile

A wardrobe app on **Angular 22 + Capacitor 8** running entirely on-device with no backend — SQLite persistence with a browser fallback, bootstrapped through `provideAppInitializer` so the database resolves before the first route.

Currently sole frontend developer on a cross-platform **Ionic trading app**: market monitoring, trading workflows, portfolio tracking and API integration.

`Capacitor` `Ionic` `SQLite` `Angular 22`

</td>
</tr>
</table>

<br/>

<!-- ══════════════════════ STACK ══════════════════════ -->

## 🧰 Tech Stack

<p align="center">
  <img src="https://skillicons.dev/icons?i=angular,react,ts,js,html,css,sass,bootstrap&theme=dark" alt="frontend"/><br/>
  <img src="https://skillicons.dev/icons?i=nodejs,express,mongodb,sqlite,docker,aws,git,github&theme=dark" alt="backend"/><br/>
  <img src="https://skillicons.dev/icons?i=vite,webpack,ionic,figma,postman,python,vscode&theme=dark" alt="tools"/>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/RxJS-1a1b27?style=flat-square&logo=reactivex&logoColor=B7178C" alt="RxJS"/>
  <img src="https://img.shields.io/badge/Module_Federation-1a1b27?style=flat-square&logo=webpack&logoColor=8DD6F9" alt="Module Federation"/>
  <img src="https://img.shields.io/badge/Capacitor-1a1b27?style=flat-square&logo=capacitor&logoColor=119EFF" alt="Capacitor"/>
  <img src="https://img.shields.io/badge/TradingView-1a1b27?style=flat-square&logo=tradingview&logoColor=2962FF" alt="TradingView"/>
  <img src="https://img.shields.io/badge/Highcharts-1a1b27?style=flat-square&logo=highcharts&logoColor=8087E8" alt="Highcharts"/>
  <img src="https://img.shields.io/badge/Plotly-1a1b27?style=flat-square&logo=plotly&logoColor=3F4F75" alt="Plotly"/>
  <img src="https://img.shields.io/badge/WebSockets-1a1b27?style=flat-square&logo=socketdotio&logoColor=ffffff" alt="WebSockets"/>
  <img src="https://img.shields.io/badge/Puppeteer-1a1b27?style=flat-square&logo=puppeteer&logoColor=40B5A4" alt="Puppeteer"/>
  <img src="https://img.shields.io/badge/n8n-1a1b27?style=flat-square&logo=n8n&logoColor=EA4B71" alt="n8n"/>
</p>

<br/>

<!-- ══════════════════════ PROJECTS ══════════════════════ -->

## 🚀 Open Source & Side Projects

<table>
<tr>
<td width="50%" valign="top">

### 🔷 Portfolio — Micro Frontend

<a href="https://hitheshmn.prehinix.com/">
  <img src="portfolio.png" width="100%" alt="Portfolio preview"/>
</a>

Angular shell plus an independently-built React remote over Module Federation, with GSAP and Lenis driving motion and smooth scroll.

`Angular` `React` `Vite` `Module Federation` `GSAP`

<a href="https://hitheshmn.prehinix.com/"><img src="https://img.shields.io/badge/Live_Site-2C5364?style=flat-square&logo=vercel&logoColor=white"/></a>

</td>
<td width="50%" valign="top">

### 👕 Dresscode — Offline Wardrobe App

Android wardrobe manager on Angular 22 + Capacitor 8, fully on-device. Catalogue from camera, inspiration shots, tag scans or receipts; build looks; get wear-pattern insights.

`Angular 22` `Capacitor 8` `SQLite` `Vitest`

<a href="https://github.com/MnHithesh/dresscode-mobile"><img src="https://img.shields.io/badge/Source-2C5364?style=flat-square&logo=github&logoColor=white"/></a>

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🎯 JobFit AI — Resume Tailor Agent

Watches Gmail for recruiter emails, extracts the JD with Gemini, and produces a tailored ATS-optimised resume in under 60 seconds — then pushes match score and gap analysis to Discord. Prompt constraints let the model reprioritise existing content but never invent experience.

`n8n` `Gemini API` `Node.js` `Discord`

<a href="https://github.com/MnHithesh/ai-resume-tailor-agent"><img src="https://img.shields.io/badge/Source-2C5364?style=flat-square&logo=github&logoColor=white"/></a>

</td>
<td width="50%" valign="top">

### ⏰ Task Reminder — Self-Hosted

Browser notifications die when the browser closes, so delivery runs through a Discord bot — an outbound WebSocket needing no public URL, open port or TLS. Uses Node's built-in `node:sqlite`, avoiding native compilation and ABI breakage.

`Node.js 24` `node:sqlite` `discord.js`

<a href="https://github.com/MnHithesh/task-remainder"><img src="https://img.shields.io/badge/Source-2C5364?style=flat-square&logo=github&logoColor=white"/></a>

</td>
</tr>
</table>

<details>
<summary><b>💰 DuoBudget — Shared Budget Tracker for Couples</b></summary>

<br/>

Shared expense tracking, cost splitting and joint financial goals, with an OpenAI-powered assistant that analyses spending patterns and returns personalised suggestions.

`React` `Node.js` `Express` `OpenAI API`

[Frontend](https://github.com/MnHithesh/duobudget_frontend) · [Backend](https://github.com/MnHithesh/duobudget_backend)

</details>

<br/>

<!-- ══════════════════════ ACTIVITY ══════════════════════ -->

## 📊 Activity

<p align="center">
  <img width="60%" src="https://streak-stats.demolab.com?user=MnHithesh&theme=tokyonight&hide_border=true&background=0D1117&ring=64B5F6&fire=64B5F6&currStreakLabel=64B5F6" alt="streak"/>
</p>

<p align="center">
  <img width="95%" src="https://github-readme-activity-graph.vercel.app/graph?username=MnHithesh&theme=tokyo-night&bg_color=0D1117&color=64B5F6&line=64B5F6&point=ffffff&hide_border=true&area=true" alt="activity graph"/>
</p>

<br/>

<!-- ══════════════════════ FOOTER ══════════════════════ -->

<p align="center">
  <i>Open to conversations about frontend architecture, real-time systems and micro frontends.</i>
</p>

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:2C5364,50:203A43,100:0F2027&height=140&section=footer&text=hitheshmn.prehinix.com&fontColor=ffffff&fontSize=20&fontAlignY=72" alt="footer"/>

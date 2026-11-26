# Yong Zhang - Resume

## Profile

| Item | Details |
| --- | --- |
| Target role | Staff Engineer / Frontend Architect |
| Experience | 18 years in web development, 13 of them at Trend Micro |
| Email | zhangyong0604@126.com |
| Location | Xuanwu District, Nanjing, China |
| Education | B.S., Information Management and Information Systems, Nanjing University of Science and Technology |
| LinkedIn | [linkedin.com/in/yong-zhang-842332bb](https://www.linkedin.com/in/yong-zhang-842332bb/) |
| GitHub | [github.com/yurizhang](https://github.com/yurizhang) |

## Strengths

- **AI agent engineering**: Claude Code is my main way of building software. Through MCP, CLIs and APIs I connect it to Figma, Jira and GitHub, so an agent covers the requirement, design, code, tests, pull request and build. I also gave the team shared hooks, skills and a project knowledge base. As of November 2026, my median ticket delivery time was about 47% shorter than in the same period of 2025 (32 → 17 days).
- **Micro-frontend architecture**: In 2021 I built the micro-frontend widget container for the Vision One security dashboard (Security Posture) from scratch. It's based on qiankun, with style isolation, a JS sandbox and remote loading, so product teams can build and deploy their widgets independently.
- **Front-end lead for a large security console**: Since 2019 I've worked on V1 Portal, the unified console of Trend Vision One (formerly Trend Micro XDR). I've merged 1,000+ pull requests across the portal and 7 platform apps.
- **Front-end architecture and performance**: I led the migration from vue-cli (webpack) to Vite, cut the first-screen i18n bundle by 30%, and made CI build output fully reproducible.
- **Mobile products and web security**: I have 5+ years of mobile product development and management, covering MDM, VMI mobile virtualization, mobile security and mobile app reputation. I also have hands-on React Native and WEEX experience, plus web security testing such as XSS.
- **Personal / partner projects**: I built education-company websites and WeChat Official Account apps on my own (PHP / MySQL). They cover e-commerce, online payment (Alipay / WeChat Pay), membership, a community forum and admin back offices.
- **Full stack and collaboration**: I can handle the Node.js / Express backend, database migrations and test suites on my own. I led the front-end team at Tuniu and am used to working across regions and teams.

## Work Experience

### Mar 2019 – Present · Trend Micro (China) · Staff Engineer

I build and maintain the front end of the Trend Vision One unified console (V1 Portal) and its platform apps, used by enterprises and service providers (xSP) worldwide.

- I drive AI-assisted development in the team. Claude Code is my main tool for delivering features, and I committed shared hooks, skills and coding guidelines for the team. I also brought a console module into the company's internal AI prototyping sandbox.
- I built the micro-frontend widget container for the Security Posture dashboard (qiankun) from scratch and still maintain it, with 92 merged pull requests.
- I've worked on the console since its Trend Micro XDR days, as it grew into Vision One, with 1,000+ merged pull requests.
- I led the front-end build upgrades: vue-cli (webpack) → Vite, on-demand locale bundles, idle-time loading of third-party scripts, and reproducible CI builds.
- I built components based on the Tonic One design system, with dark and light themes.
- I maintain the Notifications, API Keys, Product Instance, Security Posture, User Roles (RBAC) and Automation Center apps.

### Apr 2017 – Mar 2019 · Tuniu · Frontend Architect / R&D Manager (front-end team)

- Owned the front-end architecture for back-office systems and mobile sites. Led framework and standard component development, and set front-end coding standards.
- Set up an integrated dev environment (scaffolding, automated tests, deployment) and drove adoption of the front-end architecture across business lines.
- Built a front-end performance and quality monitoring platform, and used its data to keep improving site performance.

### Oct 2011 – Apr 2017 · Trend Micro (China) · Web Frontend Engineer (CoreTech)

- Full-stack development for TMMS (MDM), VMI (mobile virtualization), mobile app reputation, TDA and DLP. Front-end lead for TMMS / VMI, and took part in product planning and management.
- Chose the front-end stack and architecture (webpack + React + ES6). On the backend I used PHP, PostgreSQL, Python Django and Node.js, and wrote RESTful API design docs.
- Data visualization for large reports, browser caching and performance tuning.

### 2008 – 2011 · Early career

- Full-stack development (PHP / MySQL / jQuery) for China Mobile's 10086 Wireless City portal, an online homework platform and corporate portal sites.

## Projects

### AI agent engineering · 2026

Claude Code is my main way of building software. I use AI agents across the whole delivery flow and have packaged that into agent tooling the team can reuse.

- **End-to-end agent delivery**: The agent reads the Jira ticket and the Figma design (Figma MCP), then writes the code, runs Vitest, opens the PR with gh, updates Jira through its REST API and triggers the test-environment build. I make the design decisions and review the code.
- **Team agent tooling**: For V1 Portal I wrote Claude Code hooks (3 automatic checks: theme compatibility, CSS organization and i18n compliance), project skills (a project playbook and a theme validator) and CLAUDE.md guidelines, all committed to the repo. Teammates can use them right away, and nothing changes for anyone who doesn't use AI.
- **Context engineering**: I turned project conventions, branch topology and known pitfalls into long-term memory and a knowledge base for the agent. It keeps project context across sessions, which means less re-explaining and less rework.
- **AI prototyping platform**: I brought the console settings module into the company's internal AI prototyping sandbox, the first Vue app there. I generated UI flow docs and XState statecharts that AI prototyping tools read, so they understand page flows and state transitions.
- **AI-assisted large refactor**: With Claude and Figma MCP I split a 2,849-line component into 20 sub-components. The main file shrank by 19% with no change in behavior.
- **AI-built dev tools and quality checks**: A read-only test-environment database viewer, a database-to-UI CRUD guide and wiki for the backend, and 21 unit test suites (140+ cases). After merges, the agent runs a merge-tree check and dual-state acceptance tests. This once caught a build failure caused by a merge that silently dropped 2 files.

### Security Posture dashboard: micro-frontend widget container · 2021 – Present

The security dashboard of the Vision One platform. In 2021 I built its front-end container framework and common widgets from scratch, and I've merged 92 pull requests (about 500 commits) since.

Tech stack: React 17, qiankun 2 (built on single-spa), react-grid-layout, Highcharts, Node.js BFF

- **Micro-frontend container**: I designed the widget container on qiankun. Widgets load remotely through HTML Entry, with style isolation, a JS sandbox and idle-time prefetching. Widgets can use any framework (React, Vue and others). Product teams build, deploy and update them independently, without touching the container.
- **Dashboard interaction**: Built on react-grid-layout. Users can add, remove, rename and drag widgets and arrange them in multiple tabs. There is also a mobile widget view.
- **Common widgets**: Table, pie, line and bar chart widgets plus a data API that product teams can reuse directly.
- **Permissions and data**: What a widget shows depends on the user's role and permissions. A BFF layer aggregates data from endpoint, email and other sources.
- **Reports and export**: Dashboard export, widget reports and report preview, with localization (l10n).

### Trend Vision One unified console (V1 Portal) · 2019 – Present

Tech stack: Vue 3, Ant Design Vue, Vite, ECharts, Node.js / Express, Vitest

- Console shell and navigation: menus, the platform directory, favorites and recent visits, and app routing. I keep onboarding new apps such as Data Posture, Attack Path Analysis and Sensitive Data Classification.
- Built and packaged components based on the Tonic One design system (buttons, alert banners, inputs, menus and more), with dark and light themes.
- Endpoint / Host detail profile: supports data sources such as EPP, EDR, Edge Relay, Identity Sensor and OpenStack VMs. I added 15+ fields in 2026 alone.
- Attack simulation: the front end for simulation scenarios such as container attacks and threat actor attacks.
- Multi-site and multi-tenant: xSP service provider views, and one build shared across multiple sites.

### Front-end performance and build engineering · 2023 – 2026

- Migrated the build from vue-cli (webpack) to Vite.
- First-screen optimization: on-demand locale bundles cut the first-screen bundle from 90.5 KB to 63.8 KB (gzip, −30%). Non-critical third-party scripts now load when the browser is idle.
- Reproducible CI builds: two builds of the same source produce 162 identical output files, so cache invalidation after each release stays contained.
- Using the API Keys app as the reference, I wrote the V1 best practice for splitting static assets out to S3 with long-term caching, which other app teams follow.

### User Roles (RBAC) and platform apps · 2021 – 2026

- User Roles: main front-end developer of the core screens (role editing, permission tree, per-product permission scope), with 250+ commits.
- Notifications, Product Instance and API Keys: alerts, webhooks, credit reminders, customizable table columns and more.

### Tuniu Finance / Tuniu back-office systems · 2017 – 2019

- Built the iShow UI component library and the iShow Admin scaffold. Led the front ends of 20+ systems, including the Tuniu Finance mobile site, the loan management back office, custom trip planning and complaint management. Used React Native / WEEX on mobile, and built up finance and accounting domain knowledge.

### TMMS / VMI mobile security products · 2012 – 2017

- Front-end lead for TMMS (mobile device security management) and VMI (Virtual Mobile Infrastructure), responsible for technology choices and performance. Took part in planning and managing new mobile security and mobile app reputation products.

## Personal / Partner Projects

### Talent France (talentfr.com) · French language training and study-abroad platform · 2018 – 2019

I built the whole site, front end and back end, plus the admin back office, on my own.

Tech stack: PHP (CodeIgniter), MySQL, jQuery, Alipay / WeChat Pay

- **Content and learning**: French exam news, an online question bank and level tests, university search, success stories, course video playback and teacher profiles.
- **E-commerce and payment**: a shop with cart, orders and coupons. Integrated Alipay and WeChat Pay, handling asynchronous payment notifications and payment logs.
- **Community and user center**: forum posts, replies and topics. Sign-up and login, my courses, my question bank and my orders.
- **Admin back office**: content and operations management for courses, overseas support services, ads, coupons and admin accounts.

### Deemusic · WeChat sign-up and payment system · 2015 – 2019

I built a WeChat Official Account H5 app and admin back office for a music school on my own.

Tech stack: PHP, Smarty, MySQL, WeChat Official Account (web OAuth, JS-SDK), WeChat Pay

- **WeChat H5 app**: course and instrument showcase, trial lesson booking, online sign-up, cart and checkout, shipping addresses, user center, my class schedule and teacher leave requests.
- **WeChat features**: web OAuth login, JS-SDK sharing to Moments and chats, and WeChat Pay unified orders.
- **Referral campaigns**: share-code campaigns with tracking of successful shares, and Excel export of share data in the admin back office.
- **Admin back office**: branches, courses and class scheduling, teachers (with reviews and leave), products, orders, trial lessons and sign-ups, users and statistics.

## Skills

| Area | Technologies |
| --- | --- |
| AI agents | Claude Code, MCP (Figma and others), writing agent skills and hooks, context engineering (CLAUDE.md, long-term memory, project knowledge base), agent-driven Jira / GitHub / CI automation, AI prototyping (UI flow docs, XState statecharts) |
| Front end | Vue 3 (Options / Composition API), React, Next.js, TypeScript, jQuery, Ant Design Vue, ECharts, design-system components, i18n |
| Micro-frontends | qiankun / single-spa, Module Federation, HTML Entry, style isolation and JS sandbox, independently deployed sub-apps, react-grid-layout |
| Mobile | React Native, WEEX, hybrid apps, mobile site performance tuning |
| Build and CI | Vite, webpack, Rollup code splitting and caching strategy, Docker, GitHub Actions, reproducible builds |
| Testing | Vitest, @vue/test-utils, mock servers |
| Back end | Node.js / Express / EggJS, Go, PHP (CodeIgniter, Smarty), Python Django, RESTful API design and docs |
| WeChat and payments | WeChat Official Account development (web OAuth, JS-SDK), WeChat Mini Programs, WeChat Pay, Alipay |
| Databases | MySQL, PostgreSQL, MSSQL |
| Security | Web security testing and protection (XSS and more), permission (RBAC) design |
| Collaboration | Team leadership and communication, Jira, GitHub PR workflow, LaunchDarkly feature flags, English-speaking work environment |

## Education and Open Source

- **Education**: Sep 2000 – Jul 2004, Nanjing University of Science and Technology, B.S. in Information Management and Information Systems
- **Open source**:
    - [iShow UI](https://github.com/yurizhang/ishow): a configurable UI component library for React
    - [finance-admin](https://github.com/yurizhang/micro-finance-admin-system): an admin system solution built on Vue
    - [vue_multiple_page3](https://github.com/yurizhang/vue_multiple_page3): a vue-cli3 scaffold for multi-page apps, CDN externals and bundle optimization
- **Blog**: [cnblogs.com/yuri2016](http://www.cnblogs.com/yuri2016)

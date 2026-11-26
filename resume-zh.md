# 张勇 - 简历

## 个人信息

| 项目 | 内容 |
| --- | --- |
| 求职意向 | Staff Engineer / 前端架构师 |
| 工作年限 | 18 年 Web 开发经验，其中 13 年在 Trend Micro 趋势科技 |
| 所在地 | 南京 · 玄武区 |
| 学历 | 本科 · 南京理工大学 · 信息管理与信息系统 |
| LinkedIn | [linkedin.com/in/yong-zhang-842332bb](https://www.linkedin.com/in/yong-zhang-842332bb/) |
| GitHub | [github.com/yurizhang](https://github.com/yurizhang) |

## 个人优势

- **AI Agent 工程化**：日常以 Claude Code 为主力开发方式，通过 MCP、CLI 和 API 打通 Figma、Jira、GitHub，让 Agent 覆盖需求、设计、编码、测试、提交、构建全流程；为团队沉淀 hooks、skills 和项目知识库。截至 2026 年 11 月，需求中位交付周期比 2025 年同期缩短约 47%（32 → 17 天）。
- **微前端架构**：2021 年从 0 搭建 Vision One 安全仪表盘（Security Posture）的微前端 widget 容器框架，基于 qiankun 实现样式隔离、JS 沙箱和远程加载，各产品团队的 widget 可以独立开发、独立部署。
- **大型安全产品控制台前端主力**：2019 年至今深度参与 Trend Vision One（原 Trend Micro XDR）统一控制台 V1 Portal，累计合入 1,000+ 个 PR，覆盖 Portal 及 7 个平台级应用。
- **前端架构与性能**：主导 vue-cli (webpack) → Vite 构建迁移；首屏 i18n 包体积降低 30%，CI 构建产物完全可复现。
- **移动产品与 Web 安全**：5+ 年移动产品研发与管理经验，覆盖 MDM、VMI 移动虚拟化、移动安全、移动应用信誉服务；熟悉 React Native / WEEX 跨端开发和 XSS 等 Web 安全检测。
- **个人 / 合作项目**：独立完成教育培训类企业网站和微信公众号项目（PHP / MySQL），覆盖电商、在线支付（支付宝 / 微信支付）、会员、社区和管理后台。
- **全栈与协作**：Node.js / Express 后端、数据库迁移、测试体系都能独立完成；曾带领途牛大前端团队，熟悉跨地区、跨团队协作流程。

## 工作经历

### 2019.03 – 至今 · 趋势科技（中国）有限公司 · Staff Engineer

负责 Trend Vision One 统一控制台（V1 Portal）及周边平台应用的前端开发与维护，服务全球企业客户和 xSP 服务商。

- 推动团队 AI 化开发：以 Claude Code 为主力完成需求交付，为团队提交 hooks、skills 和项目规范，并把控制台模块接入公司内部的 AI 原型沙箱平台。
- 从 0 搭建 Security Posture 安全仪表盘的微前端 widget 容器框架（qiankun），并持续维护至今，累计合入 92 个 PR。
- 从 Trend Micro XDR 时期参与控制台建设，跟随产品演进为 Vision One，累计合入 1,000+ 个 PR。
- 主导前端工程化升级：vue-cli (webpack) 迁移到 Vite、i18n 语言包按需加载、第三方脚本空闲加载、CI 确定性构建。
- 参考 Tonic One 设计系统开发组件，支持深浅色主题。
- 维护 Notifications、API Keys、Product Instance、Security Posture、User Roles (RBAC)、Automation Center 等应用。

### 2017.04 – 2019.03 · 途牛旅游网 · 前端架构师 / 研发经理（大前端团队）

- 负责中后台系统和移动端网站的前端架构，主导框架和标准组件开发，制定前端开发规范。
- 搭建集成开发环境（快速开发、自动化测试、部署发布），推动前端架构在各业务线落地。
- 建立前端性能与质量监测平台，根据监测数据持续优化网站性能。

### 2011.10 – 2017.04 · 趋势科技（中国）有限公司 · Web 前端开发工程师（CoreTech）

- 负责 TMMS（MDM 移动设备管理）、VMI（移动虚拟化）、移动应用信誉服务、TDA、DLP 等产品的前后端开发，担任 TMMS / VMI 前端负责人，参与产品规划与管理。
- 负责前端技术选型和架构（webpack + React + ES6），后端使用 PHP / PostgreSQL / Python Django / Node.js，编写 RESTful API 设计文档。
- 大数据量报表的可视化、浏览器缓存与性能优化。

### 2008 – 2011 · 早期经历

- 参与中国移动 10086 无线城市（和生活）、在线作业平台、集团门户网站的前后端开发（PHP / MySQL / jQuery）。

## 项目经验

### AI Agent 工程化实践 · 2026

以 Claude Code 为主力开发方式，把 AI Agent 用到需求交付全流程，并沉淀为团队可复用的 Agent 基础设施。

- **Agent 端到端交付**：Agent 读取 Jira 需求和 Figma 设计稿（Figma MCP），完成编码、Vitest 测试、gh 提 PR、调 Jira REST API 回写进度、触发测试环境构建；我负责方案决策和代码审核。
- **团队 Agent 基础设施**：为 V1 Portal 编写 Claude Code hooks（主题兼容、CSS 组织、i18n 合规 3 项自动检查）、项目 skills（项目 playbook、主题校验）和 CLAUDE.md 规范并提交进仓库，团队开箱即用，对不用 AI 的同事零影响。
- **上下文工程**：把项目规范、分支拓扑、已知坑点沉淀为 Agent 的长期记忆和知识库，跨会话保持项目上下文，减少重复说明和返工。
- **AI 原型平台**：把控制台设置模块接入公司内部的 AI 原型沙箱平台，成为其中第一个 Vue 子应用；生成供 AI 原型工具读取的 UI 流程文档和 XState 状态图，让 AI 能理解页面流程和状态转换。
- **AI 辅助大型重构**：用 Claude + Figma MCP 把 2,849 行的单体组件拆成 20 个子组件，主文件减少 19%，行为零变化。
- **AI 构建研发工具与质量把关**：测试环境数据库查看器、后端从数据库到 UI 的 CRUD 开发指南与 Wiki、21 个单元测试套件（140+ 用例）；合并后由 Agent 做 merge-tree 校验和双态验收，发现过一次合并静默丢失 2 个文件导致的构建故障。

### Security Posture 安全仪表盘：微前端 Widget 容器框架 · 2021 – 至今

Vision One 平台的安全仪表盘。2021 年从 0 搭建前端容器框架和通用 widget，至今累计合入 92 个 PR、约 500 次提交。

技术栈：React 17、qiankun 2（基于 single-spa）、react-grid-layout、Highcharts、Node.js BFF

- **微前端容器**：基于 qiankun 设计 widget 容器，用 HTML Entry 方式远程加载 widget，实现样式隔离、JS 沙箱和浏览器空闲时预加载；widget 与技术栈无关（React / Vue 等均可），各产品团队独立开发、独立部署和更新，不用改动容器。
- **仪表盘交互**：基于 react-grid-layout 实现 widget 的添加、删除、重命名、拖拽排序和多 Tab 布局，并提供移动端 widget 视图。
- **通用 Widget**：提供表格、饼图、折线图、柱状图等通用 widget 和数据 API，各产品团队可直接复用。
- **权限与数据**：按用户角色和权限控制 widget 展示内容，配合 BFF 层聚合 Endpoint、Email 等多源数据。
- **报表与导出**：实现仪表盘导出、widget 报表和报表预览，支持多语言（l10n）。

### Trend Vision One 统一控制台（V1 Portal）· 2019 – 至今

技术栈：Vue 3、Ant Design Vue、Vite、ECharts、Node.js / Express、Vitest

- 控制台外壳与导航：菜单、平台目录、收藏与最近访问、应用路由接入，持续接入 Data Posture、Attack Path Analysis、Sensitive Data Classification 等新应用。
- 参考 Tonic One 设计系统开发和封装组件（按钮、告警条、输入框、菜单等），支持深浅色主题。
- Endpoint / Host Detail Profile：支持 EPP、EDR、Edge Relay、Identity Sensor、OpenStack 虚拟机等数据源，仅 2026 年就新增 15+ 个字段。
- 安全攻击模拟（Simulation）：实现容器攻击、威胁组织攻击等模拟场景的前端。
- 多站点与多租户：支持 xSP 服务商视图，多个站点共用一套构建。

### 前端性能与工程化 · 2023 – 2026

- 构建从 vue-cli (webpack) 迁移到 Vite。
- 首屏优化：i18n 语言包按需加载，首屏包 90.5 KB → 63.8 KB（gzip，−30%）；非关键第三方脚本改为浏览器空闲时加载。
- CI 确定性构建：同一份源码两次构建的 162 个产物文件完全一致，发版后缓存失效范围可控。
- 以 API Keys 应用为样板，制定 V1 静态资源拆分上 S3 并长期缓存的最佳实践，供各应用团队参照。

### User Roles (RBAC) 与平台应用 · 2021 – 2026

- User Roles：角色编辑、权限树、各产品权限范围选择等核心界面的主要前端开发者，累计 250+ 次提交。
- Notifications、Product Instance、API Keys：通知告警、Webhook、Credit 提醒、表格自定义列等功能。

### 途牛金融 / 途牛中后台 · 2017 – 2019

- 开发 iShow UI 组件库和 iShow Admin 脚手架，主导途牛金融 M 站、小贷管理后台、行程定制、投诉管理等 20 多个系统的前端；移动端使用 React Native / WEEX，并积累了金融与财务业务知识。

### TMMS / VMI 移动安全产品 · 2012 – 2017

- TMMS（移动设备安全管理）与 VMI（虚拟移动基础架构）的前端整站负责人，负责技术选型与性能优化；参与移动安全、移动应用信誉服务等产品的创新规划与管理。

## 个人 / 合作项目

### 大脸法语（talentfr.com）· 法语培训与留学服务平台 · 2018 – 2019

独立开发整站前后端和管理后台。

技术栈：PHP（CodeIgniter）、MySQL、jQuery、支付宝 / 微信支付

- **内容与学习**：法语考试资讯、在线题库与水平测评、留学院校查询、成功案例、课程视频播放、教师介绍。
- **电商与支付**：严选商城、购物车、订单、优惠券；对接支付宝和微信支付，处理支付异步通知并记录支付日志。
- **社区与用户中心**：论坛发帖、回复和话题；注册登录、我的课程、我的题库、我的订单。
- **管理后台**：课程、境外陪伴服务、广告、优惠券、管理员等内容与运营管理。

### 蒂双语音乐 · 微信公众号报名与缴费系统 · 2015 – 2019

为音乐培训机构独立开发微信公众号 H5 应用和管理后台。

技术栈：PHP、Smarty、MySQL、微信公众号（网页授权、JS-SDK）、微信支付

- **公众号 H5**：课程与乐器展示、试听预约、在线报名、购物车与下单、收货地址、用户中心、我的课程安排、老师请假。
- **微信能力**：网页授权登录、JS-SDK 分享到朋友圈和好友、微信支付统一下单。
- **分享裂变**：分享码活动和分享成功回流，后台可导出分享数据（Excel）。
- **管理后台**：分校、课程与排课、教师（含点评与请假）、商品、订单、试听与报名、用户和数据统计。

## 技能清单

| 方向 | 技术 |
| --- | --- |
| AI Agent | Claude Code、MCP（Figma 等）、Agent Skills 与 Hooks 编写、上下文工程（CLAUDE.md、长期记忆、项目知识库）、Agent 驱动的 Jira / GitHub / CI 自动化、AI 原型（UI 流程文档、XState 状态图） |
| 前端 | Vue 3（Options / Composition API）、React、TypeScript、jQuery、Ant Design Vue、ECharts、设计系统组件、i18n |
| 微前端 | qiankun / single-spa、HTML Entry、样式隔离与 JS 沙箱、子应用独立部署、react-grid-layout |
| 移动端 | React Native、WEEX、Hybrid App、移动 M 站性能优化 |
| 工程化 | Vite、webpack、Rollup 分包与缓存策略、Docker、GitHub Actions、确定性构建 |
| 测试 | Vitest、@vue/test-utils、Mock 服务 |
| 后端 | Node.js / Express / EggJS、PHP（CodeIgniter、Smarty）、Python Django、RESTful API 设计与文档 |
| 微信与支付 | 微信公众号开发（网页授权、JS-SDK）、微信小程序、微信支付、支付宝支付 |
| 数据库 | MySQL、PostgreSQL、MSSQL |
| 安全 | XSS 等 Web 安全检测与防护、权限（RBAC）设计 |
| 协作 | 团队管理与沟通、Jira、GitHub PR 流程、LaunchDarkly 灰度发布、英文工作环境 |

## 教育与开源

- **教育**：2000.09 – 2004.07 南京理工大学 · 信息管理与信息系统 · 本科
- **开源**：
    - [iShow UI](https://github.com/yurizhang/ishow)：基于 React 的可配置 UI 组件库
    - [finance-admin](https://github.com/yurizhang/micro-finance-admin-system)：基于 Vue 的后台管理系统方案
    - [vue_multiple_page3](https://github.com/yurizhang/vue_multiple_page3)：基于 vue-cli3 的多页面、CDN 外链与打包优化脚手架
- **博客**：[cnblogs.com/yuri2016](http://www.cnblogs.com/yuri2016)

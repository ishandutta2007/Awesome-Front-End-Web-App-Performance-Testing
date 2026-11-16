# Awesome-Front-End-Web-App-Performance-Testing

# Top Front-End Web & App Performance Testing Ecosystem

**Curated List of SaaS Platforms & Open-Source GitHub Projects**  
*Focused on Core Web Vitals, Synthetic Monitoring & Self-Hosted Performance Auditing*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Front-End Web & App Performance Testing**. These tools help teams measure page speed, track Core Web Vitals, and catch performance regressions—covering everything from Google's free auditing engine to commercial monitoring platforms with real-user data and CI-integrated budgets.

**Examples** include Google Lighthouse, WebPageTest, k6, SpeedCurve, Calibre, DebugBear, GTmetrix, and Pingdom (the category leaders).

**Open-source emphasis**: This section highlights every major active project for self-hosted performance auditing, open-source synthetic testing, and community-driven web vitals monitoring—ideal for teams seeking data sovereignty and avoiding per-check or per-site SaaS pricing. The open-source landscape is anchored by **Lighthouse**, Google's free auditing engine that runs anywhere Chrome runs [citation:1][citation:10], and **WebPageTest**, the battle-tested testing platform available under a permissive Apache 2.0 branch [citation:2][citation:11].

Contributions welcome! Open an PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

| Product | Description | Pricing (Starting) | Free Tier / Trial Limits |
|---------|-------------|-------------------|--------------------------|
| **[SpeedCurve](https://www.speedcurve.com/)** | Performance monitoring with synthetic tests, real-user monitoring (RUM), and Core Web Vitals tracking. Positioned for teams wanting continuous performance budgets. | Starter: **$20/month** (billing unit not specified) [citation:6] | No permanent free plan; free trial available [citation:6] |
| **[Calibre](https://calibreapp.com/)** | Web performance monitoring unifying RUM, Google CrUX data, and synthetic tests. Tracks Core Web Vitals and performance budgets. | Starter: **$50–$75/month**; Team: **$150/month**; Company: **$1,500/month** [citation:4][citation:13] | **15-day free trial** (no credit card); no permanent free tier [citation:4] |
| **[DebugBear](https://www.debugbear.com/)** | Lighthouse-based performance monitoring with synthetic tests across devices and locations. | **$125/month** (paid plans) [citation:5] | No free account; **14-day free trial**; limited guest spot checks available [citation:14] |
| **[GTmetrix](https://gtmetrix.com/)** | Website speed testing and performance monitoring. Free spot checks available; paid plans for monitoring. | Free spot checks available; paid plans via GTmetrix [citation:7] | **Free**: basic speed test (no credit card required) [citation:7] |
| **[Pingdom](https://www.pingdom.com/)** | Uptime and page speed monitoring. | **$15/month** (Uptime or Page Speed monitoring) [citation:9] | No free plan; free spot checks from 7 locations; **30-day free trial** [citation:9] |
| **[BlazeMeter](https://www.blazemeter.com/)** | Load testing and API monitoring platform (Broadcom). | Quote-only for full platform; API Monitoring free plan available | **14-day trial** with 100,000 requests; **Free plan**: 25,000 requests/month, 1 team member [citation:8] |

## Open-Source GitHub Projects

| Project | Star Badge | Description |
|---------|------------|-------------|
| **[Lighthouse](https://github.com/GoogleChrome/lighthouse)** | [![Stars](https://img.shields.io/github/stars/GoogleChrome/lighthouse?style=social&color=white)](https://github.com/GoogleChrome/lighthouse/stargazers) | **The most widely used open-source performance auditing tool.** **Apache-2.0**, maintained by Google. Runs in **Chrome DevTools, CLI, Node module, or web UI (PageSpeed Insights)**—audit any page, public or authenticated [citation:1][citation:10]. **Performance, accessibility, SEO, and best-practices audits** with actionable references explaining why each matters and how to fix it [citation:1]. **Lighthouse CI** prevents regressions by running audits in CI pipelines [citation:10]. **Best for teams wanting Google's canonical performance scoring** without a commercial subscription. |
| **[WebPageTest](https://github.com/WPO-Foundation/webpagetest)** | [![Stars](https://img.shields.io/github/stars/WPO-Foundation/webpagetest?style=social&color=white)](https://github.com/WPO-Foundation/webpagetest/stargazers) | **The most configurable open-source performance testing platform.** **Apache 2.0 branch available** (master branch uses Polyform Shield 1.0.0) [citation:2][citation:11]. **Self-host your own instance** with full control over test locations, browsers, and network conditions [citation:2]. **REST API** with `/bulktest` (PHP) and `/batchtool` (Python) for bulk test submission and analysis [citation:2][citation:11]. **Cross-platform browser agent** supports real devices and browsers. **Best for teams needing deep waterfall analysis and private test infrastructure** without per-test fees. |
| **[k6](https://github.com/grafana/k6)** | [![Stars](https://img.shields.io/github/stars/grafana/k6?style=social&color=white)](https://github.com/grafana/k6/stargazers) | **Open-source load testing with browser performance capabilities.** **AGPL-3.0**. **k6 browser module** runs Chromium-based browser tests alongside protocol-level load tests. **Playwright-to-k6 conversion path** available (not zero-cost—selectors and fixtures often need hand work) [citation:3]. **Grafana Cloud free tier**: 10,000 browser executions + 100,000 API executions per month [citation:3]. **Best for teams wanting load testing and browser performance in one tool** with a generous managed free tier. |

### Additional Strong Open-Source Options

| Project | Star Badge | Description |
|---------|------------|-------------|
| **[Lighthouse CI](https://github.com/GoogleChrome/lighthouse-ci)** | — | **CI integration for Lighthouse.** Runs audits on every commit/PR, asserts performance budgets, and surfaces regressions before deploy. **Best for teams wanting Lighthouse scores as a quality gate** in GitHub Actions or other CI [citation:10]. |

**Frameworks for building custom systems**: Choose **Lighthouse** for canonical performance scoring with zero cost and broad CI integration [citation:1][citation:10], and **WebPageTest** for deep waterfall analysis on self-hosted infrastructure with full test configuration control [citation:2][citation:11]. **k6** fills the gap for teams wanting load testing and browser performance in one tool with a generous managed free tier [citation:3].

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Performance testing tools execute requests against potentially production URLs; rate-limit synthetic tests and avoid overloading origin servers during audits.
- **Free tiers and pricing vary significantly in this category.** **Calibre offers only a 15-day trial** with no permanent free tier—pricing jumps from **$150/month (Team) to $1,500/month (Company)** with no middle ground [citation:4]. **DebugBear starts at $125/month** with only a 14-day trial and limited guest spot checks [citation:5][citation:14]. **SpeedCurve starts at $20/month** but has no free plan [citation:6]. **GTmetrix offers free spot checks** without an account [citation:7], and **Pingdom provides free spot checks from 7 locations** with a 30-day trial before the $15/month plan [citation:9]. **BlazeMeter's free plan is drastically limited** compared to its trial—25,000 requests vs. 100,000, and only 1 team member vs. 6 [citation:8]. **Open-source Lighthouse and WebPageTest eliminate per-test fees entirely**—the trade-off is operational effort for self-hosting WebPageTest [citation:2][citation:11]. **Validate whether you need managed monitoring (Calibre, DebugBear, SpeedCurve) or self-hosted auditing (Lighthouse, WebPageTest)** before committing.

---

**Made for performance engineers, front-end developers, and teams building web performance infrastructure.**  
Let's make front-end performance testing more open, measurable, and cost-predictable.

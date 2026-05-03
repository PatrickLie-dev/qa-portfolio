# 🧪 QA Portfolio

> Manual QA testing portfolio showcasing test planning, test case design, bug reporting, and exploratory testing across web and mobile applications.

---

## 🛠️ Skills & Tools

| Category | Tools / Skills |
|---|---|
| **Test Management** | Google Sheets, Jira (personal project) |
| **Bug Reporting** | Structured bug reports with severity, priority, reproduction steps |
| **Test Techniques** | Equivalence partitioning, boundary value analysis, exploratory testing |
| **Test Types** | Functional, negative, edge case, regression |
| **Browsers** | Chrome, Microsoft Edge |
| **Platforms** | Web (desktop), Mobile (Android/iOS) |

---

## 📁 Projects

### 01 — SauceDemo Login Page Testing
**App:** [saucedemo.com](https://www.saucedemo.com)
**Type:** Web application — E-commerce demo
**Focus:** Login functionality — functional, negative, and edge case testing

| Item | Details |
|---|---|
| Total test cases | 8 |
| Pass | 7 |
| Fail | 1 |
| Bugs found | 1 |

**What I tested:**
- Valid login flow (happy path)
- Invalid credentials handling
- Empty field validation
- Password field masking
- Username case sensitivity (edge case)

**Key finding — BUG-001:**
> The app performs **case-sensitive username validation** — entering `STANDARD_USER` (uppercase) with the correct password results in a login failure, despite `standard_user` being a valid registered account. Most modern applications treat usernames as case-insensitive. This creates a confusing user experience with no helpful error message.

📄 [View test cases & bug report](./01-saucedemo-login/test-cases.xlsx)

---

## 🐛 Bug Reports Summary

| Bug ID | Title | App | Severity | Status |
|---|---|---|---|---|
| BUG-001 | Login fails when username is entered in uppercase | SauceDemo | Medium | Open |

---

## 📈 Progress

This portfolio is actively being built as part of a structured 3-month QA learning roadmap.

- [x] ~~Set up portfolio repository~~
- [x] ~~Project 1: Login page test cases (SauceDemo)~~
- [ ] Project 2: End-to-end e-commerce flow (SauceDemo)
- [ ] Project 3: Mobile app testing
- [ ] ISTQB Foundation preparation

---

## 📬 Contact

- **LinkedIn:** [https://linkedin.com/in/patrick-lie-315964302/]
- **Email:** [patricklie995@gmail.com]

---

*Last updated: May 2026*

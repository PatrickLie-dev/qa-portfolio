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

### 02 — SauceDemo Products & Cart Flow Testing
**App:** [saucedemo.com](https://www.saucedemo.com)  
**Type:** Web application — E-commerce demo  
**Focus:** Product listing, sorting, cart management, and full checkout flow

| Item | Details |
|---|---|
| Total test cases | 13 |
| Pass | 13 |
| Fail | 0 |
| Bugs found | 0 |

**What I tested:**
- Product sort functionality (A-Z, Z-A, Price low-high, Price high-low)
- Add single and multiple products to cart
- Remove products from both product listing and cart pages
- Cart contents accuracy (names, prices, quantities)
- Full end-to-end checkout flow (step 1 form, order overview, order confirmation)
- Checkout form validation (empty fields)
- Price calculation verification (item total + tax = order total)

**Notable observations:**
> Checkout form validates fields sequentially (First Name first), consistent with login page behavior. Price calculations were verified manually — all totals correct. Cart badge updates in real time without page reload across all add/remove actions.

📄 [View test cases](./02-saucedemo-products-cart/test-cases.xlsx)

---

### 03 — My Demo App Mobile Testing (Android)
**App:** [My Demo App v2.2.0](https://github.com/saucelabs/my-demo-app-android/releases) by Sauce Labs  
**Type:** Mobile application — Android (Emulator: Medium Phone API 36.0)  
**Focus:** Product catalog, sorting, product detail, and cart functionality

| Item | Details |
|---|---|
| Total test cases | 13 |
| Pass | 13 |
| Fail | 0 |
| Bugs found | 1 |

**What I tested:**
- App launch and initial screen behavior
- Product catalog display (24 products — images, names, prices, ratings)
- Scroll stability across full catalog
- Product detail navigation and back navigation (scroll position preserved)
- Sort functionality (Name A-Z, Name Z-A, Price low-high, Price high-low)
- Product detail screen elements (name, image, price, rating, color selector, quantity selector, Add to Cart, Product Highlights)
- Add to cart with quantity 1 and quantity 3
- Cart icon badge update on add/remove
- Empty cart state display

**Key finding — BUG-002:**
> The app **crashes when tapping any product after "Sauce Labs Backpack (yellow)"** in the default Name - Ascending catalog order. Products up to and including Sauce Labs Backpack (yellow) open correctly. The crash is consistent and reproducible across all affected products, making a significant portion of the catalog inaccessible.

📄 [View test cases & bug report](./QA_Portfolio_Login_TestCases.xlsx)

---

## 🐛 Bug Reports Summary

| Bug ID | Title | App | Severity | Status |
|---|---|---|---|---|
| BUG-001 | Login fails when username is entered in uppercase | SauceDemo Login | Medium | Open |
| BUG-002 | App crashes when tapping products after Sauce Labs Backpack (yellow) | My Demo App v2.2.0 | Critical | Open |

---

## 📊 Overall Stats

| Metric | Count |
|---|---|
| Total test cases executed | 34 |
| Total passed | 33 |
| Total failed | 1 |
| Total bugs documented | 2 |
| Features tested | 3 |

---

## 📈 Progress
This portfolio is actively being built as part of a structured 3-month QA learning roadmap.

- [x] ~~Set up portfolio repository~~
- [x] ~~Project 1: Login page test cases (SauceDemo)~~
- [x] ~~Project 2: Products & cart flow testing (SauceDemo)~~
- [x] ~~Project 3: Mobile app testing (My Demo App Android)~~
- [ ] ISTQB Foundation preparation

---

## 📬 Contact
- **LinkedIn:** [https://linkedin.com/in/patrick-lie-315964302/]
- **Email:** [patricklie995@gmail.com](mailto:patricklie995@gmail.com)

---

*Last updated: May 2026*

# Agent E2E QA Workflow - Playwright

An AI-powered end-to-end testing automation framework that leverages Playwright and AI agents to automatically generate test plans, scripts, and reports from user stories. This project demonstrates a complete agentic QA pipeline for e-commerce checkout processes.

## 🎯 Project Overview

This project showcases an intelligent QA workflow that automates the entire testing lifecycle—from requirement analysis to test execution and reporting. It focuses on comprehensive testing of the SauceDemo e-commerce application's checkout process.

### Key Features

✔ **AI-Powered Test Planning** – Automatically generate test plans from user stories  
✔ **Smart Test Generation** – Convert test plans into ready-to-run Playwright scripts  
✔ **Exploratory Testing** – Perform interactive testing using Playwright MCP  
✔ **Automated Healing** – Self-healing tests that adapt to UI changes  
✔ **Comprehensive Reports** – AI-generated test execution reports  
✔ **GitHub Integration** – Automatic artifact commits and version control  

## 🧠 AI Agents in This Workflow

This agentic QA pipeline utilizes three specialized agents:

- **Test Planner Agent** – Analyzes user stories and generates comprehensive test scenarios
- **Test Generator Agent** – Converts test plans into executable Playwright automation scripts
- **Test Healer Agent** – Automatically identifies and fixes failing tests with minimal intervention

## 🧰 Tech Stack

| Component | Technology |
|-----------|-----------|
| Test Framework | Playwright |
| MCP Servers | Playwright MCP, GitHub MCP |
| AI Orchestration | AI Agents |
| Runtime | Node.js |
| Test Language | JavaScript/TypeScript |
| Reporting | Custom AI-Generated Reports |

## 📁 Project Structure

```
AgentE2EQAWorkflow-Playwright/
├── README.md                                    # Project documentation
├── user-stories/                                # Requirements and user stories
│   └── SCRUM-101-ecommerce-checkout.md          # E-commerce checkout requirements
├── specs/                                       # AI-generated test plans
│   └── saucedemo-checkout-test-plan.md          # Test plan for checkout flow
├── tests/                                       # Automated test scripts
│   └── saucedemo-checkout/
│       ├── cart-review.spec.ts                  # Cart review tests
│       ├── checkout-information-validation.spec.ts  # Information validation tests
│       ├── complete-checkout-flow.spec.ts       # Complete checkout flow
│       ├── order-completion.spec.ts             # Order completion tests
│       └── order-overview.spec.ts               # Order overview tests
└── test-results/                                # Test execution reports
    └── SCRUM-101-checkout-test-report.md        # Detailed test report
```

## 🚀 Getting Started

### Prerequisites

- Node.js (v16 or higher)
- npm or yarn package manager
- Git
- GitHub account

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/pavanoltraining/AgentE2EQAWorkflow-Playwright.git
   cd AgentE2EQAWorkflow-Playwright
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Install Playwright browsers**
   ```bash
   npx playwright install
   ```

## 📋 Usage

### Running Tests

Execute all tests:
```bash
npx playwright test
```

Run tests in a specific file:
```bash
npx playwright test tests/saucedemo-checkout/complete-checkout-flow.spec.ts
```

Run tests with UI mode:
```bash
npx playwright test --ui
```

Run tests in debug mode:
```bash
npx playwright test --debug
```

### Viewing Test Reports

After test execution, view the HTML report:
```bash
npx playwright show-report
```

## 🔄 End-to-End Workflow

The project demonstrates a complete AI-driven QA workflow:

```
User Story (SCRUM-101)
        ⬇
AI Test Plan Generation (specs/)
        ⬇
Exploratory Testing via Playwright MCP
        ⬇
Automation Script Generation (tests/)
        ⬇
Test Execution & Healing
        ⬇
AI Generated Test Report (test-results/)
        ⬇
GitHub Commit & Version Control
```

## 📊 Test Scenarios

### SauceDemo E-Commerce Checkout Tests

**Application:** https://www.saucedemo.com

**Test Credentials:**
- Username: `standard_user`
- Password: `secret_sauce`

**Test Coverage:**

1. **Cart Review** – Verify cart display, item details, and total calculation
2. **Checkout Information** – Validate form fields, mandatory field checks, and error handling
3. **Order Overview** – Confirm order summary, payment info, and totals
4. **Order Completion** – Verify success message and completion flow
5. **Error Handling** – Test validation and error scenarios

## 📝 Documentation

- [User Story: SCRUM-101](user-stories/SCRUM-101-ecommerce-checkout.md) – Complete requirements and acceptance criteria
- [Test Plan](specs/saucedemo-checkout-test-plan.md) – Detailed test scenarios and specifications
- [Test Report](test-results/SCRUM-101-checkout-test-report.md) – Latest test execution results

## 🔧 Configuration

Test configuration can be modified in `playwright.config.ts` (if present) to adjust:
- Browser types (Chromium, Firefox, WebKit)
- Test timeouts
- Retry logic
- Reporter settings
- Base URL
- Parallel execution


## 👤 Author

**Pavan** 

## 🔗 Links

- [GitHub Repository](https://github.com/pavanoltraining/AgentE2EQAWorkflow-Playwright)
- [SauceDemo Application](https://www.saucedemo.com)
- [Playwright Documentation](https://playwright.dev)

---

**Last Updated:** May 31, 2026  

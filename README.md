SauceDemo (Swag Labs) — Manual & Exploratory QA Testing

Manual and exploratory testing of the SauceDemo e-commerce web app, with a full test execution log and 30 documented defect reports.

📄 Full report: SauceDemo_QA_Report.pdf

Course project for Software Testing & Quality Assurance (CSSE 604), University of Karachi (UBIT). Solo project, tested 05–09 October 2026.

Results at a glance
Metric	Count
Test cases executed	124 (100 planned, 2 additional scripted, 21 exploratory)
Passed	87
Failed	37
Unique defects reported	30
Severity	Defects
Critical	4
High	11
Medium	9
Low	6
Scope
Login and authentication (all six demo accounts)
Product inventory, product details and sorting
Cart operations and cart badge
Checkout form validation, order overview and tax calculation
Order completion
Session handling, direct URL access and browser navigation
UI, responsive layout (375 px) and basic accessibility (WCAG 2.1)
Performance observation

Out of scope: load/stress testing and penetration testing.

Notable defects
ID	Defect	Severity
SD-BUG-001	An order can be placed with an empty cart ($0.00 order completed)	High
SD-BUG-007	Cart is not cleared on logout, so the next user inherits it (stored in localStorage)	High
SD-BUG-008	Checkout information step can be skipped by opening the overview URL directly	High
SD-BUG-016	Order overview doubles the item total (problem_user)	Critical
SD-BUG-022	Finish button does not complete the order (error_user)	Critical
SD-BUG-025	Inventory shows random prices that change on refresh (visual_user)	Critical

The report contains all 30 defects, each with steps to reproduce, expected and actual results, a test oracle, reproducibility and screenshot evidence.

Testing techniques

Boundary value analysis · Equivalence partitioning · Decision table testing · State transition testing · Exploratory testing · Error guessing · Comparison testing · Session/security testing · Accessibility testing · Console/log analysis · Regression testing

Environment and tools
Windows 10 (64-bit), Google Chrome 155
Chrome DevTools: Elements, Console, Application (cookies, localStorage), Performance, device toolbar
Microsoft Excel (test execution log), Microsoft Word (report)
Report structure
Project objective, scope and test environment
Test case execution log (124 cases)
Test execution summary and severity definitions
Defect reports (one per page, standard defect-report template from W. E. Lewis)
Appendices: features list, tools, techniques, references and limitations
Note

SauceDemo is a demo site built for testing practice, and some of its accounts contain deliberate faults. Each defect is still reported because it is reproducible and breaks an identifiable rule.

Author

Malika Fatima — BS Software Engineering, University of Karachi (UBIT) LinkedIn · GitHub

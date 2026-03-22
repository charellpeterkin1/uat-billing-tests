
# UAT Billing Test Automation Suite

This project simulates a User Acceptance Testing (UAT) suite for a billing web application. It automates verification of routing logic for different client types (`retail`, `enterprise`, `gov`) and includes a login simulation using Selenium and Python.

The goal is to demonstrate how a QA Engineer can build, structure, and run end-to-end automated tests, complete with mock login flow and routing assertions.

## Preview


![Billing App Screenshot](uat-billing-screenshot.png)
![Billing Test Results](uat-billing-screenshot-results.png)

### Testing Scope

This test suite validates:

- Login workflow
- Invoice routing logic for retail clients
- Invoice routing logic for enterprise clients
- Invoice routing logic for government clients

#### Folder Structure

- `automation/` – Python Selenium scripts for test automation  
- `mock-app/` – Lightweight Flask app that simulates a real billing app  
- `test-cases/` – Manual test documentation  
- `results/` – Logs or output files from test runs  

---

##### Tools & Technologies

- Python 3.11+  
- Selenium WebDriver  
- Flask  
- ChromeDriver  
- Git  

---

How to Run Locally

1. Clone the repo
```bash
git clone https://github.com/charellpeterkin/uat-billing-tests.git
cd uat-billing-tests
```

2. Set up and activate virtual environment
```bash
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

3. Start the mock billing app
```bash
cd mock-app
flask run
```

4. In a second terminal, run the test
```bash
cd automation
source ../venv/bin/activate
python3 test_invoice_routing.py
```

All test outcomes (e.g., login success, routing validation) will print directly to the terminal.

---

Sample Test Output

```
Login form filled successfully  
Retail invoice routing passed  
Enterprise invoice routing passed  
Gov invoice routing passed  
Test complete. Browser closed.
```

---

Author

**Charell Peterkin**  
QA Engineer | Technologist | Mom of two | Passionate about tech accessibility  
[GitHub](https://github.com/charellpeterkin) | [LinkedIn](https://www.linkedin.com/in/charellpeterkin)

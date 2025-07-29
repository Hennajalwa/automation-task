# Automation Testing Suite - Selenium + Postman

**Submitted by:** Henna Jalwa, U.K  
**Date:** 29 July 2025  
**Task:** Automated Testing for Web Application (UI + API)

## 🚀 Quick Setup (< 2 minutes)

### Prerequisites
- Java 11+ installed
- Maven 3.6+
- Chrome browser
- Postman (for API testing)

### Installation & Execution
```bash
# Clone/Navigate to project
cd automation-task

# Run Selenium UI Tests
cd selenium-tests
mvn clean test

# Run Postman API Tests
# Open Postman and import the collection from postman-tests/collections/
# Import environment from postman-tests/environments/QA.postman_environment.json
# Run the collection manually or use Postman's collection runner

# View Reports
# UI Test Reports: selenium-tests/target/surefire-reports/
# API Test Reports: docs/test-reports/api-test-execution-report.md
```

## 📁 Project Structure
```
automation-task/
├── README.md                          # This file
├── docs/
│   ├── test-plan.md                   # Test strategy document
│   └── test-reports/                  # Test execution reports
├── selenium-tests/                    # UI Automation (Java)
│   ├── src/test/java/tests/          # All-in-one test classes
│   └── pom.xml                       # Maven dependencies
├── postman-tests/                     # API Automation
│   ├── collections/                   # Postman test collections
│   └── environments/                  # Environment configurations
└── screenshots/                       # Test evidence
```

## 🎯 Test Coverage

### UI Testing (Selenium WebDriver)
- ✅ User Registration (Valid scenarios)
- ✅ User Login (Valid/Invalid credentials)  
- ✅ Profile Management (Update user info)
- ✅ User Deletion
- ✅ Form Validations
- ✅ Error Handling

### API Testing (Postman)

- ✅ POST /user/signup (Create Account - Valid)
- ✅ POST /user/signin (Login - Positive/Negative)
- ✅ GET /userInfo (Read User Details)
- ✅ PATCH /userInfo (Update User)
- ✅ DELETE /userInfo (Delete User)

## 🛠️ Tools & Frameworks

| Component | Tool | Rationale |
|-----------|------|-----------|
| UI Automation | Selenium WebDriver + Java | Cross-browser support, mature ecosystem |
| Test Framework | TestNG | Parallel execution, detailed reporting |
| API Testing | Postman | User-friendly interface, easy test creation |
| Build Tool | Maven | Dependency management, standardized builds |
| Reporting | TestNG Reports + Postman Reports | Comprehensive test results |

## 🌐 Test Environments

- **QA Environment:** https://user-login-sys.netlify.app/ (UI)
- **API Environment:** https://user-login-mern-app.onrender.com/ (Backend)

## 📊 Test Results Summary

### Latest Execution Results
- **UI Tests:** 5/5 Passed ✅ (Execution Time: ~2m 30s)
- **API Tests:** 5/5 Passed ✅ (Execution Time: ~45s)
- **Total Coverage:** 100% of defined test scenarios

## 🔧 Troubleshooting

### Common Issues
1. **Chrome Driver Issues:** Ensure Chrome browser is updated
2. **Maven Dependencies:** Run `mvn clean install` if dependencies fail
3. **API Environment:** Verify endpoints are accessible from your network
4. **Postman Collections:** Ensure environment variables are properly set

### Support
For any issues or questions, refer to:
- [Test Plan Documentation](docs/test-plan.md)
- [Detailed Test Reports](docs/test-reports/)

---
**Note:** This test suite demonstrates automated testing capabilities for both UI and API layers of a web application, using Postman for API testing and consolidated Selenium scripts for UI automation. 
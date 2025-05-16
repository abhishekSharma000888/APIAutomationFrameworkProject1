# **REST Assured API Automation Framework**

A robust **API Automation Testing Framework** built with **REST Assured**, designed for **functional, regression, and integration testing** of RESTful APIs.

## **🚀 Tech Stack**
| Category       | Tools/Libraries |  
|---------------|----------------|  
| **Core Framework** | REST Assured, Java 11+ |  
| **Build Tool** | Maven |  
| **Testing Framework** | TestNG |  
| **Reporting** | Allure Report |  
| **Logging** | Log4j2 |  
| **Static Code Analysis** | SonarLint |  
| **Version Control** | Git & GitHub |  
| **CI/CD** | Jenkins |  
| **JSON Parsing** | Jackson & Gson |  

---

## **📌 Features**
✅ **REST Assured** for API testing with BDD-style syntax  
✅ **TestNG** for test execution, parallel runs, and assertions  
✅ **Allure Report** for detailed and interactive test reports  
✅ **Log4j2** for structured logging  
✅ **Jackson & Gson** for JSON payload serialization/deserialization  
✅ **Maven** for dependency management  
✅ **Jenkins** integration for CI/CD pipeline  
✅ **SonarLint** for code quality checks

---

## **🛠 Setup & Execution**

### **Prerequisites**
- Java 11+
- Maven 3.8+
- Allure CLI (for report generation)

### **1. Clone the Repository**
```bash
git clone https://github.com/your-username/rest-assured-api-framework.git
cd rest-assured-api-framework
```

### **2. Build the Project**
```bash
mvn clean install
```

### **3. Run Tests**
#### **Run all tests**
```bash
mvn test
```  
#### **Run tests with a specific TestNG suite**
```bash
mvn test -Dsurefire.suiteXmlFiles=testng.xml
```  

### **4. Generate Allure Report**
```bash
allure serve allure-results
```  

### **5. Jenkins Integration**
- Configure a **Jenkins job** with a **Maven build step**
- Use the **Allure Plugin** to publish reports

---

## **📂 Project Structure**
```
src/
├── main/
│   ├── java/
│   │   ├── config/          # Configuration files (e.g., API endpoints, headers)
│   │   ├── models/          # POJO classes for request/response (Jackson/Gson)
│   │   ├── utils/           # Helper classes (e.g., API client, assertions)
│   │   └── payloads/        # JSON payload builders
│   └── resources/
│       ├── log4j2.xml       # Log4j2 configuration
│       └── config.properties # Environment variables
│
├── test/
│   ├── java/
│   │   ├── tests/           # Test classes (TestNG)
│   │   └── listeners/       # TestNG listeners
│   └── resources/
│       ├── testng.xml       # TestNG suite configuration
│       └── test-data/       # Test data (JSON, CSV)
```

---

## **📊 Reports & Logs**
- **Allure Report**: Detailed test execution reports (run `allure serve allure-results`)
- **Logs**: Stored in `logs/` (configured via Log4j2)

---

## **🔧 Best Practices**
✔ **Use POJOs** (with Jackson/Gson) for request/response handling  
✔ **Modularize API requests** for reusability  
✔ **Use TestNG DataProviders** for data-driven testing  
✔ **Follow API Contract Testing** (OpenAPI/Swagger validation)  
✔ **Integrate with CI/CD** (Jenkins/GitHub Actions)

---

## **📜 License**
This project is licensed under **MIT License**.

---

## **📬 Contact**
For questions or contributions, reach out to:  
📧 [your-email@example.com](mailto:your-email@example.com)  
🔗 [GitHub Profile](https://github.com/your-username)

---

**Happy Testing! 🚀**

---

Would you like any modifications (e.g., adding Docker support, more details on payload management, or CI/CD pipeline steps)? Let me know!
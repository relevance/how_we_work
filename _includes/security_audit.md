### Security Audit {#security_audit}

A security audit will typically include five phases:

* Source Code Audit: We review the project's source code and identify vulnerabilities to test in subsequent phases. Key areas include input sanitization, SQL queries and sensitive data storage.
* XSS Audit: We test all endpoints exposed by the application to verify that scripts cannot be injected into the application. This reduces the risk of Cross-Site Scripting (XSS), which can expose sensitive customer data, violate privacy, and lead to further compromises.
* SQL Injection Audit: We test all endpoints exposed by the application to verify that SQL cannot be injected into the database. An SQL injection attack can expose sensitive data and corrupt the database.
* Fuzzing Audit: We crawl and index the application for fuzzing vulnerabilities. Fuzzing is an automated attack, which bombards an entire application with bad data and verifies that the application responds appropriately.
* Deployment Stack Audit: We test the production environment, examining key elements such as the operating system, web server and applicable databases.

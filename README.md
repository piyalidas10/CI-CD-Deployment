# CI-CD-Deployment
  - YAML is a human-readable data serialization language. It is commonly used for configuration files and in applications where data is being stored or transmitted. YAML is a strict JSON superset and includes extra features such as the notion of tagging data types, support for non hierarchical data structures, the option to structure data with indentation, and multiple forms of scalar data quoting. YAML is an open format.
  - YAML is one of the most popular data serialization languages, and it is used mostly for writing configuration files.
   - With YAML, you can define your API's endpoints, parameters, and responses in a clear and concise format. Tools like Swagger and OpenAPI take advantage of YAML's simplicity to generate beautiful and interactive documentation.
   - YAML is a human-readable data serialization format that is commonly used in DevOps. YAML provides several benefits for DevOps, including ease of use, readability, and flexibility. YAML can be used in DevOps for a variety of tasks, such as defining infrastructure, describing deployments, and configuring pipelines.
   - YAML is well-suited for configuration files due to its structured and readable format. It simplifies the process of defining configurations by using indentation and key-value pairs, making it manageable and adaptable for various software applications.

## CI/CD Tools
The top CI/CD tools include popular choices like Jenkins, GitLab CI/CD, GitHub Actions, CircleCI, and Azure DevOps, which are widely used for automating software builds, testing, and deployments. Other strong contenders are TeamCity for robust build management, Bamboo for seamless Atlassian integration, Travis CI for open-source projects, Buddy for simplicity, and Spinnaker for continuous delivery. 

**Jenkins :** An open-source automation server known for its extensive plugin ecosystem and flexibility, making it suitable for various projects.   
**GitLab CI/CD :** A powerful, integrated platform that provides CI/CD capabilities directly within the GitLab platform for source code management.     
**GitHub Actions :** Allows for workflow automation and CI/CD directly within GitHub, making it easy to automate tasks from the repository.   
**CircleCI :** A cloud-based CI/CD platform renowned for its speed, reliability, and ability to automate builds across multiple environments.   
**Azure DevOps :** Microsoft's comprehensive platform for developer services, offering CI/CD pipelines and integration with other Azure services.  
**Bitbucket Pipelines :** An integrated CI/CD solution within Bitbucket for automating builds, tests, and deployments directly from your repository.   
**AWS CodePipeline :** Amazon Web Services' service for orchestrating CI/CD pipelines, integrating with various AWS services to automate releases.   
**GoCD :** An open-source tool focused on continuous delivery with an emphasis on visualizing and managing complex workflows.   
**TeamCity :** A user-friendly and powerful CI/CD solution from JetBrains, offering robust build management across various platforms.   
**Bamboo :** Atlassian's continuous delivery pipeline platform that integrates smoothly with other Atlassian products like Jira and Bitbucket.   
**Travis CI :** A cloud-based CI/CD tool popular in the open-source community, specifically designed for building and testing projects hosted on GitHub.   
**Buddy :** Known for its user-friendly interface, Buddy simplifies the creation of CI/CD pipelines and workflows.   
**Spinnaker :** A continuous delivery platform developed by Netflix that excels at automating the deployment process, especially for cloud-native applications.   

## CI/CD Security
CI/CD (Continuous Integration/Continuous Deployment) security tools are designed to integrate security checks and validations into the CI/CD pipeline, ensuring that security vulnerabilities are identified and addressed before the code is deployed to production. The primary goal is to shift security left in the development lifecycle, so potential issues are spotted as early as possible.
**Static Application Security Testing (SAST)** : 
**Dynamic Application Security Testing (DAST)** : 
**Software Composition Analysis (SCA)** :
**Interactive Application Security Testing (IAST)** : 

## CI/CD Security Tools
CI/CD (Continuous Integration/Continuous Deployment) security tools are designed to integrate security checks and validations into the CI/CD pipeline, ensuring that security vulnerabilities are identified and addressed before the code is deployed to production. The primary goal is to shift security left in the development lifecycle, so potential issues are spotted as early as possible.

  -  If you want enterprise-grade SAST + SCA with full DevSecOps integration → Checkmarx.
  -  If you prefer cloud-native SaaS with SAST+DAST → Veracode.
  -  If you want code quality + some security → SonarQube.
  -  If you focus on open-source vulnerabilities & container security → Snyk.

Veracode
-------------------------------------------------------------
The Veracode tool is a cloud-based application security platform that uses automated, on-demand scanning to identify and help remediate security flaws in software applications. It offers various testing types, including Static Application Security Testing (SAST) for code-level analysis, Dynamic Application Security Testing (DAST) for runtime testing of web applications, and Software Composition Analysis (SCA) for third-party code, all integrated into a single platform for scalability and ease of use.

  -  Veracode = full-stack AppSec platform (SAST + DAST + SCA + IAST) for DevSecOps. It’s often used by enterprises that want security integrated at every stage of the pipeline, not just static analysis.
  -  Shift-Left Security → scan code early in CI/CD pipelines.
  -  Security gates in pipelines → fail builds with critical flaws.
  -  Continuous Testing → every commit, merge, or release is tested.
  -  Feedback loops → fast remediation guidance for developers.
  -  Governance → centralized reporting for security teams.
  -  Results appear in the Veracode dashboard
  -  Veracode can scan web, mobile, and third-party applications, including legacy code and open-source components. 


Coverity
--------------------------------------------------------------
Coverity is a Static Application Security Testing (SAST) tool developed by Synopsys. It scans source code without executing it to identify:
  -  Security vulnerabilities (e.g., SQL injection, XSS, buffer overflows)
  -  Code quality issues (e.g., null pointer dereferences, resource leaks)
  -  Compliance issues (e.g., OWASP Top 10, CERT, MISRA standards)
  -  CI/CD Integration (Coverity can run automatically during builds → blocking builds with critical security flaws.)
  -  Shift-left Security (Developers get security feedback inside IDEs before committing code)
  -  Continuous Security Testing (Each commit/merge request is scanned for vulnerabilities)
  -  Risk Management (Provides metrics (defects per KLOC, remediation rate, severity distribution) to track progress)
  -  Reduces false positives (smarter analysis than many other SAST tools)
  -  Defects uploaded to Coverity Connect (dashboard)
  -  Pipeline fails if critical vulnerabilities exist

It’s widely used in DevOps and DevSecOps pipelines to shift security left — meaning, catching issues early in development instead of later in production.

Splunk
--------------------------------------------------------------
Splunk is a platform that collects and indexes machine-generated data (logs, metrics, traces) from various sources—servers, apps, containers, CI/CD tools, and cloud infrastructure. It then provides real-time monitoring, alerting, visualization, and analytics.    
Splunk is an effective tool for log management and data analytics that aids companies in collecting, analyzing, and visualizing machine-generated data in real-time. **Splunk is extensively utilized for IT ops, cybersecurity, DevOps monitoring, and business analytics.**    

  -  **Ingestion of Deployment Logs :** Splunk integrates seamlessly with various CI/CD tools and platforms,allowing teams to ingest deployment logs generated during the build, test, and deployment phases. CI/CD tools such as Jenkins, GitLab CI/CD, Travis CI, or CircleCI can be configured to send logs directly to Splunk using HTTP event collectors or Splunk forwarders.
  -  **Centralized Log Management :** Once logs are ingested into Splunk, they are centralized within a unified platform, providing a single source of truth for monitoring and analysis. Logs from different stages of the CI/CD pipeline, including build logs, test results, deployment logs, and application logs, are aggregated and indexed for easy retrieval and analysis.
  -  **Real-time Monitoring and Analysis :** Splunk enables real-time monitoring and analysis of deployment activities, allowing teams to track the progress of builds and deployments, monitor resource utilization, and detect anomalies or errors. Custom dashboards and visualizations in Splunk provide insights into key performance indicators (KPIs), trends, and patterns, facilitating proactive decision-making and troubleshooting.
  -  **Alerting & Notification :** Splunk can trigger alerts when certain criteria are met – for instance, if a specific error message appears, if the number of failed login attempts exceeds a threshold in a 5-minute window, or if a server’s CPU usage stays above 90% for too long. Alerts can be delivered through various channels (email, SMS, creating a ServiceNow ticket, executing a script, etc.). This real-time alerting capability means Splunk can function as a monitoring system for IT operations and security.
  -  **Dashboards and Visualization :** To make sense of large data sets, Splunk offers robust visualization and reporting features. Users can build interactive dashboards that display charts, graphs, tables, maps, and other visualizations reflecting the data in Splunk​. These dashboards are highly customizable – you can create panels for different metrics (e.g., a line chart of website response times, a pie chart of log severity levels, a single value showing the count of active alerts, etc.). Splunk also provides many out-of-the-box reports and the ability to generate PDF reports on a schedule. This visualization capability turns raw data into at-a-glance insights for technical and non-technical audiences alike.


Checkmarx
--------------------------------------------------------------
Checkmarx is a software security platform that focuses on Application Security Testing (AST) to help developers identify and fix vulnerabilities early in the software development lifecycle (SDLC). It’s widely used in DevSecOps pipelines because it integrates well with CI/CD tools, Git repositories, and IDEs.

  - Checkmarx offers both SAST and DAST capabilities as part of its comprehensive Checkmarx One application security platform.
  - Enterprise-grade SAST + SCA with full DevSecOps integration
  - Shift-left security: find vulnerabilities before production.
  - Automates compliance with OWASP Top 10, SANS 25, PCI DSS, etc.
  - Provides a unified dashboard for all security risks.
  - SAST (Static Application Security Testing): Analyzes source code, bytecode, or binaries without executing them. Detects issues like SQL injection, XSS, insecure data handling, etc. Supports multiple programming languages and frameworks.
  - SCA (Software Composition Analysis) : Scans open-source libraries and dependencies. Detects known vulnerabilities (CVEs), license risks, and outdated components.
  - DAST (Dynamic Application Security Testing, via partners) : Tests running applications from the outside (black-box testing). Simulates real-world attacks while the app is live.
  - IaC Security : Scans Infrastructure-as-Code (Terraform, CloudFormation, Kubernetes, etc.). Finds misconfigurations and compliance issues before deployment.
  - API Security : Tests API definitions (Swagger, OpenAPI) for vulnerabilities.
  - Integration into CI/CD : Works with Jenkins, GitHub Actions, GitLab CI, Azure DevOps, CircleCI, etc. Automates scans as part of the build pipeline.
  - Developer-Friendly Tools : Plugins for VS Code, IntelliJ, Eclipse, etc. Provides remediation guidance and secure coding practices.

Acunetix
--------------------------------------------------------------
Acunetix is a web application security testing tool that focuses on detecting vulnerabilities in websites, web apps, and APIs. It’s widely used by security teams and DevOps engineers to automate vulnerability scanning during development and in production.

  -  Acunetix is primarily a DAST (Dynamic Application Security Testing) tool, which tests applications by simulating external attacks from a "black-box" perspective, without needing access to the source code
  -  Automated Vulnerability Scanning : Detects OWASP Top 10 issues like SQL Injection, Cross-Site Scripting (XSS), CSRF, SSRF, and more.
  -  Web Application & API Security : Scans REST, SOAP, GraphQL APIs, Single-Page Applications (SPAs), and modern frameworks like React, Angular, Vue.
  -  Network Security Checks : Includes scanning for open ports, misconfigurations, and weak SSL/TLS.
  -  Continuous Integration Support : Integrates with CI/CD tools (Jenkins, GitHub Actions, GitLab CI/CD, Azure DevOps, etc.).
  -  Compliance Reporting : Generates reports for PCI DSS, HIPAA, ISO 27001, OWASP Top 10, GDPR, etc.
  -  Crawler & Scanner: Deep crawling of complex apps (including JavaScript-heavy SPAs).
  -  Interactive Application Security Testing (IAST): Works with AcuSensor to give more accurate results with fewer false positives.
  -  Risk Prioritization: Shows severity levels and remediation guidance.
  -  Team Collaboration: Supports multi-user roles and workflows for enterprises.
  -  Integration: Connects with Jira, GitHub, GitLab, Azure, Slack, and other DevOps/SecOps tools.

OWASP Zed Attack Proxy (ZAP)
--------------------------------------------------------------
A full featured free and open source DAST tool that includes both automated scanning for vulnerabilities and tools to assist expert manual web app pen testing.

  -  A man-in-the-middle proxy tool designed to find vulnerabilities in web applications.
  -  Can intercept, inspect, and modify traffic between the browser and web application.
  -  Useful for manual security testing as well as automated scanning.
  -  Designed for beginners but powerful enough for professionals.
  -  Intercepting Proxy : Allows you to view and modify requests/responses.
  -  Automated Scanning : Passive & active scanning for vulnerabilities (SQLi, XSS, CSRF, insecure headers, etc.).
  -  Spidering & Crawling : Discovers endpoints and application paths automatically.
  -  Fuzzer : Sends large volumes of custom payloads to test input validation.
  -  API Security Testing : Supports OpenAPI, SOAP, GraphQL scanning.
  -  Authentication Testing : Can handle session tokens, login pages, SSO, etc.
  -  Plug-in Marketplace : Extend functionality with community add-ons.
  -  Automation & CI/CD : Works with Jenkins, GitHub Actions, GitLab CI, etc.
  -  Scripting Support : Supports scripting in Python, JavaScript, Groovy, and others.
  -  Cross-Platform : Runs on Windows, Linux, macOS, and even as a Docker container.

OWASP (Open Worldwide Application Security Project) is a non-profit organization that works to improve the security of software through community-led projects, standards, tools, and educational resources. It’s one of the most recognized authorities in the field of application security.

  -  OWASP Top 10 → A list of the most critical security risks to web applications, updated regularly (latest version: 2021).
  -  OWASP Projects → Community-driven tools & guides like:
        -  OWASP ZAP (Zed Attack Proxy) → Free DAST tool.
        -  Cheat Sheet Series → Best practices for secure coding.
        -  OWASP Dependency-Check → Detects vulnerable libraries.
        -  OWASP ASVS (Application Security Verification Standard) → Framework for testing application security.
  - Security Training & Awareness → Conferences, meetups, and documentation.
  - Compliance & Standards Alignment → Many companies align their AppSec programs with OWASP standards.

OWASP Top 10 (2021 Categories)
  -  Broken Access Control
  -  Cryptographic Failures (previously Sensitive Data Exposure)
  -  Injection (SQLi, NoSQLi, LDAP, etc.)
  -  Insecure Design
  -  Security Misconfiguration
  -  Vulnerable & Outdated Components
  -  Identification & Authentication Failures
  -  Software & Data Integrity Failures
  -  Security Logging & Monitoring Failures
  -  Server-Side Request Forgery (SSRF)


Codecov | Code Coverage
--------------------------------------------------------------
Codecov is a code coverage reporting tool that integrates with CI/CD pipelines to help teams understand how well their codebase is tested. It focuses on providing insights into test coverage, highlighting untested parts of your code, and ensuring that changes don’t reduce coverage quality.

  -  Multi-language support: Works with most programming languages (Python, JavaScript, Java, Go, C/C++, Ruby, PHP, etc.).
  -  Coverage visualization: Generates reports with line-by-line annotations showing which lines are covered by tests.
  -  Pull request integration: Adds coverage checks and comments directly into GitHub, GitLab, or Bitbucket PRs/MRs.
  -  Coverage thresholds: You can enforce minimum coverage requirements (e.g., block merging if coverage drops below 80%).
  -  Test impact analysis: Helps spot untested code paths introduced by recent changes.
  -  CI/CD compatibility: Works with GitHub Actions, GitLab CI, CircleCI, Jenkins, Travis CI, and many more.
  -  Security & privacy: Offers both cloud and self-hosted options.



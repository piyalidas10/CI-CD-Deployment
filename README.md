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

Splunk
--------------------------------------------------------------
Splunk is a platform that collects and indexes machine-generated data (logs, metrics, traces) from various sources—servers, apps, containers, CI/CD tools, and cloud infrastructure. It then provides real-time monitoring, alerting, visualization, and analytics.    
Splunk is an effective tool for log management and data analytics that aids companies in collecting, analyzing, and visualizing machine-generated data in real-time. **Splunk is extensively utilized for IT ops, cybersecurity, DevOps monitoring, and business analytics.**    

  -  **Ingestion of Deployment Logs :** Splunk integrates seamlessly with various CI/CD tools and platforms,allowing teams to ingest deployment logs generated during the build, test, and deployment phases. CI/CD tools such as Jenkins, GitLab CI/CD, Travis CI, or CircleCI can be configured to send logs directly to Splunk using HTTP event collectors or Splunk forwarders.
  -  **Centralized Log Management :** Once logs are ingested into Splunk, they are centralized within a unified platform, providing a single source of truth for monitoring and analysis. Logs from different stages of the CI/CD pipeline, including build logs, test results, deployment logs, and application logs, are aggregated and indexed for easy retrieval and analysis.
  -  **Real-time Monitoring and Analysis :** Splunk enables real-time monitoring and analysis of deployment activities, allowing teams to track the progress of builds and deployments, monitor resource utilization, and detect anomalies or errors. Custom dashboards and visualizations in Splunk provide insights into key performance indicators (KPIs), trends, and patterns, facilitating proactive decision-making and troubleshooting.
  -  **Alerting & Notification :** Splunk can trigger alerts when certain criteria are met – for instance, if a specific error message appears, if the number of failed login attempts exceeds a threshold in a 5-minute window, or if a server’s CPU usage stays above 90% for too long. Alerts can be delivered through various channels (email, SMS, creating a ServiceNow ticket, executing a script, etc.). This real-time alerting capability means Splunk can function as a monitoring system for IT operations and security.
  -  **Dashboards and Visualization :** To make sense of large data sets, Splunk offers robust visualization and reporting features. Users can build interactive dashboards that display charts, graphs, tables, maps, and other visualizations reflecting the data in Splunk​. These dashboards are highly customizable – you can create panels for different metrics (e.g., a line chart of website response times, a pie chart of log severity levels, a single value showing the count of active alerts, etc.). Splunk also provides many out-of-the-box reports and the ability to generate PDF reports on a schedule. This visualization capability turns raw data into at-a-glance insights for technical and non-technical audiences alike.

Summary of the Work I have completed with JustIT



# Week 1 - Data Technician Workbook Summary

## Task – Data Laws and Regulations
Researched and explained key UK data protection laws including:
- **Data Protection Act**: governs secure and fair use of personal data.
- **GDPR**: EU-wide law for personal data privacy and control.
- **Freedom of Information Act**: public access to data held by authorities.
- **Computer Misuse Act**: prohibits unauthorised access or cybercrime.
Each section outlined what the law is, why it matters, real-world examples, and consequences of breaches.

## Task – Excel Practice
- Created tables, sorted data, and used SUM and AVERAGE functions.
- Analyzed dataset performance for English, Math, and Science.
- Practiced using Excel formulas and sorting/filtering tools.

## Task – Pivot Tables & SWITCH Function
- Created Pivot Tables using sales data by region and product.
- Applied the `SWITCH` function to classify sales volumes (High, Medium, Low).
- Analyzed bike sales by demographics and region, identifying profitability patterns.

## Task – Presentation Preparation
- Researched how to prepare and deliver data findings to senior leaders.
- Discussed presentation tools, public speaking, and visualization best practices.
- Evaluated tools for data visualisation and delivery effectiveness.
<img width="537" height="75" alt="Excel Screenshot" src="https://github.com/user-attachments/assets/5b6e3c17-856a-464a-b8e4-9a8596f4d446" />

---
**Overall Focus:** Developing understanding of data protection laws, Excel data analysis, pivot tables, and professional presentation skills.

#Workbook Week 2 Summary

## Task – Tableau Introduction
- Compared Tableau versions: Desktop, Public, Server, Cloud, and supporting tools.
- Explained Tableau Public limitations: all data is public, limited connectors, no live updates.

## Task – Data Analysis Projects
- **Spotify Dataset**: Discovered songs with higher “danceability” and pop genre were most popular.
- **Health Dataset**: Analyzed healthcare trends and reflected on data use within the NHS for decision-making.

## Task – Power BI Labs
- **Lab 1:** Imported data into Power BI Desktop.
- **Lab 2:** Transformed and loaded cleaned data.
  
## Task – Power BI Reports and Dashboards
- **Lab 6:** Designed professional Power BI report layouts.
- **Lab 9:** Created interactive dashboards.
<img width="464" height="553" alt="Tableau Screenshot" src="https://github.com/user-attachments/assets/b51f15de-ab84-486e-bd83-ca07ff175fc8" />

---
**Overall Focus:** Building visualisation and data storytelling skills using Tableau and Power BI.

# Database Concepts Workbook Summary Week 3

## Task – Database Fundamentals
Explored key database concepts and relationships:
- **Primary Key** – Uniquely identifies each record in a table; must be unique and non-null.
- **Secondary Key** – A candidate key not chosen as the primary; may allow duplicates or nulls.
- **Foreign Key** – Links one table to another by referencing the primary key, enforcing referential integrity.

### Real-world Relationship Examples
- **One-to-One:** Person ↔ Passport, Employee ↔ Company Car, Patient ↔ Medical Record  
- **One-to-Many:** Customer → Orders, Author → Books, Department → Employees  
- **Many-to-Many:** Students ↔ Courses, Movies ↔ Actors, Products ↔ Orders (via junction tables)

## Task – Relational vs Non-Relational Databases
### Relational Databases (RDBMS)
- Store data in structured tables with relationships defined by primary and foreign keys.
- Use SQL for queries (e.g., MySQL, PostgreSQL).

### Non-Relational Databases (NoSQL)
- Store unstructured or semi-structured data (documents, key-value, graph).
- More flexible and scalable, suited for social media, IoT, and large-scale real-time applications.

**Example:** E-commerce product catalogues benefit from NoSQL due to variable product attributes and scalability.

## Task – SQL JOIN Types
Explained six key join types and their uses:
- **Self Join:** Relates a table to itself (e.g., employees and managers).  
- **Inner Join:** Returns only matching rows from both tables (e.g., products with sales).  
- **Left Join:** All records from the left, and matching from the right (e.g., all customers, even without orders).  
- **Right Join:** All records from the right, matching from the left (e.g., all customers including those without orders).  
- **Full Join:** Combines all rows from both tables, showing nulls where no matches exist (e.g., all students and all library cards).  
- **Cross Join:** Combines every row with every row in another table (e.g., all colour and size combinations).

## Task – Database Design Essay
Designed a database for a small retail business to manage inventory, sales, and loyalty data.

### Key Steps
1. **Understanding Requirements:** Store data on inventory, sales, customers, and loyalty points.  
2. **Users:** Store owner and customers; owners need reports, customers view loyalty points.  
3. **Design:** Two main tables – inventory/sales data and customer information.  
4. **Implementation:** Created `Store_db` with SQL commands such as:  
   ```sql
   CREATE DATABASE Store_db;
   USE Store_db;
   CREATE TABLE DailySummary (
       SummaryDate DATE PRIMARY KEY,
       TotalCustomers INT,
       TotalProductsSold INT,
       TotalStockRemaining INT
   );
   INSERT INTO DailySummary (SummaryDate, TotalCustomers, TotalProductsSold, TotalStockRemaining)
   VALUES ('2025-09-29', 30, 150, 450);
   ```
5. **Maintenance:** Regular backups, accuracy checks, and data security measures.

##Task – SQL Practical Scenarios
Applied SQL queries to solve real-world data problems using the `world_db` dataset.

### Example Scenarios
- **Count Cities in USA** – Determine number of U.S. cities.  
- **Highest Life Expectancy** – Identify top country for longevity.  
- **Cities with ‘New’ in Name** – Compile list for marketing campaign.  
- **Population Queries** – Filter cities above 2M, between 500K–1M, or smallest populations.  
- **Sorting and Limiting Results** – Show first 10 cities, or rows 31–40 by population.  
- **Geographic Queries** – Find European cities, capital of Spain, and average population per country.  
- **Comparisons** – Capital city populations, high GDP per capita cities, and countries with low density.  
<img width="239" height="324" alt="SQL screenshot" src="https://github.com/user-attachments/assets/2de6c739-3c36-4c53-9f6f-f958e385b2e8" />


**Overall Focus:**  
Developed a comprehensive understanding of database structures, relationships, SQL joins, and practical data analysis.  
Learned how to design, implement, and query a functional database system using real-world scenarios.

# Cloud Computing Workbook Summary Week 4

## Day 1: Task 1 – Introduction to Cloud Computing
Researched fundamental cloud computing concepts and business benefits.

### What Cloud Computing Does
- Provides on-demand access to computing resources (storage, databases, software, servers) via the internet.
- **Real-world uses:** data storage, collaboration tools, backup/recovery, scalable apps, remote work enablement.

### Business Benefits
- **Cost-effective:** Pay-as-you-go model removes need for hardware investment.  
- **Scalable:** Instantly adjust resources based on demand.  
- **Secure and reliable:** High-level security, data recovery, and global access.  
- **Innovative:** Rapid deployment of apps/services.  
- **Remote access:** Enables flexible, distributed teams.

### Alternatives to Cloud
- **On-premises infrastructure:** Full control but high cost, limited scalability, requires maintenance and IT teams.

### Major Cloud Providers and Key Features
| Provider | Features | Common Uses |
|-----------|-----------|-------------|
| **AWS** | Broad services, global data centres, scalability | Hosting, analytics, disaster recovery |
| **Microsoft Azure** | Integrates with Microsoft 365, hybrid solutions | Business analytics, app hosting |
| **Google Cloud** | AI/ML tools, cost efficiency | Data processing, app development |
| **IBM Cloud** | Strong hybrid/AI focus | Enterprise and security-heavy workloads |

---

## Task – Cloud Service Models

### IaaS – Infrastructure as a Service
- Virtualised computing resources (servers, networks, storage).  
- **Use cases:** hosting websites, scaling workloads, disaster recovery.  
- **Examples:** AWS EC2, Azure VMs, Google Compute Engine.

### PaaS – Platform as a Service
- Provides ready-made environments for developers to build and deploy apps.  
- **Use cases:** app development, prototyping, scaling apps.  
- **Examples:** GCP App Engine, Azure App Service, AWS Elastic Beanstalk, Heroku.

### SaaS – Software as a Service
- Fully functional apps delivered via internet browser or app.  
- **Use cases:** collaboration, file storage, CRM, project management.  
- **Examples:** Microsoft 365, Google Workspace, Salesforce, Slack, Dropbox.

---

## Task – Cloud Deployment Models

| Cloud Model | Description | Example Use Case |
|--------------|--------------|------------------|
| **Public Cloud** | Shared resources provided by third-party vendors. | Small e-commerce site hosting via AWS. |
| **Private Cloud** | Dedicated environment for one organisation; higher control/security. | Bank protecting sensitive financial data. |
| **Hybrid Cloud** | Combines public and private clouds for flexibility. | Hospital storing records privately but using Azure for analytics. |
| **Community Cloud** | Shared between organisations with common goals or compliance needs. | Universities sharing research data. |

---

## Computer Misuse Act and Data Protection

### Task – Computer Misuse Act (1990)
Addresses unauthorised computer activity:
1. **Unauthorised Access** – Accessing data/systems without permission (e.g., student viewing confidential files).  
2. **Access with Intent to Commit Offences** – Hacking to commit fraud or theft (e.g., stealing banking info).  
3. **Unauthorised Acts to Impair Operation** – Disrupting systems or spreading malware (e.g., DoS attacks).

### Police and Justice Act (2006) Updates
- **Harsher penalties** – Up to 10 years imprisonment.  
- **New offence** – Intentional impairment of computer operations.  
- **Hacking tool offence** – Illegal to create, share, or use hacking software.

### Data Employers Can Store
- **Without permission:** Contact info, employment details, attendance/performance.  
- **With permission:** Health/medical data, biometric data, personal beliefs.

### Copyright and Software Piracy
- **Copyright infringement:** Sharing music or files without permission.  
- **Plagiarism:** Copying and submitting someone’s work without credit.  
- **Consequences:** Legal prosecution, financial loss, malware risk, lack of support, fines.

### Related Acts and Clauses
Covers legislation such as:
- **Computer Misuse Act 1990**
- **Police and Justice Act 2006**
- **Copyright Acts 1988 & 1992**
- **Data Protection Act 2018**
- **Health & Safety (Display Screen Equipment) Regulations 1992**
- **Consumer Rights Act 2015**

---

## Task – Explore Relational Data in Azure
Completed Lab 3: Investigated relational data within Azure environments using SQL-based queries, examining data structure, table relationships, and storage principles.

## Task – Explore Non-Relational Data in Azure
Completed Lab 4: Explored non-relational (NoSQL) data models in Azure, focusing on flexible data formats, scalability, and real-world cloud-based data handling.

<img width="713" height="600" alt="Azure Screenshot" src="https://github.com/user-attachments/assets/32e3622c-f741-4951-bd7c-fb7bb5c81dac" />

---

**Overall Focus:**  
Developed foundational cloud computing knowledge — from service models and deployment types to cybersecurity and data protection laws — with practical cloud labs in Microsoft Azure.



## Python Basics
- Created **FizzBuzz** using Python conditional logic and loops.

## Pandas Data Handling
Completed exercises with `student.csv` covering:
- **Data Loading & Exploration:** `read_csv`, `.head()`, `.info()`, `.describe()`
- **Indexing & Slicing:** Selected columns and filtered rows.
- **Data Manipulation:** Added, renamed, and dropped columns.
- **Grouping & Aggregation:** Used `groupby`, `value_counts`, and mean calculations.
- **Advanced Operations:** Built pivot tables, applied conditional grading logic, and sorted data.
- **Exporting Data:** Saved processed DataFrame to CSV.

## Day 4: Real-World Data Work
- Analyzed `GDP (nominal) per Capita.csv` — viewed rows, selected columns.
- Worked through collaborative Jupyter Notebook to apply learned data analysis and visualization techniques.

<img width="458" height="742" alt="PythonScreenshot" src="https://github.com/user-attachments/assets/836d4848-4c46-45d0-beba-34af5622a612" />

---
**Overall Focus:** Strengthened Python skills for data analysis and manipulation using pandas, preparing data for visualization and reporting.

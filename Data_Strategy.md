# DATA STRATEGY
## July 17, 2020
## Authors RIHAD & SAMIRA

The concept of MDM (Master Data Management) originated around 2008 when data warehousing and ERP solutions became popular in many firms. With the increase of data volume and the number of databases, and thus the increase in the number of applications for users to enter and read the data, it became more and more important to make sure that correct master data definitions are used so that there is a single truth in the data without discrepancies, duplications or being out-of-date

The first example is related to customer information. In a large organization, there could be multiple customer databases populated and managed by multiple applications, and the same customer in the real world could receive multiple direct mails or notifications from the same company. As the data grows, the master data consists of not only the customer information but also other key data assets, such as the data of prospects, suppliers, panelists, and products. MDM has been a challenge to implement because all 3 aspects of processes, technology, and tools are required to ensure that the master data is coordinated and synchronized across the enterprise

![](https://media.giphy.com/media/H0kxiS2RJF2HC/giphy.gif)

## WHY IS MDM IMPORTANT?
With the recent explosion of big data and rapid progress of analytics and IoT, the consistency of referencing and applying high-quality master data has become unprecedentedly crucial. An enterprise should not only need to make sure it has its key data assets efficiently and accurately managed, but also embrace new data

To fully realize the economic potential by joining or referencing the existing master data that the firm already owns, MDM needs to be an essential part of the data strategy for a company to grow and profit as well as one of the core missions for C-Suites and Executives such as CIO (Chief Information Officer)

There have been 2 main reasons for failures of MDM initiatives in the past 10 years

1. Relying on only technology and tools without buy-in and support from business units
2. Focusing on fixing and solving current data issues, without forward-thinking

For MDM to be successful, it needs to be first a business-driven process and embraced by business departments and executives. In many cases, fundamental changes to business processes will are required to establish and maintain unified master data and some of the most difficult MDM issues are not technical at all. Next, a forward-looking strategy is crucial in placing MDM as an essential part of data management in an organization, since it proactively lays the foundation for future success

Numerous experiences tell us that the implementation of MDM is easiest and smoothest when a dataset has just been introduced for ETL (exploration, transformation, and loading) and into an Ai project. Trying to fix for existing data assets and processes often require high cost and large effort, which also likely leads to a big impact on the current deliverables

Below is a comparison to illustrate the big differences between implementing MDM at the start Vs. fixing the issues of existing data and systems

* Delayed Implementation of MDM
* Implement MDM from the Beginning
* Duplicate processes in silos and costly developments
* Efficient and faster development with lower cost
* Data quality issues everywhere with no easy way to track down
* Fewer data quality issues that are faster to fix
* Low customer satisfaction
* High customer satisfaction
* Data asset potentials are not fully realized
* Generate more revenue opportunity
* Difficult to migrate to a new data platform
* Much easier to migrate to new data platform when needed

### FOUR STEPS TO SUCCESSFUL MDM IMPLEMENTATION

Once a MDM strategy is set, the next step is to implement the master data management within an enterprise. This is a big topic that can be covered in much depth in a book by itself. In this blog, we would like to give a very high-level introduction and point out 4 steps that are essential for the successful implementation of MDM

Each of the steps will warrant its own topic in the future with more elaborations and detailed examples

#### STEP 1: Establish Data Governance Embraced by the Entire Organization
This is the most critical and essential piece of MDM, and also the most difficult one. To enforce MDM requires the commitment of a data governance committee, which normally has the following structure

* Executive and Advisory Information Console - C-Suite and department heads
* Information Stewards - data governance managers/directors usually from IT or CIO organizations
* Data Stewards - domain experts from every business UNIT

The main missions of the committee include the following

* Establish data governance policies and procedures, and revise them based on business needs or changes in data, operations, and technology
* Establish regular communication channels to communicate and reinforce policies clearly
* Establish the right escalation process for data issues, prioritize and make decisions wisely and efficiently
* Ensure buy-in and ownership from all stakeholders

Below lists some of the key areas that the data governance committee should make decisions on

* A holistic view of the company’s datasets and what the core data assets are in the enterprise
* Document and define how data assets should be shared or used under the right security and regulatory constraints
* Establish standard definitions and business rules for data elements in a data asset or data object
* Determine the right course of actions or plans to ensure that data policies and procedures are enforced and executed across the organization
* Resolve definition ambiguities or conflicts

#### STEP 2: Apply MDM to New Data Applications
Always keep in mind that the simplest and most efficient way to make MDM successful is to enforce data consistency when the data is created. MDM is a long-term project and requires the long-term commitment of a firm. Any attempt to change the data in an ad hoc way renders the effort both ineffective and costly

Data governance policies and definitions are implemented throughout 2 channels

1. via any new projects and application development
2. by using data governance software

Many organizations’ MDM implementations stall because of the high cost and effort they faced when trying to fix the existing systems and issues; they did not realize that the best way to start with MDM is to apply it for going forward for new projects, which will test it out first and enable the organization to build up expertise and experience

In addition, most of the data governance should be implemented directly as part of data related projects into applications and reports. For example, data governance should enforce and propagate its definitions, policies, and principles into the following technical implementations

* Logical and physical design of databases (data modeling)
* Define column/field names and business rules in the ETL process
* Define display names and formulas in the reporting engine
* Configuration and set up when using third-party software such as ERP and Salesforce
* Enforce by Quality Assurance, and testing and User Acceptance Testing

#### STEP 3: Select the Right MDM Software
An ideal MDM software should have the following functionalities

1. Referencing and access to the metadata of master data assets in a company (e.g., RDBMS, Hive, flat files, etc.)
2. Enable information and data stewards to define and modify the definitions easily in the tool
3. Capable of reviewing the data and configure business rules to apply or enforce what has been defined in the data itself

There are many tools on the market that can do 1 and 2, but it's not easy to do 3 with the same tool. This is the reason why MDM software can be also a data integration tool at the same time or Vice Versa. Recent rapid progress in Ai has made such software more powerful with enhanced data management, which has a bright future in the coming years

Keep in mind that a tool is still a tool. Without the Governance committee and sponsorship from the C-Suite and executives, the software itself cannot play the magic and is not sufficient. In addition, constant communications and reinforcement by information stewards and data stewards in each department also play more essential roles than the software itself

#### STEP 4: Leverage MDM Capability to Manage Existing and Legacy Systems
Many firms may not have the luxury to create new master datasets from scratch, which means they need to revamp the existing database and related applications. Applying MDM to the existing data assets often requires a large amount of effort, which could also fail or abort due to complexity and cost. To make the MDM effort successful, careful planning is required to establish a road-map with multiple phases. Sometimes, it may be a better strategy to apply MDM only partially, until the data or system is migrated to the new platform, while focusing on applying MDM to new master data that are being added or new applications and processes that are being built for the enhanced and new data sources to be joined with the master data

## CONCLUSION
MDM has become a necessity for an organization to fully realize its datasets’ revenue and profit potential, but it's not easy to implement. MDM first needs to become a permanent part of the data strategy in order for the firm to have a long-term commitment. Next, it requires consistent governance and sponsorship from the top management, as well as persistent efforts from information stewards of IT/CIO departments and data stewards of business departments. The challenge of fixing existing data and system issues should not stop the adoption of MDM for an enterprise. Instead, applying MDM to the new data sources and new applications will lay the foundation to gradually apply it successfully to the existing data and systems

# Ethics Declarations
## Competing Interests
The authors declare no competing interests

# Rights & Permissions
Open Access This article is licensed under a Creative Commons Attribution 4.0 International License, which permits use, sharing, adaptation, distribution and reproduction in any medium or format, as long as you give appropriate credit to the original author(s) and the source, provide a link to the Creative Commons license, and indicate if changes were made. The images or other third party material in this article are included in the article’s Creative Commons license, unless indicated otherwise in a credit line to the material. If material is not included in the article’s Creative Commons license and your intended use is not permitted by statutory regulation or exceeds the permitted use, you will need to obtain permission directly from the copyright holder. To view a copy of this license, visit http://creativecommons.org/licenses/by/4.0/


![](https://drive.google.com/uc?export=view&id=1i7fzIUxz-oEs8V4uMdoZCQUl51NMrbVz)

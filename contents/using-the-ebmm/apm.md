# APM and Solution Domains

In 2007, Microsoft IT realized that it had a problem.  There were thousands of applications running, and the relationships between them were complex.  Keeping the entire portfolio of applications running required full time care and feeding and any change to an operating system or a new browser meant months of testing to make sure that the whole framework wouldn’t come crashing down around our ankles.

I was in the Enterprise Architecture team, and volunteered to be part of the effort to reduce the number of applications through a process we termed “portfolio rationalization.”  The goal was to remove redundant systems, obsolete systems, and systems that were unusually expensive to keep maintained.  Our challenge was to find these overlapping critters among thousands of systems.

A huge part of the problem — no single person knew every system.  In fact, for the majority of systems, no single person knew the entire system.  Documentation was often sparse or would describe technical details (how to install and configure it) but not functional details (what it did, who it was for, and why it needs to exist).  The latter information would have to be hand crafted from the knowledge of a broad array of people and, in some cases, from simply digging through the system itself (documentation, code, data, references, etc).

It was an Application Portfolio Management (APM) challenge of epic proportions, and we addressed it with a novel method… or at least we tried to.  To be completely honest, at the time I was a relatively young Enterprise Architect and didn’t understand change management and how to convince people to use novel methods.  So while two of us (Gabriel Morgan and myself, Nick Malik) created a method called “Solution Domains,” based on a taxonomy of systems, and created nice PowerPoint decks to explain it, it didn’t catch on.  So many lessons learned since that day!

The method is sound, and I stand behind it.  Unfortunately, the effort at Microsoft,  at that time, reduced to “shooting the low hanging fruit.”  In other words, finding apps with very few people willing to defend the app, challenging it’s need to exist, and if no one screamed, deleting it.  There was some effort made to replace really old apps with more modern ones, but those efforts were expensive and not necessarily fruitful.  No, the real portfolio rationalization wasn’t all that rational.  But it worked.  Microsoft managed to cut the sheer size of it’s Application Portfolio in half.  Good work.

## So what was this method based on Solution Domains?

We start with a taxonomy of systems and a definition useful for creating that taxonomy.  We then map each system to one (or a handful) of elements in that taxonomy.  Then we navigate through the taxonomy, assigning groups of systems to individual architects. Those architects are responsible for understanding all of the systems in their domain, and proposing methods for rationalizing that part of the portfolio.

It’s a fairly simple method.  The effort failed on the part where we assign architects to domains.  The company had already assigned project managers to own completely different portfolios of applications (grouped by company silo, not by functionality or data assets).  Result: systems with the loudest executives survived while systems with quiet (or new) execs were deleted.   What can I say?

Regardless, here is the taxonomy.  Perhaps it can be effectively used somewhere by someone.  It is no longer in use in Microsoft.

## Taxonomy

### 1.0 CM Channel Marketing

#### 1.1 Channel Planning + Measurement

Software services for defining the channels, determining and managing sales and marketing targets, tracking marketing investments and goals, and measurement of both marketing effectiveness and brand value.

#### 1.2 Market Segmentation Tools

Software services for organizing research about market segments, creating and managing segment profiles, targeting, filtering, suppression, categorization

#### 1.3 Market Competitive Intelligence

Software services for organizing research about competitor’s capabilities, products, and financials, along with strategies to respond

#### 1.4 Campaign Management

Software services for planning, managing, tracking and measuring marketing campaigns, including approval workflow, budgeting, scenario management, and response tracking

#### 1.5 Lead Generation

Software services for acquiring leads from internal and external sources by channel, including list management, evaluation, qualification and allocation of leads.

#### 1.6 Marketing Collateral Development

Software services involved in the creation of artifacts (images, content, layouts, standards, ad spots) that are developed for the purpose of branding, advertising, product positioning, lead generation, and guided selling.

#### 1.7 Selling Framework Management

Software services for defining marketing programs for each channel, business rules, selection of products for programs, eligibility of customers, durations, metrics

### **2.0 CCM Community and Collaboration Management**

#### 2.1 Collaboration Reporting and Analysis

Software services for measuring and tracking activity on a community or portal site, including click-through analysis and service level tracking

#### 2.2 Portal Authoring Tools

Software services for generating knowledge content, including editing, workflow, information rights management, template management, search management, tagging, and management of subject matter experts.

#### 2.3 Portal Display

Software services for managing the rendering and display of knowledge content including search query and results, delivery of subscribed content, collaboration, globalization, personalization, crawler and relevancy management, web-parts, and integration with back-end data sources.

### 3.0 SCM Supply Chain Management**

#### 3.1 SCM Materials Procurement

Software services used to select, order, receive, track, return, and control the flow of materials into the supply chain.

#### 3.2 Supplier Management

Software services used to recognize, enroll, collaborate, report, and retain supply chain suppliers.   (there may be some overlap with partner relationship management on this one)

#### 3.3 SCM Validation

Software services used to manage, measure, and validate the capabilities and quality of vendor-supplied parts and assemblies against agreed levels of quality and service.

#### 3.4 Manufacturing Management

Software services used to manage, measure, and control the manufacturing processes and quality control used for manufacturing parts, assemblies and finished products.

#### 3.5 SCM Forecasting

Software services used to plan for supply chain variations based on demand fluctuations, supply and manufacturing conditions, vendor capabilities, and design changes.

#### 3.6 SCM Logistics

Software services used to manage, document, dispatch, and control the movement of materials, assemblies and finished goods through transportation channels and warehousing, including reverse logistics (returns)

### **4.0 PM Project Management**

#### 4.1 Release Management

Software services for managing the promotion of software to another environment such as Staging, User Acceptance and Production environments.

#### 4.2 Project task Management

Software services for managing the definition, execution/completion, status, dependencies, of project tasks

#### 4.3 Project Resource Management

Software services for finding, allocating, reserving and forecasting project resources including people, facilities, supplies, et al. This set of tools is similar to those needed by Workforce Management.

4.4 Engagement Management

Software services for managing the engagement of a project including features which support project portfolio management, budgeting, costing, 3rd party contractor management, status reporting and conditions of satisfaction

4.5 Quality Management

Software services to manage project performance review activities (e.g. project process quality, project artifact quality, and technical solution quality) such as Review Questionnaire, Findings and Recommendations Registry, Quality Analysis, and workflow

4.6 Time and Expense Management

Software services used to manage project resource Time and Expense such as Time Entry, Time Accounting and Reporting, project Expense Entry, and Expense Accounting and Reporting.

**5.0 RM Relationship Management**

5.1 Agreement Management

Software services involved with the creating of reusable templates for sales agreements, including the management of legal clauses, the creation of configured quotes, the presentation of quotes in a proposal package with legal documents, and the collection of electronic signatures on legal documents

5.2 Order Management

Software services involved in collecting orders from customers for products and subscriptions, validating the order against the agreement, generating the invoice and setting up the obligations under the order for fulfillment.

5.3 Contact management

Software services involved in tracking and responding to contacts between the Enterprise and customers, partners and suppliers, including call center management as well as tracking the contacts from communities and subscriptions as well as contact lifecycle. Data elements include Account, Incident, Inquiry, and Communication Preference.

5.4 Event Management

Software services used for managing events such as online registration, room booking, event logistics planning, resource material storage and workflow

5.5 Opportunity Management

Software services used for managing the sales opportunities and leads, from lead management and proposal tracking to collaborative selling, and Forecasting. Data elements mastered in this domain include Sales Territory, Lead and Opportunity.

5.6 Sales Engagement

Software services used for managing the sales engagement process including workflow, direct sales, guided selling, competitive escalation, and product configuration and the distribution of price data.

5.7 Customer Attribute Asset Management

Software services used for segmenting and attributing data to customers for the sake of profiling and later data mining/analysis. These tools track and manage the qualifications, awards, certifications, and rankings earned by customers and partners in their profiles, and help match up solutions that may lead to opportunities.

5.8 Party Management

Software services used to manage the data related to external companies, people, and organizations (parties) for the purposes of synchronizing all relationship information.   Tools include external data acquisition and integration, and duplicate party mgmt

5.9 Support Incident Management

Software services used for managing Incidents such as Call Queuing and Routing, Incident Request, Live web collaboration, service entry, eligibility verification, Incident Resolution, Incident Issue Escalation, and Workflow. Used for issue resolution for all customer facing activities, including product support requests, billing disputes, internal information requests (legal, HR and IT support services), complaint management, etc.   Note that management of eligibility claims is handed in Claim Management.

**6.0 OM Obligation Management**

6.1 Claim Management

Software services involved with the management and delivery of products or services that are only fulfilled when claimed by the customer, including incentives, support incidents, insurance claims, and subscription-based entitlements.

6.2 Customer Asset

Software services used for assigning entitlements to customers for subscriptions, licenses, support incidents (etc) that can be claimed, along with the billing processes used for periodic billing

6.3 Digital Delivery

Software services involved in the digital distribution and delivery of intellectual property in a secure manner to partners and customers who are legitimately authorized to receive it. This includes injection of license keys, product activation, validation of license enforcement, and tracking of license key usage to the product.

6.4 Obligation Planning & Forecasting

Software services used to manage the operational and budgetary implications of the variations in demand for customer asset claims and subscription services.

**7.0 PLM Product Lifecycle Management**

7.1 PLM Analytics

Software services for auditing and logging the process, lifecycle events, and controls for the product lifecycle.

7.2 IP Asset Management

Software services for managing, tracking, archiving, and securing IP assets

7.3 Manufacture Design

Software services involved in designing the processes, tools, facilities, and organizational structures needed to successfully manufacture a product.

7.4 Product End of Life Control

Software services involved with minimizing the costs and maximizing the return of products and product artifacts as the product nears the end of its lifespan. This includes IP management, selling off artifacts, archiving of IP, designs, business records, service and customer data.

7.5 Requirements Management

Software services involved in eliciting and collecting requirements and perceived defects, surveying prospects, arranging and coordinating target audiences, managing requirement lifecycles, prioritizing requirements, and tracing across products and versions.

7.6 Product R&D

Software services used for managing the creation of product artifacts and the definition of service product artifacts

**8.0 PIM Product Information Management**

8.1 PIM Analytics

 Software services for attributing the product hierarchies to support business intelligence and reporting on product attributes.

8.2 Assembly and BOM Management

Software services involved with managing the hierarchy of components within a Bill of Materials needed to correctly assemble a manufactured product.

8.3 Product Definition and Collateral

Software services involved with creating a vision of a product to meet the needs of a marketplace, positioning, price planning, features definition, and management of the documents produced during these processes.

**9.0 CSR Corporate Services and Relations**

9.1 Audit and Compliance Management

Software services involved with insuring that corporate obligations to auditors, investors, and regulatory agencies are kept, including Software services for managing audit processes, investigative compliance processes, and reporting requirements

9.2 Philanthropy / Charity

Software services for tracking and managing the contributions of the corporation and employees, including matching funds, grant program and request management, efficacy measurement, and publication of results.

9.3 Travel and Expense Management

Software services for managing travel, including pre-trip approval, online booking, creation and management of expense reports, policy enforcement, and reporting

9.4 Government / Industry Affairs

Software services for managing specific contacts with government agencies, industry consortia, legislative and government advocates/lobbying agencies, including legal entity management, filing of documents and memberships, and tracking of corporate obligations

9.5 Environment, Health, and Safety

Software services used in the creation, management, and enforcement of policies for product safety, plant safety, hazardous substance notification and reporting, waste and emissions management, and occupational health and safety. This includes management and auditing of vendors, as well as Software services for collecting and investigating reports, and reporting to regulatory agencies and community groups.

9.6 Global Trade Services

Software services used to track and manage customs and compliance with government agencies and regulatory bodies needed for world trade compliance, including validating that orders can legally be sent to specific countries, companies or individuals according to the policies of local jurisdictions.

9.7 Corporate Transportation

Software services used to manage corporate assets used to transport goods and people around or between corporate facilities, including maintenance, dispatch, and route management.

**10.0 FM Financial Management**

10.1 Financial Planning

Software services for corporate budgeting, tax planning, strategic financial planning and resource targeting.

10.2 Investment Management

Software services for managing capital assets, investment projects, cash management and portfolio and risk management.

10.3 Billing And Collections

Software services used in the billing and collection of payments. This includes credit management, dispute management, collections management, electronic bill presentment, billing of time-and-materials engagements, royalty management, reimbursements and rebates, bank relationship management, and third-party rebilling.

10.4 Financial Accounting

Software services involved in managing financial accounting including, GL, AR, AP, fixed assets accounting, cash management, tax accounting, inventory accounting, and financial statement generation.

10.5 Management Accounting

Software services involved in financial management of internal resources, including profit center accounting, cost center and internal financial management, investment management, project accounting, and product cost accounting

10.6 Incentive and Commission Management

Software services involved with allocating sales to individuals, teams, organizations and subsidiaries for the purpose of calculating incentives and commissions, both for distribution to employees as well as partners. This includes cooperative marketing, sales commissions, and subsidiary financing.

**11.0 APS Asset Procurement and Security**

11.1 Real Estate Management

Software services used to manage the real property owned, leased, or managed by the enterprise, including support for property acquisition, portfolio management, property management, technical management, and support processes.

11.2 Fixed Asset Management

Software services used to manage fixed assets, including inventory management and tracking.

11.3 Physical Security Management

Software services involved with managing security devices, systems, and networking, as well as Software services for identifying and prioritizing threats, auditing and logging of processes, and resource allocation related to the physical security of the corporate premises.

11.4 Network Asset Management

Software services involved in managing identities, group management, and password policies as well as Software services for identifying and prioritizing threats, tracking and managing malware, taking inventory of installed client and server software, and other desktop management functions that create a secure corporate networking environment for sharing electronic resources.

11.5 Art Collection Management

Software services used to manage the acquisition, valuation, and control of art assets owned by the enterprise.

11.6 Indirect Procurement

Software services used to manage the procurement of supplies and materials for business consumption.   This includes Software services for B2B invoice receipt, procurement policy review, financial settlement as well as time entry of billed time from vendors.

**12.0 HR Human Resource Management**

12.1 Training and Readiness

Software services involved with manage readiness for Individuals and Organizations including training schedules, training resources and materials, training plans and training delivery management

12.2 Workforce Planning

Software services for finding and reserving talented people (including their availability) for internal or external assignment. Tools in this platform support forecasting and demand management of talent resources.

12.3 Talent Management

Software services used for tracking workforce talent, capabilities, performance, and readiness.   This domain supports performance review and commitments, employee training, mentoring, career planning and employee satisfaction surveys.

12.4 Benefits Management

Software services used for tracking employee benefits, leave administration, promotions, stock, retirement, and electronic paystub communication.

12.5 Time and Attendance

Software services used to manage project resource Time such as Time Entry, Time Accounting and Reporting.

12.6 Payroll and Legal Reporting

Software services used the distribution of payroll including direct deposit, deductions, and tax reporting.

12.7 Staffing (Recruiting)

Software services used to track job opportunities, applicants, and interviews.

12.8 Global Employee Management

Software services used to manage legal and cultural differences for managing the workforce, including immigration filing and workflow

**13.0 ITM Information Technology**

13.1 Planning and Delivery Management

Software services used to manage and control the process of defining, funding, controlling, managing, and accounting for the projects that create capabilities in the Information Technology ecosystem.

13.2 Life-Cycle Data Management

Software services used to manage the taxonomy, sources, relationships, management, quality measurement, quality improvement, and secure control of data assets within the enterprise.

13.3 Architecture

Software services used to manage the definition, modeling, compliance, and adoption of business process, application, information, and technological architectures.

13.4 Integration Management services

Software services used to transmit and control data connections and system functional interdependencies between different platforms in the Information Technology ecosystem. This includes standards and controls for adoption of Business-to-Business connections between the enterprise and our partners, suppliers, and customers.

13.5 Operational Support Services

Software services used to manage the day-to-day operations of providing data and telecommunications support, including Helpdesk, hardware maintenance, device management, network identity management, disaster recover, and intrusion detection.

**14.0 KM Knowledge Management**

14.1 Asset Storage Management

Software services involved in the tracking, maintenance, and control of digital assets, including data storage, digital intake, image scanning, indexing, and search. This includes digital corporate records, legal assets, and document management. These services are also used by the Collaboration and Communication Management family to manage and control portal documentation.

14.2 Information Access Identity Management

Software services involved in managing the user identities, roles, permissions, permission rules, repositories, and auditing of access for individuals and organizations to gain access to documents, records, portal content, and system data.

14.3 Information Lifecycle Management

Software services involved in the tracking, maintenance, and control of information assets, including search, metadata control, record retention, physical document inventory and management, and archiving.

14.4 Asset Duplication Management

Software services involved in insuring that the data managed in asset storage is correctly collected and not duplicated.

**15.0 BI Business Intelligence**

15.1 Strategic Enterprise Management

Business Intelligence and reporting software services used to manage the corporation, including support for balanced scorecards, risk management, strategic planning, and internal investment planning.

15.2 Operations Analytics

Business intelligence and reporting software services used to manage and illustrate corporate financials, including management reporting, budget analysis, forecasting, profitability, cost analysis, and cash flow management as well as reporting software services used to manage and illustrate corporate financials, including management reporting, budget analysis, forecasting, profitability, cost analysis, and cash flow management predict, control, and analyze the various operational processes that feed the value chain, including marketing, sales, procurement, inventory, manufacturing, logistics, customer service, quality, customer asset management and workforce readiness.
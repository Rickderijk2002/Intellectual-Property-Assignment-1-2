# Assignment 1: Task Division (Trio 1)

Three people, three approximately equal contributions, within the 3000-word limit.

Roles are **Person A, Person B and Person C**.

**Proposal: Gilbert takes Person A and additionally acts as Case Owner and Integrator**, based on his lead role in the original Business Monitor/LBT project, including its implementation and final report.

Persons B and C are assigned by the trio.

The report analyses one common and agreed version of the Learning Benchmarking Tool (LBT). All section owners must use the case definition below and must not independently change the architecture, data flows, purposes, actor roles or other assumptions.

---

## Step 0, together: agreed case definition

### Project

The report analyses the **intended operational Learning Benchmarking Tool (LBT)** developed for Business Monitor, rather than only the current synthetic-data MVP.

The current MVP uses synthetic data as a proof of concept. The operational LBT is intended to work with real organisational learning and participant data.

Participating organisations use Business Monitor to evaluate the effectiveness of organisational learning programmes.

### Processing architecture

Business Monitor administers participant surveys on behalf of participating organisations. For survey administration, Business Monitor therefore initially processes directly identifiable participant data required to contact participants and manage the survey process.

After collection, Business Monitor pseudonymises participant-level survey and learning data for analytical processing.

Business Monitor retains the information required to link participant identities to pseudonymous identifiers only for as long as necessary to administer the relevant survey cycle, including required follow-up measurements. The identity data and re-identification information are stored separately from the analytical dataset and are subject to restricted access.

Once re-identification is no longer necessary for the survey purpose, the identifying information and mapping are deleted in accordance with a defined retention policy.

The pseudonymised participant-level data are used to calculate programme-level indicators based on the Kirkpatrick L1-L4 framework:

- L1: Reaction;
- L2: Learning;
- L3: Behaviour;
- L4: Results.

The LBT also contains predictive analytics. These models operate at **programme level only**. They are intended to predict or estimate programme-level learning outcomes and KPIs.

The LBT does **not** predict individual employee performance, behaviour, capability or future outcomes and is not intended to support employment decisions concerning individual participants.

Data from participating organisations are subsequently aggregated for cross-organisational benchmarking. Customer-facing benchmark outputs are intended to be aggregated and anonymised.

The resulting high-level processing chain is:

**Survey administration with identifiable data  
→ pseudonymisation by Business Monitor  
→ separate and restricted storage of identity/re-identification information  
→ pseudonymised participant-level analytical processing  
→ programme-level KPI calculation  
→ programme-level predictive analytics  
→ cross-organisational aggregation and benchmarking  
→ aggregated/anonymised customer output**

Identifying information and the re-identification mapping are retained only for as long as required for survey administration and necessary follow-up measurements, after which they are deleted according to the defined retention policy.

### Personal-data layers

For consistency, distinguish between three data layers throughout the report:

1. **Survey-administration and identification data**
   - directly identifiable participant data;
   - for example name, email address, organisation and learning programme;
   - the information required to link participant identities to pseudonymous identifiers;
   - used only where necessary to administer the survey cycle and required follow-up measurements;
   - stored separately from the analytical dataset with restricted access;
   - deleted when re-identification is no longer necessary for the survey purpose.

2. **Analytical data**
   - pseudonymised participant identifier;
   - survey responses;
   - learning and evaluation measurements;
   - pre/post learning scores and other relevant LBT indicators;
   - used to calculate programme-level L1-L4 KPIs.

3. **Benchmark data and outputs**
   - aggregated programme-level KPIs;
   - programme-level model outputs;
   - cross-organisational benchmark statistics;
   - intended to be anonymised so that individual participants are no longer reasonably identifiable.

Pseudonymised participant-level data are still treated as personal data. Pseudonymisation must therefore not be treated as equivalent to anonymisation.

### Special-category data

The standard LBT is **not intended to collect or process Article 9 GDPR special-category personal data**.

The analysis should nevertheless consider whether survey design, particularly free-text responses, could unintentionally result in the collection of special-category data and whether this can be prevented through data minimisation and privacy-by-design measures.

### GDPR roles: working hypothesis

The GDPR role of Business Monitor must be assessed **per processing operation** rather than assigning one role to Business Monitor for the entire LBT.

The working hypothesis is:

- the participating organisation acts as **controller** for employee learning evaluation;
- Business Monitor may act as **processor** when administering surveys and performing agreed analytics on behalf of the participating organisation and according to its instructions;
- Business Monitor may act as **controller** for cross-organisational benchmarking where it independently determines the purpose and essential means of that processing.

These are working hypotheses. The report must legally assess and justify the controller/processor determination rather than presenting the roles as assumptions.

### Consistency rule

All three authors must use this Step 0 case definition.

Do not independently change:

- the LBT processing architecture;
- the three data layers;
- the purposes of processing;
- the level at which predictions are made;
- the assumption concerning individual decision-making;
- the treatment of special-category data; or
- the working hypothesis concerning GDPR roles.

If legal analysis shows that one of these assumptions should be changed, discuss this with the trio before changing the report.

---

## The split

| Role | Owns | Advice share (Section IV) | Approx. words |
|---|---|---|---|
| **Person A – Gilbert** | **Section I: Introduction + Description.** Operational LBT, processing architecture, personal data, data subjects, Article 9 assessment and GDPR actor roles. Also acts as **Case Owner and Integrator**. | Data alternatives and architecture: data reduction, pseudonymisation, aggregation and anonymisation | ~500 + ~200, plus Case Owner/Integrator |
| **Person B** | **Section II: How are the data processed?** Processing purposes and application of Article 5 GDPR principles | Technical and organisational measures, retention, security, accountability and data protection by design | ~550 + ~250 |
| **Person C** | **Section III: On which legal basis?** Lawful basis per processing purpose and controller, including assessment of relevant Article 6 grounds | Overall lawful-processing assessment and required governance changes | ~900 + ~150 |

The exact allocation may change during integration. The final report must remain below the assignment's 3000-word limit.

**Why this balances:** Person C carries the most substantial lawful-basis analysis but writes the smallest separate advice contribution. Person A has a smaller analytical section and therefore also takes the **Integrator** role.

### Case Owner: Person A

Person A was closely involved in the original Business Monitor/LBT project, including its implementation and final report, and therefore acts as the **factual point of reference for the LBT case**.

The Case Owner is responsible for maintaining consistency concerning:

- the LBT system architecture;
- the original and intended operational functionality;
- the data flows;
- the distinction between the synthetic MVP and the intended operational LBT;
- the variables and data used by the system;
- the calculation of the Kirkpatrick L1-L4 indicators;
- the programme-level predictive models;
- the cross-organisational benchmarking functionality.

Questions from Persons B and C concerning how the LBT works, what data it processes, or what the intended functionality is should first be checked against the agreed Step 0 case definition and, where necessary, discussed with the Case Owner.

The **Case Owner role concerns factual consistency only**. It does not give Person A authority over the legal analysis of Persons B and C.

Each section owner remains responsible for:

- identifying the relevant legal provisions and case law;
- applying those rules to the agreed LBT facts;
- considering counterarguments;
- reaching their own legally reasoned conclusions.

If the legal analysis indicates that an assumption in the Step 0 case definition should be changed, this must be discussed by the trio before the case definition or another section is changed.

The Integrator is responsible for:

- report header;
- group number;
- names and student numbers;
- final word count;
- consistent terminology;
- citation and footnote formatting;
- Technology Statement;
- final consistency check;
- rendering the final PDF from the `.qmd`.

---

# Person A

**Assigned to: Gilbert**

In addition to Section I, Person A acts as Case Owner and Integrator.

Because Sections II and III depend on an accurate description of the processing, Person A should establish the factual LBT processing architecture early and make it available to Persons B and C before they complete their legal analyses.

## Section I: Introduction + Description

Person A establishes the factual and legal foundation used by Sections II and III.

### A1. Describe the operational LBT

Briefly explain:

- what Business Monitor's Learning Benchmarking Tool does;
- that the current MVP is based on synthetic data;
- that this report analyses the intended operational version using real organisational learning data;
- that Business Monitor administers participant surveys;
- that participant-level data are pseudonymised for analytics;
- that L1-L4 KPIs are calculated at programme level;
- that predictive analytics operate at programme level;
- that cross-organisational benchmarking uses aggregated data.

Do not describe the LBT as making individual employee predictions or employment decisions.

### A2. Identify the personal data

Identify which data qualify as personal data.

Use the three agreed data layers:

1. identifiable survey-administration data;
2. pseudonymised participant-level analytical data;
3. aggregated/anonymised benchmark data.

Describe how Business Monitor performs pseudonymisation, including the temporary retention and separate storage of the information required to link participant identities to pseudonymous identifiers.

Do not treat pseudonymisation as anonymisation. The analytical dataset remains personal data while participants can be re-identified using additional information.

Explicitly distinguish **pseudonymisation** from **anonymisation**.

Assess whether the benchmark outputs can reasonably be regarded as anonymous rather than merely pseudonymised.

### A3. Identify the data subjects

Identify the natural persons whose personal data are processed.

The primary data subjects are employees or other participants taking part in organisational learning programmes.

Consider whether other natural persons appear in the data and whether they need to be addressed.

### A4. Article 9 special-category data

Assess whether the intended LBT needs Article 9 special-category personal data.

The standard design assumption is that these data are not required.

Consider whether free-text survey responses or unnecessary demographic variables could nevertheless introduce special-category data.

### A5. Controller and processor determination

Determine GDPR roles **per processing operation**.

At minimum analyse:

1. the participating organisation's employee learning evaluation;
2. Business Monitor's survey administration;
3. Business Monitor's participant-level analytical processing;
4. Business Monitor's cross-organisational benchmarking.

Do not simply state:

> Business Monitor is both controller and processor.

Explain **why** it has a particular role for each relevant processing operation by applying the GDPR controller/processor concepts to the LBT facts.

### Person A: Section IV contribution

Develop advice concerning whether personal-data processing can be avoided or reduced.

Consider:

- collecting fewer directly identifying data;
- deleting or separating contact information after survey administration;
- early pseudonymisation;
- separation of the identity key from analytical data;
- aggregation;
- anonymisation of benchmark outputs;
- minimum cohort sizes;
- avoiding unnecessary demographic attributes;
- limiting or avoiding free-text fields where appropriate.

---

# Person B

## Section II: How are the data processed?

Person B analyses the purposes and the data protection principles.

### B1. Define the processing purposes

Distinguish between the main processing operations and purposes:

1. **survey administration**;
2. **participant-level learning analysis**;
3. **programme-level KPI calculation**;
4. **programme-level predictive analytics**;
5. **cross-organisational benchmarking**.

Avoid describing all LBT processing as one generic purpose.

### B2. Apply Article 5 GDPR

Apply the relevant Article 5 GDPR principles to the actual LBT processing.

Cover:

#### Lawfulness, fairness and transparency

Assess whether participants can reasonably understand:

- which data are collected;
- why they are collected;
- that Business Monitor is involved;
- how their responses are analysed;
- whether their data contribute to cross-organisational benchmarking.

Coordinate the detailed lawful-basis analysis with Person C.

#### Purpose limitation

Pay particular attention to the transition from:

**employee learning evaluation → cross-organisational benchmarking**

Assess whether the purposes are sufficiently specified and whether later benchmarking use requires separate consideration.

#### Data minimisation

Assess which data are actually necessary for:

- survey administration;
- participant-level analytics;
- programme-level KPI calculation;
- benchmarking.

Consider whether identifiable information remains necessary throughout the survey cycle and for required follow-up measurements, and whether it can be deleted once those purposes have been completed.

#### Accuracy

Assess the importance of accurate survey and learning data for KPI calculation and programme-level predictive analytics.

Consider limitations associated with survey responses and derived KPIs.

#### Storage limitation

Assess whether the retention of identifiable participant data and the re-identification mapping is necessary throughout the survey cycle, including follow-up measurements, and determine how the retention period should be linked to that purpose.

Assess whether deletion of the identifying information and mapping once re-identification is no longer necessary satisfies the storage limitation principle.

Consider different retention requirements for:

- identifiable survey-administration data;
- pseudonymised analytical data;
- aggregated/anonymised benchmark data.

Do not assume that one retention period is appropriate for every data layer.

#### Integrity and confidentiality

Consider the security implications of Business Monitor receiving directly identifiable survey data and maintaining a pseudonymisation mechanism.

Assess the separation between:

- directly identifiable participant data;
- the re-identification mapping; and
- the pseudonymised analytical dataset.

Consider whether access to the identity and re-identification information should be technically and organisationally restricted to personnel responsible for survey administration.

#### Accountability

Assess how controllers can demonstrate compliance.

### Person B: Section IV contribution

Develop concrete technical and organisational measures.

Consider:

- role-based access control;
- separation of identifiable and analytical datasets;
- secure storage of the re-identification key;
- encryption;
- logging;
- deletion and retention schedules;
- minimum cohort sizes for benchmark reporting;
- prevention of re-identification from small groups;
- records of processing activities where required;
- processor agreements where required;
- DPIA where applicable;
- documented assessments;
- data protection by design and by default.

Recommendations must follow from problems or risks identified in Section II rather than becoming a generic GDPR checklist.

---

# Person C

## Section III: On which legal basis?

Person C analyses lawful processing **per processing purpose**.

Do not select one Article 6 ground for the entire LBT.

### C1. Participating organisation: employee learning evaluation

Determine:

- who is controller;
- the purpose of processing;
- which Article 6 ground or grounds could potentially apply;
- the legal requirements of those grounds;
- whether those requirements are satisfied in the LBT context.

Consider the employment context when assessing consent.

### C2. Business Monitor acting on behalf of the organisation

Analyse Business Monitor's role when:

- administering surveys;
- collecting responses;
- pseudonymising participant data;
- performing agreed analytics for the organisation.

Explain the relationship between the controller's lawful basis and Business Monitor's processing as processor.

Consider the requirements governing the controller-processor relationship where relevant.

### C3. Business Monitor's cross-organisational benchmarking

If Business Monitor qualifies as controller for this separate processing purpose, determine which Article 6 lawful basis could support the processing.

Give particular attention to **legitimate interest**, if relevant.

Do not merely state that legitimate interest applies.

Analyse:

1. the legitimate interest being pursued;
2. whether the processing is necessary for that interest;
3. whether participants' interests, rights or fundamental freedoms override that interest.

Consider reasonable expectations of employees and the safeguards built into the LBT architecture.

### C4. Consent

Assess whether consent is a suitable lawful basis where relevant.

In particular consider whether consent in an employment context can satisfy the requirement that consent be freely given.

Do not assume that participation in a survey automatically provides valid GDPR consent for every subsequent processing purpose.

### C5. Article 9 if necessary

The working assumption is that the standard LBT does not require special-category data.

If the analysis identifies unavoidable Article 9 processing, determine whether an Article 9(2) exception would be available.

Do not use Article 9 analysis merely because the data concern employees.

### Person C: Section IV contribution

Provide the lawful-processing component of the overall advice.

State:

- which processing activities can continue under which conditions;
- where the lawful basis is uncertain or problematic;
- whether purposes need to be separated more clearly;
- whether Business Monitor's controller and processor activities require clearer governance separation;
- what changes are required before operational deployment.

---

# Lecture material

The lectures already given provide the starting point for the legal analysis.

| Role | Primary lecture material |
|---|---|
| **Person A** | Lecture 1: GDPR scope and concepts, personal data, data subjects, controllers and processors |
| **Person B** | Lecture 3: Article 5 data protection principles |
| **Person C** | Lectures 2 and 4: Article 6 lawful processing, consent, contract, legitimate interest and special-category data |
| **All** | Lecture 1 legal reasoning approach: identify the relevant rule/concept → identify the legal test → apply it to the LBT facts → reach a reasoned conclusion |

Lecture 5 should be reviewed after it has been given, particularly for fairness, transparency, profiling and automated decision-making.

Because the LBT predictive models operate at programme level rather than making individual employee decisions, do not assume that individual automated decision-making rules apply. Assess their relevance based on the actual processing.

---

# Legal research responsibility

Each section owner is responsible for identifying and checking the **primary legal provisions, relevant case law and appropriate recommended/additional reading** used in their section.

Lecture slides are a starting point for identifying legal issues, not a substitute for authoritative legal sources.

The Evaluation Guide places the greatest weight on **Analysis & Assessment (9/15 points)**. Therefore, each section should demonstrate:

1. identification of the relevant legal issue;
2. identification of the applicable legal rule or concept;
3. explanation of the legal test;
4. application to the concrete LBT facts;
5. consideration of relevant counterarguments or uncertainty;
6. a reasoned conclusion.

Avoid merely describing GDPR provisions.

The reasoning should show **why** a provision applies and **how** it affects the LBT.

---

# Section IV: Advice

Section IV is developed jointly.

It should not become a generic list of GDPR recommendations.

Each recommendation must follow logically from the analysis in Sections I-III.

The advice should address at least:

### Data architecture

- minimisation of identifiable data;
- pseudonymisation;
- separation of identity and analytical data;
- aggregation;
- anonymisation of benchmark outputs;
- protection against re-identification.

### Governance

- clear separation of Business Monitor's processor and controller activities;
- appropriate controller-processor arrangements;
- clearly documented processing purposes and responsibilities.

### Transparency

- clear information for participants concerning Business Monitor's role;
- participant-level analytics;
- programme-level analytics;
- cross-organisational benchmarking.

### Retention

- separate retention rules for identifiable, pseudonymised and anonymised/aggregated data.

### Security

- access control;
- encryption;
- secure key management;
- logging;
- appropriate organisational controls.

### Accountability and privacy by design

- appropriate documentation;
- DPIA where required;
- documented legitimate-interest assessment where relied upon;
- data protection by design and by default;
- periodic review of whether participant-level data remain necessary.

### Functional limitation

The LBT should remain a programme-level learning evaluation and benchmarking system.

Individual-level predictions or use of LBT outputs for automated employment decisions concerning individual participants are outside the agreed scope and should not be introduced without a separate legal and privacy assessment.

---

# Review and integration

1. **Case-definition check**

   Before drafting, all three authors confirm that they are using the Step 0 architecture.

2. **Peer review in a ring**

   - A reviews B;
   - B reviews C;
   - C reviews A.

   Review the legal reasoning and factual consistency, not just language.

3. **Cross-section consistency review**

   Before final integration, Person A performs a factual case review to verify that Sections I-IV describe the LBT consistently.

   This review checks factual consistency only and must not override the independent legal conclusions of Persons B and C.

   Check specifically that:

   - actor roles are consistent between Sections I and III;
   - purposes are consistent between Sections II and III;
   - Person C uses the same processing operations identified by Person B;
   - advice addresses risks actually identified in Sections I-III;
   - pseudonymisation and anonymisation are not used interchangeably;
   - programme-level prediction is not accidentally described as individual profiling.

4. **Section IV sitting**

   All three authors combine their advice contributions into one coherent recommendation and conclusion.

5. **Cross-trio review**

   Trio 2 reads the complete draft according to the agreed group process.

6. **Final integration by Person A**

   Person A checks:

   - one consistent voice;
   - one set of LBT facts;
   - consistent terminology;
   - correct citations and footnotes;
   - no unnecessary repetition;
   - compliance with the 3000-word limit;
   - complete report header;
   - complete Technology Statement;
   - successful final PDF rendering.

---

# Suggested timeline

| By | Milestone |
|---|---|
| **3 Oct** | Step 0 case definition agreed and roles A/B/C assigned |
| **23 Oct** | Drafts of Sections I, II and III plus individual advice contributions completed |
| **30 Oct** | Ring review completed and joint Section IV session held |
| **4 Nov** | Integrated draft sent to Trio 2 for cross-review |
| **10 Nov** | Final substantive and legal review completed |
| **13 Nov, 23:59** | Submission deadline |

Aim to have the substantive report complete by 10 November. The final days should be reserved for checking, formatting and submission rather than substantive rewriting.

---

# AI rule, for everyone

Follow the assignment's applicable AI Index requirements.

Under **AI Index Level 2**, AI may only be used within the limits permitted by the course, such as reviewing a completed draft for spelling, grammar, coherence and referencing where allowed.

AI must not be used to generate assignment text, tables or graphs where this is prohibited by the course rules.

Anyone using an AI tool must inform the Integrator so that its use can be correctly reported in the **Technology Statement**.

When in doubt about whether a particular use is permitted, check the official course or assignment instructions before using the tool.
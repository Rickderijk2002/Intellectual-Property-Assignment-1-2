---
status: active
project: school
type: reference
subtype: assignment-case-source
course: Intellectual Property and Privacy
course_code: JM0160-M-6
assignment: 1
last_updated: 2026-10-02 12:26
---

# Business Monitor: DIiA Final Report (Learning Benchmarking Tool)

The group's own earlier project, chosen as the case for Assignment 1 (data protection). Written by
Team 5 for Data Entrepreneurship in Action I, dated 2025-12-16: Gilbert Laanen, Rick de Rijk,
Stefan Vonk, Tycho van Rooij, Thom Verzantvoort. This is **the facts of the case**, not a lecture
source. Original PDF: `00 - Inbox/DliA_Final_Report.pdf`.

**Conversion caveats.** Machine conversion with markitdown, 2026-10-02. The table of contents was
dropped. Figures 1 to 12 (dashboards, canvases, schema diagram) are lost, only their captions
survive. Multi-column tables (Tables 1 to 7, Appendices A to D) came out with cells in scrambled
order, so check the original PDF before quoting any figure from a table. Lone numbers are page
numbers. Appendices E and F (Python documentation) are in the file but irrelevant to the legal
analysis.

Course context: [[03 - School/Courses/Intellectual Property and Privacy/Intellectual Property and Privacy README|Intellectual Property and Privacy README]]

---

1 Executive Summary

Business Monitor aims to help organisations improve learning effectiveness by providing a unified,
evidence-based evaluation approach. Many organisations currently lack an integrated chain from L1
experience to L4 results, and KPI definitions vary widely across programs. This project develops a
Minimum Viable Product of the Learning Benchmarking Tool (LBT), demonstrating how such an end-to-end
evaluation chain can be standardized and technically implemented.

The MVP is built on a fully synthetic organisational dataset that reflects realistic program- and
participant-level structures. A standardized KPI framework is introduced, aligned with the four Kirkpatrick
levels across Experience, Learning, Behaviour, and Results, following established evaluation theory
(Kirkpatrick 1998; Kirkpatrick and Kirkpatrick 2006). These KPIs are integrated into an interactive Power BI
environment, covering the Learn, Perform, and Return dashboards.

Figure 1: Learning Benchmarking Tool overview dashboard

The analytical layer includes a correlation module to identify structural relationships across the evaluation
chain, and an exploratory prediction model that translates KPI changes into directional scenario outcomes.
The model is not intended for causal inference, but it demonstrates feasibility for scenario-based
benchmarking once real-world organisational data become available.

Initial findings from the synthetic dataset show patterns consistent with established learning theories,
including positive associations between experience, confidence, behaviour change, and downstream
results. These relationships indicate how an integrated evaluation pipeline can support HR and L&D
stakeholders in making more evidence-informed decisions.

4

Figure 2: Prediction Model Tab

The MVP remains constrained by the use of synthetic data, limited generalizability, and the exploratory
nature of the prediction model. However, it establishes a GDPR-safe technical foundation and a scalable
KPI structure that can directly ingest organisational data. Future development will prioritize partner pilots,
benchmarking logic, more robust modelling, and enhancements to the

2 Market Opportunity, Value Proposition, and Business Model

2.1 Market Opportunity

Organizations invest substantial resources in learning and development, yet often lack credible,
comparable, and longitudinal insight into the effectiveness of these investments. Multiple studies show
that internal evaluations remain dominated by isolated satisfaction measures and completion rates, which
offer limited value for strategic decision-making or demonstrating organizational impact (Personnel and
Development 2023; Innovate HR 2022). At the same time, organizations increasingly seek evidence-based
approaches to learning effectiveness, but available external benchmarks are fragmented, proprietary, or
methodologically opaque, reducing trust and practical usability for senior leadership and HR
decision-makers (Sopact 2023).

Discussions with Business Monitor and an analysis of their existing role as an independent data
intermediary indicate a clear opportunity for a standardized learning benchmarking service. Such a service
should translate evaluation data into transparent and reproducible KPIs, enable cross-program and
cross-organization comparisons, and comply with privacy and confidentiality requirements. These needs
align with broader developments in HR analytics, where integrated data environments and structured
benchmarking are increasingly recognized as foundational capabilities for improving organizational
decision-making [ Marler and Boudreau (2017); Bersin (2020)].

5

Table 1: Market Opportunity and Concept Selection Overview

Market
Opportunities

Enable
organizations to
compare the ROI
and effectiveness of
their learning
programs against
industry
benchmarks. This
helps identify
strengths, gaps, and
best practices, and
provides evidence
for continuous
improvement and
stronger
justification for
future investments.

Venture Core Abilities

Customers

• Multi-source data

• Corporate HR and L&D

integration (HR systems,
training performance data,
industry benchmarks).

• Advanced analytics and
statistical modeling (to
compare program outcomes
with peers).

• Data visualization and

dashboards (benchmark
comparisons for different
stakeholders).

• Secure data management
and compliance (to handle
sensitive HR and training
data responsibly).

departments, to evaluate
how their training outcomes
compare with industry
averages and competitors.

• Executive leadership (CFOs,

CLOs, Boards), to use
benchmarking data for
strategic decisions and
budget allocation.

• Consulting firms (HR and
L&D consultancies), to
provide clients with
benchmarking insights as
part of advisory services.

• Training providers (corporate

universities, external
vendors), to demonstrate
the added value of their
programs against market
benchmarks.

The Learning Benchmarking Tool is positioned to fill this gap by operationalizing Kirkpatrick’s model into a
structured benchmarking environment, enabling a consistent and interpretable way to assess how learning
activities translate into behavioral change and organizational outcomes.

2.2 Value Proposition

The Learning Benchmarking Tool provides HR and L&D professionals with a structured way to understand
how their training programs perform relative to anonymized benchmarks and to identify concrete levers
for improvement. The core of the value proposition is threefold.

First, the tool standardizes evaluation metrics across programs and organizations by applying a consistent

6

operationalization of the Kirkpatrick levels. This replaces the fragmented and heterogeneous evaluation
approaches that dominate current practice, where organizations often rely on isolated satisfaction items or
completion rates that lack strategic value (Personnel and Development 2023; Innovate HR 2022).

Second, the tool leverages Business Monitor’s neutral position and technical infrastructure to aggregate
and anonymize learning evaluation data. This reduces the methodological and compliance burden for
individual organizations while ensuring that cross-organizational comparisons remain secure, comparable,
and GDPR-compliant. The approach addresses a major pain point in the L&D domain: the lack of
trustworthy external benchmarks and the difficulty of comparing outcomes across heterogeneous datasets
(Sopact 2023).

Third, the tool translates complex analytical structures, such as driver analyses, chain-drop diagnostics,
scenario simulations, and correlation patterns, into interpretable visualizations and narratives. These
outputs help HR and L&D professionals justify learning investments, communicate findings to senior
leadership, and target opportunities for improvement with confidence. The emphasis on actionable,
evidence-based insight aligns with broader sector developments advocating for more rigorous approaches
to measuring learning effectiveness and business impact.

Figure 3: Value Proposition Canvas for the Learning Benchmarking Tool

2.3 Business Model

The business model builds on Business Monitor’s role as a neutral hub for cross-organizational data
collaboration. Participating organizations contribute anonymized evaluation data under clear governance
agreements, and in return gain access to structured benchmarks that help interpret the effectiveness of
their learning programs in a broader context.

7

Figure 4: Business Model Canvas for the Learning Benchmarking Tool

This model relies on a straightforward exchange. Organizations receive standardized insights that would be
difficult to generate on their own, while Business Monitor curates the underlying dataset and maintains
the analytical environment. The approach is supported by established findings in HR analytics, which
highlight the growing importance of integrated data infrastructures, comparable metrics, and accessible
analytical tools for decision-making (Marler and Boudreau 2017; Bersin 2020).

The revenue structure follows a subscription model that grants access to the benchmarking dashboard.
Additional services, such as interpretation support or workshops, can be offered to organizations seeking
deeper contextualization of their results. This creates a sustainable path in which value increases as more
organizations contribute data, and where Business Monitor can gradually expand the analytical depth as
the benchmark dataset grows. The model fits the organization’s strategic position and meets the practical
realities of data availability and GDPR compliance (Standardization 2022).

2.4 Validation of Assumptions

Two related solution directions were examined at the start of the project: a Training Investment
Optimization Advisor and the Learning Benchmarking Tool. A structured opportunity assessment was
conducted to evaluate both concepts across criteria such as data readiness, implementation feasibility,
customer validation potential, and compliance risk.

8

Figure 5: Opportunity Assessment: Benchmarking Tool vs Optimization Advisor

The assessment showed a clear divergence in feasibility. The Optimization Advisor requires mature,
integrated HR and financial datasets, consistent identifiers, and validated links between learning and
business performance. These conditions are not currently met and introduce substantial privacy and
methodological challenges, making the concept difficult to validate in a near-term prototype. In contrast,
the Learning Benchmarking Tool aligns well with the available survey and program datasets, requires fewer
assumptions, and demonstrates a clearer short-term value for HR and L&D professionals.

Interviews and conversations with Business Monitor confirmed that benchmarking is a recognizable and
recurring need. Many organizations indicate uncertainty about how their training performance compares
to peers and lack the means to generate reliable external reference points. External studies reinforce this
challenge and highlight the need for comparable, trustworthy learning evaluation practices (Personnel and
Development 2023; Innovate HR 2022; Sopact 2023)

Two refinements emerged from discussions with Business Monitor and academic supervisors. The first is
the decision to align the conceptual backbone with the Kirkpatrick model, which improves interpretability
and provides a stable structure for comparing programs across organizations. The second is the deliberate
use of a synthetic dataset to validate the analytical workflow, ensuring that the full process can be tested
without exposing sensitive organizational information.

9

2.5 Mapping to the Moonshot Quadrant

The opportunity assessment also relates to the Market Opportunity Navigator’s “Moonshot” quadrant.
Concepts that require extensive data maturity, high analytical complexity, and long development cycles
typically fall into this category. The Optimization Advisor maps directly to this quadrant because it relies on
financial impact modeling and multi-source HR integration that exceed current data readiness. This places
it in a long-term innovation space that may become viable once data maturity increases.

The Learning Benchmarking Tool avoids this position. Its data requirements match the existing Business
Monitor datasets, and its analytical components can be demonstrated with synthetically generated inputs.
As a result, it occupies a more feasible quadrant where evidence can be generated within the timeframe
and constraints of the DIiA project. This explains why the benchmarking concept progresses as the
validated direction while the Optimization Advisor remains a long-term strategic possibility.

3 Data

3.1 Data Description

The analytical foundation of the Learning Benchmarking Tool is the synthetic dataset LPBT_synthetic_v3,
which consists of program-level and participant-level data, complemented by dimensional reference
tables. We used the received data solely to establish the contextual boundaries of the synthetic dataset,
such as defining realistic minimum and maximum values. All structures are designed to be
schema-compatible with future real data while avoiding disclosure risks. A detailed description of the
schema is provided in Appendix A.

At program level, the synthetic_programs table contains one record per learning program, including
variables describing training type, delivery format, duration, target group, and design quality, as well as
process indicators such as invitations, attendance, and completion. It also stores outcome measures
aligned with the four Kirkpatrick levels, including satisfaction, perceived relevance, knowledge gain, skill
application, and several proxies for business impact such as Net Impact Score, productivity-related
changes, and retention-related indicators.

At participant level, the synthetic_participants table captures contextual characteristics, link keys to
program records, and items such as manager support and investment-related fields that can be aggregated
into KPIs. Dimensional tables provide standardized categories for sectors, locations, and course types.
Together, these structures support flexible filtering and aggregation in the dashboard.

10

Figure 6: High-level schema of the LPBT_synthetic_v3 dataset

A complete variable-level description of all fields used in the dataset is provided in Appendix C (Data
Dictionary).

3.2 KPI Mapping and Analytical Framework

The KPI framework translates Kirkpatrick’s four evaluation levels into a set of actionable indicators that can
be calculated consistently across programs. The framework provides a transparent structure for linking
survey items, derived ratios, and analytical constructs to their corresponding evaluation levels, ensuring
comparability across organizations. The full mapping used in the Power BI implementation is documented
in Appendix B.

At Reaction level (L1), the indicators summarize participants’ immediate experiences with the learning
intervention, including satisfaction, trainer quality, goal clarity, and perceived program coherence. These
indicators reflect the established first level of the Kirkpatrick model, which traditionally captures how
participants respond to the training environment (Kirkpatrick and Kirkpatrick 2009).

At Learning level (L2), the KPIs capture knowledge acquisition, confidence, relevance, and motivation to
apply learned skills. This aligns with research emphasizing the importance of perceived relevance and
cognitive gains in predicting later stages of transfer (Thalheimer 2018).

At Behavior level (L3), indicators focus on real-world application and the presence of transfer-supporting
conditions. Items such as alignment with job tasks, supervisory support, and follow-up coaching reflect

11

well-established determinants of transfer in the behavioral domain (Baldwin and Ford 1988; Saks and
Burke 2012).

At Results level (L4), the KPIs approximate organizational outcomes, including Net Impact Score,
ROI-related ratios, productivity impact, and changes in retention. These measures reflect established
models for evaluating the organizational returns of training (Phillips 2016; Alvarez, Salas, and Garofano
2004).

The mapping ensures that each indicator used in the dashboards and prediction model has a clearly
defined position within the evaluation structure. This transparency supports an academic evaluation
mindset and enables reproducible benchmarking across organizations, which is essential for building
cumulative evidence in learning analytics.

3.3 Data Preparation and Modeling Approach

Business understanding and data understanding informed the design of the schema and distributions. In
the data preparation phase, synthetic records were generated with plausibility constraints, such as valid
Likert scales, consistent attendance and completion relationships, and realistic ranges for costs and
benefits. Dependencies between design variables and outcomes were embedded to obtain meaningful
structure for analysis, while preserving sufficient randomness to avoid deterministic patterns.

For the analytical components in Power BI, the following methods were applied:

Table 2: Overview of analytical components implemented in the Learning Benchmarking Tool.

Analyti-
cal
Compo-
nent

Descrip-
tive
Bench-
marking

Objective

Summarize
performance per
KPI and compare
against synthetic
or peer
benchmarks.

Methodological
Approach

Output in
Dashboard

KPI cards, gauges,
and trend visuals.

DAX measures in
Power BI
aggregating
program- and
participant-level
data.

Interpretation

Identifies
strengths and
weaknesses per
training program
relative to
benchmarks.

12

Analyti-
cal
Compo-
nent

Inter-
Level
Correla-
tion
Analysis

Driver
Impor-
tance
Modeling

Objective

Quantify
relationships
between
Kirkpatrick levels
(Reaction →
Learning →
Behavior →
Results).
Identify key design
and context
variables
explaining KPI
variance.

Pearson or
Spearman
correlation
computed via
embedded Python
script.

Random Forest
and Gradient
Boosting models
(scikit-learn)
executed in Power
BI Python visual.

Methodological
Approach

Output in
Dashboard

Correlation
heatmap and
Chain Drop
visualization.

Interpretation

Shows where
effectiveness is
lost or maintained
between
evaluation stages.

Bar chart of
feature
importances (top 5
drivers).

Highlights which
factors (e.g.,
design quality,
trainer quality)
most influence
outcomes.

Inter-level correlations between the four indices are calculated to explore how value propagates from
Reaction to Results. A Chain Drop indicator quantifies relative decreases in effectiveness between levels.
For the Prediction Model tab, embedded Python scripts train tree-based models (Random Forest and
Gradient Boosting) to estimate the relative importance of design and context features in explaining
variation in selected KPIs. Modeling is intentionally explanatory rather than predictive: the focus is on
interpretability and managerial insight, not on forecasting.

3.3.1 Benchmark readiness

To ensure that benchmarking outputs are based on sufficiently complete and reliable inputs, each program
record is evaluated against a minimal set of data-quality criteria. The resulting variable benchmark_ready
equals 1 only when all of the following conditions are met:

• at least eight participants are registered
• attendance rate is at least sixty percent and completion at least fifty percent
• key Learn and Perform KPIs are available
• training type and delivery format are specified

This flag enables PowerBI to filter out incomplete or low-quality records in the dashboards and prevents

13

programs with insufficient data from influencing benchmark distributions. Applying this rule ensures
comparability across programs and supports consistent interpretation of benchmarked KPI values.

3.4 KPI Structure and Formulas

To operationalize the Kirkpatrick evaluation framework within the Learning Program Benchmarking Tool, a
structured KPI table was designed. Each indicator links conceptual evaluation dimensions (Reaction,
Learning, Behavior, and Results) with measurable data fields and consistent formulas to ensure
comparability across programs.

The table below summarizes the active KPIs used in the current version of the dashboard – full KPI table is
available in Appendix D. They represent a mix of quantitative and comparative indicators covering baseline
inputs, intermediate outcomes, and organizational results.

Table 3: Overview of KPIs processed in the Learning Benchmarking Tool.

KPI

Description

participa-
tion_rate_kpi

applicabil-
ity_kpi
behav-
ior_change_kpi
follow-
up_coach-
ing_kpi
job_align-
ment_kpi

profes-
sional_rele-
vance_kpi
skill_applica-
tion_rate_kpi

Share of invitees that
enrolled/attended the
program.
Perceived applicability of the
training to the job.
Self- or manager-rated
behavioral change.
Share of participants
receiving post-training
coaching.
Degree to which training
content aligns with current
role/tasks.
Perceived relevance of the
program for professional
growth.
Share of participants
applying learned skills at
work.

Kirkpatrick
Level

Baseline

Behavior

Behavior

Behavior

Behavior

Behavior

Behavior

Formula

(participants_count ÷
invitations) × 100

average(applicability_likert ÷
5) × 100
average(behav-
ior_change_likert)
(follow_up_coaching_likert ÷
participants) × 100

average(job_alignment_likert
÷ 5) × 100

average(professional_rele-
vance_likert ÷ 5) × 100

(participants_apply_skills ÷
participants_count) × 100

14

KPI

Description

Kirkpatrick
Level

Formula

confi-
dence_kpi

knowl-
edge_gain_kpi

learning_en-
gagement_kpi

learn-
ing_trans-
fer_readi-
ness_kpi
motiva-
tion_ap-
ply_kpi
goal_achieve-
ment_kpi
learner_satis-
faction_kpi
manager_sup-
port_kpi
program_co-
herence_kpi
trainer_effec-
tiveness_kpi
bench-
mark_posi-
tion_kpi
employee_en-
gagement_in-
dex_(δ)_kpi
learn-
ing_roi_kpi
learn-
ing_cost_ra-
tio_kpi

Average post-training
confidence in applying the
learned skills.
Relative improvement in
knowledge test scores.

Composite index from
participation + completion +
activity.
Readiness and perceived
ability to transfer learning to
the job.

Learning

AVERAGE(confidence_likert)

Learning

Learning

Learning

((post_test_score –
pre_test_score) ÷
pre_test_score) × 100
index(participation,
completion)

average(transfer_readi-
ness_likert ÷ 5) × 100

Motivation to apply learned
skills in practice.

Learning

average(motivation_ap-
ply_likert ÷ 5) × 100

Perceived achievement of
individual learning goals.
Overall satisfaction with the
learning experience.
Manager support influencing
transfer readiness.
Perceived coherence and
structure of the program.
Perceived effectiveness of
the trainer/facilitator.
Relative position compared
to external benchmark.

Reaction

Reaction

Reaction

Reaction

Reaction

Results

Change in employee
engagement related to
learning.
Estimated financial return on
learning investment.
Net investment share of HR
budget allocated to learning.

Results

Results

Results

average(goal_achieve-
ment_likert ÷ 5) × 100
average(satisfaction_likert ÷
5) × 100
average(manager_sup-
port_likert)
average(program_coher-
ence_likert ÷ 5) × 100
average(trainer_quality_lik-
ert ÷ 5) × 100
(organization_kpi_value ÷
benchmark_average) × 100

((engagement_after –
engagement_before) ÷
engagement_before) × 100
(total_benefit ÷ total_cost)

(Training Investment ÷ Total
HR Budget) × 100

15

KPI

Description

nps_satisfac-
tion_kpi

nps_experi-
ence_score

Net Promoter Score derived
from the balance of
promoters and detractors by
using the
nps_experience_score.
Composite experience score
reflecting perceived quality
of the learning intervention,
based on weighted
satisfaction, trainer quality,
relevance, coherence, and
job alignment.

productiv-
ity_im-
pact_kpi
promo-
tion_rate_kpi

retention_im-
prove-
ment_kpi
train-
ing_cost_ra-
tio_kpi

Relative productivity
improvement after the
program.
Share of participants
promoted or internally
transferred.
Relative improvement in
retention for the target
group.
Share of total HR budget
invested in training
programs, used as a
cost-efficiency indicator.

Kirkpatrick
Level

Results

Results

Results

Results

Results

Results

Formula

(NPS_Promoters_Pct –
NPS_Detractors_Pct) × 100

round(0.40 ×
satisfaction_likert + 0.20 ×
trainer_quality_likert + 0.20 ×
professional_relevance_likert
+ 0.10 ×
program_coherence_likert +
0.10 × job_alignment_likert,
0)
((output_after –
output_before) ÷
output_before) × 100
(promotions_or_transfers ÷
total_participants) × 100

((retention_after –
retention_before) ÷
retention_before) × 100
training_cost_ratio_kpi = 100
- DIVIDE ( [Training
Investment], [Total HR
Budget] ) * 1000

Note: Each formula corresponds to a calculated measure implemented within the Learning Benchmarking
Tool data model and Power BI dashboard.

This structure ensures consistency between survey data, calculated fields, and Power BI visualizations,
enabling transparent tracking of learning effectiveness across organizations.

16

3.5 Findings, Robustness, and Limitations

Within the synthetic dataset, several consistent patterns emerge that are in line with established
evaluation and transfer literature. Average scores across the four Kirkpatrick levels show a gradual decline
from Reaction and Learning towards Behavior and Results, and the chain-drop visual often indicates the
largest gap between Behavior (L3) and Results (L4). This pattern mirrors findings that positive training
experiences and self-reported learning do not automatically translate into measurable business outcomes,
and that the transfer stage is a frequent bottleneck in practice (Kirkpatrick and Kirkpatrick 2009; Baldwin
and Ford 1988).

The correlation heatmap further supports this interpretation. Reaction and Learning indicators, such as
satisfaction, trainer quality, relevance, and coherence, show moderate to strong intercorrelations and are
positively associated with application-related measures, which is consistent with models that emphasise
the importance of perceived relevance and instructional quality for later transfer (Thalheimer 2018). At
the same time, correlations between L1–L2 indicators and Results-level KPIs are noticeably weaker,
reflecting the well-documented attenuation between learner experience and organisational outcomes
(Alvarez, Salas, and Garofano 2004). This combination of moderate within-level correlations and weaker
links to L4 supports the plausibility of the synthetic structure.

Feature-importance analyses in the prediction model point to a similar story. Across different model runs
and filter selections, program design quality, trainer effectiveness, perceived relevance, job alignment, and
manager support frequently appear among the most influential predictors for impact-related KPIs. These
variables are also highlighted in transfer research as key conditions for successful application on the job,
which strengthens confidence that the modelling approach is picking up theoretically meaningful patterns
rather than arbitrary artefacts (Baldwin and Ford 1988; Saks and Burke 2012; Thalheimer 2018). The
scenario model builds on these drivers by identifying which of them offer the largest plausible
improvement margins within the observed data range.

Several internal checks were used to assess robustness within the synthetic setting. Correlation structures
were inspected using both Pearson and Spearman coefficients and with multiple threshold values; the
main clusters of strongly related indicators remain stable under these variations. In the prediction model,
Random Forest and Gradient Boosting regressors were compared, and although performance levels vary
across KPIs, the highest-ranked drivers are largely consistent across algorithms. Scenario outputs were
further constrained by observed value ranges, to avoid unrealistic extrapolations. Together, these checks
do not prove external validity, but they do suggest that the findings are internally coherent and resilient to
reasonable analytical choices.

At the same time, the use of fully synthetic data is a deliberate and important limitation. The distributions,
correlations, and effect sizes in the current dataset have been constructed to reflect plausible learning and
impact patterns, but they do not represent any specific organisation or sector. As a result, numerical results
in the dashboards and prediction model cannot be interpreted as empirical evidence about real-world

17

programs. The synthetic environment is suitable for validating the technical pipeline, the interpretability of
visualisations, and the overall analytical logic, yet external validity must be established in subsequent
pilots with real organisational data (Personnel and Development 2023; Innovate HR 2022; Sopact 2023).

A second limitation concerns the nature of the indicators themselves. Most KPIs are based on self-report
scales, which are subject to response bias, ceiling effects, and limited sensitivity to small changes.
ROI-related and productivity-oriented indicators are expressed as proxies rather than direct financials,
especially in the absence of integrated HR and financial systems. Moreover, all relationships uncovered in
the current analyses are associational. The models capture patterns that are consistent with theory, but
they do not establish causality and should not be interpreted as such.

In summary, the findings from the synthetic dataset provide a coherent and theory-consistent
demonstration of how the Learning Benchmarking Tool can structure, analyse, and visualise evaluation
data. The robustness checks show that the main patterns are stable across reasonable analytical
variations, while the limitations make clear that future work must focus on calibrating the framework with
real organisational datasets and on refining KPIs where necessary. This staged approach is appropriate for
an MVP in a sensitive HR analytics context: it ensures that the analytical design is sound before moving
towards real-world pilots and cross-organisational benchmarking.

4 Minimum Viable Product (MVP)

4.1 MVP Description

The Minimum Viable Product (MVP) of the Learning Benchmarking Tool is implemented as a Power BI
environment that integrates synthetic data, standardized KPIs, and analytical components into one
coherent user interface. It translates the Kirkpatrick evaluation model into five interactive tabs that allow
users to explore and interpret learning effectiveness across multiple dimensions.

4.2 Reaction Dashboard (L1)

The Reaction dashboard visualizes the immediate participant response to training programs.
It aggregates satisfaction scores, perceived goal achievement, program coherence, trainer effectiveness,
and perceived managerial support. Each KPI is displayed through interactive cards and gauges that
benchmark the program’s results against peer averages. Users can filter by sector, course type, delivery
format, and year to identify patterns in participant sentiment. A supplementary trend line allows
time-based exploration of how reaction indicators evolve across reporting periods. This dashboard helps
organizations understand how participants experience the training and whether the instructional design,
trainer quality, and managerial support align with learner expectations.

18

Figure 7: Reaction dashboard (L1)

4.3 Learning Dashboard (L2)

The Learning dashboard focuses on measurable learning outcomes such as knowledge gain, confidence,
and motivation to apply newly acquired skills. It combines quantitative indicators (e.g., pre- and post-test
scores) with perception-based measures (e.g., self-rated confidence, transfer readiness). All values are
normalized to ensure comparability across programs and industries. By comparing programs or cohorts,
HR and L&D managers can evaluate which instructional formats or topics produce the strongest learning
improvements.

19

Figure 8: Learning dashboard (L2)

4.4 Behavior Dashboard (L3)

The Behavior dashboard addresses the transfer of learning into the workplace. It aggregates data on skill
application, job alignment, professional relevance, and the availability of follow-up coaching. An index
visual summarizes the overall transfer strength, while secondary visuals reveal which contextual factors,
such as profesional relevance, skill rate and job alignment. Benchmark gauges indicate whether
participants are applying what they learned at a level consistent with comparable organizations. This tab
thereby connects the learning process with actual behavioral change, offering insight into the
sustainability of training outcomes.

20

Figure 9: Behavior dashboard (L3)

4.5 Results Dashboard (L4)

4.6 Results (L4)

The Results dashboard integrates the L4 indicators that reflect how learning interventions translate into
organisational outcomes. The page brings together the core business-related metrics from the synthetic
dataset, including productivity impact, retention improvement, promotion rate, training cost, the ROI ratio,
employee engagement, NPS, and the benchmark position. These indicators are presented through
gauge-style visuals that show both the absolute value and its position within the observed range, which
allows users to interpret each measure relative to the broader dataset.

A central element of this dashboard is the Net Impact Score, which provides a standardised way to assess
the overall value created at the Results level. The Net Impact Score follows the same logic as the Net
Promoter Score by calculating the difference between the percentage of high-impact responses and the
percentage of low-impact responses (Performitiv 2022) . High-impact responses represent the highest
category of the results scale, while low-impact responses fall within the lower range. The resulting value
indicates the net balance of impact. For example, when the score is 22, the share of participants reporting
high impact exceeds the share reporting low impact by twenty-two percentage points. The dashboard also
displays the underlying proportions of high-impact and low-impact responses, which helps users
understand how the score is composed.

21

In addition to the Net Impact Score, the Results dashboard provides trend lines that show how results
evolve over time and a heatmap that compares outcome patterns across branches and training types.
These visuals support benchmarking and reveal differences between domains, formats, or sectors.
Contextual metrics, such as participation rate, completion rate, attendance rate, total programs, and total
invitations, offer additional insight into the scale of learning activity within the filtered view.

Taken together, the Results dashboard enables decision-makers to evaluate the business impact of
learning interventions, compare performance across organisational segments, and identify where
improvements are likely to lead to meaningful gains.

Figure 10: Results Dashboard (L4)

4.7 Prediction Model Tab

4.7.1 Purpose and reading logic of the Prediction Model tab

The Prediction Model tab provides an exploratory decision aid that estimates how selected learning
indicators contribute to variation in a chosen KPI, and how targeted adjustments in related metrics could
influence expected performance. This part of the dashboard is designed to complement descriptive
insights by offering a scenario-based perspective on improvement potential, using a supervised learning
model trained on the filtered subset of the dataset.

Users begin by selecting a KPI of interest, together with optional filters for program type, seniority level,
delivery format, or cohort. The dashboard then trains a model on the active data slice and calculates a

22

baseline prediction for the selected KPI. This baseline reflects the expected value of the KPI given the
current characteristics of the filtered records. The user can specify a scenario adjustment to explore how
much improvement, or decline, they would like to investigate. The model evaluates this requested change
against what is realistically achievable within the range of the data.

4.7.2 Reading the Chain-Drop Plot

In addition to the driver and scenario visuals, the Prediction Model tab includes a chain-drop plot that
summarises the average scores across the four Kirkpatrick levels for the active filter selection. The plot
displays the values for Reaction (L1), Learning (L2), Behavior (L3), and Results (L4) as a horizontal
sequence, making it possible to observe at which stage value is gained or lost.

The chain-drop visual highlights how learning effectiveness progresses from initial participant experience
towards measurable business outcomes. A decline between consecutive levels indicates where
effectiveness is not fully carried through. For example, when Reaction and Learning scores are relatively
strong but Results lag behind, this suggests that positive experiences and knowledge gains do not fully
translate into operational or organisational improvement.

When the largest drop occurs between Behavior (L3) and Results (L4), the tool displays an interpretive
message indicating a bottleneck between application and business impact. This means that participants
report applying what they learned on the job, but the organisation does not yet observe corresponding
improvements in productivity, retention, engagement, or other business-level KPIs. The message provides
a concise interpretation of this pattern and helps users focus on structural or contextual factors that may
limit the translation of learning into measurable outcomes.

The percentage value shown next to the message represents the chain-drop magnitude between L3 and L4
for the selected filters. This helps users understand the extent of the gap and whether it is minor,
moderate, or substantial. The chain-drop visual therefore complements the prediction model by providing
a high-level diagnostic of where value is maintained or lost within the broader learning-to-impact
pathway.

4.7.3 Reading the correlation heatmap

The correlation heatmap shows the strongest relationships between KPIs within the currently filtered
subset of data. Instead of displaying the full matrix, the visual highlights only the top N indicators, where N
is controlled by the Top_x parameter in the dashboard. The selection is based on the highest absolute
off-diagonal correlations across all available KPIs. Users can switch between Pearson and Spearman
correlation, depending on whether they want to focus on linear or rank-based relationships. The applied
threshold further filters out weaker correlations so that only the most substantial patterns remain.

23

Each KPI label includes its Kirkpatrick level (L1–L4), which makes it immediately visible whether an
indicator belongs to Reaction, Learning, Behavior, or Results. The heatmap is ordered by level and lightly
segmented, so that users can see at a glance whether strong correlations occur within a single level or
span multiple levels in the learning pathway. For example, high correlations between L1 indicators such as
trainer effectiveness and L2 indicators such as confidence or learning engagement suggest that perceived
instructional quality is closely aligned with self-reported learning outcomes.

Only off-diagonal relationships are used to determine which KPIs enter the top N set; self-correlations of
1.00 are ignored in the selection and are not interpreted. In the heatmap itself, warmer colors indicate
positive associations and cooler colors indicate negative associations. Strong positive correlations imply
that higher values on one KPI tend to coincide with higher values on another, whereas negative
correlations indicate opposing movement.

By combining the correlation heatmap with the chain-drop visual and the driver-based prediction model,
users obtain a multi-perspective view of how learning value develops across the Kirkpatrick levels. The
heatmap acts as a structural diagnostic: it reveals which KPIs form tightly connected clusters, where links
between levels are strong or weak, and which indicators behave more independently within the synthetic
dataset. This structural insight complements scenario simulations by indicating where improvements in
one KPI are most likely to co-occur with changes in others.

4.7.4 Reading the line above the prediction plots

The line above the prediction plots summarises the key diagnostic values of the scenario simulation. The
scenario goal represents the improvement the user wants to explore, while the model-achievable
improvement shows how much of that goal can realistically be reached based on historical patterns and
the remaining variation in the dataset. The remaining gap is the difference between both values and
indicates how ambitious the scenario is relative to what the data supports.

The robust R² value reflects how well the model explains variation in the selected KPI. It is computed
through repeated testing on random subsamples and provides a more stable estimate than a single
train–test split. Values close to 1 indicate that the model captures most of the underlying structure. Values
near zero or negative point to weak patterns, in which case the scenario outputs should be interpreted
cautiously.

Next to the title, the dashboard also presents the Δ Total benefit, expressed in percentage points. This
value estimates how much the organisation’s expected business value changes when applying the model’s
recommended KPI adjustments, staying within the limits observed in the dataset. The colour of this label
indicates whether the expected effect is positive or negative, providing a direct visual cue for
decision-makers.

Together, these metrics provide a compact summary of how the selected scenario relates to the

24

underlying data, how much improvement can realistically be achieved, and how much confidence users
can place in the predictions generated by the model.

4.7.5 Reading the values in the driver and scenario plots

The first visual shows the relative influence of underlying dataset variables on the selected KPI. These
drivers represent the features that most strongly explain variation within the filtered population, rather
than causal factors. The bars help users understand which structural components of the learning
environment are most predictive within the model. The intention is to provide orientation about
underlying patterns, not direct recommendations.

The second visual shows the model-suggested numeric adjustments on related KPIs or numeric indicators,
after scaling them to the scenario goal and constraining them to the realistic ranges observed in the
dataset. For each indicator, the model:

1. tests a feasible step size based on its distribution,
2. estimates the marginal effect on the selected KPI,
3. determines the maximum realistic change within the observed minimum–maximum bounds,
4. and then scales this change proportionally to the user’s scenario goal.

The resulting bars display the scenario-scaled lift on the selected KPI and the corresponding change
applied to each driver. These values reflect where the model finds meaningful leverage within the available
data and where improvement is naturally limited because the dataset shows little or no variation.

4.7.6 Overall interpretation

Together, the prediction summaries, the feature influence plot, and the scenario lift simulation allow users
to explore different goals, compare model outputs across populations, and understand where meaningful
improvements are statistically plausible. The tab supports informed discussion about leverage points,
expected limits within the data, and the relative importance of different learning-related drivers, without
making causal claims.

25

Figure 11: Prediction Model Tab

A detailed technical description of the prediction model, including the full preprocessing pipeline, model
architecture, feature aggregation procedure, and scenario-simulation logic, is provided in the appendix.
This ensures transparency of the modelling steps while keeping the main report focused on the conceptual
design and interpretation of the results. Readers who wish to examine the underlying code or
implementation details can refer to Appendix E (Correlation Heatmap) and Appendix F (Dynamic KPI
Scenario Model).

4.7.7 Realistic User Scenarios

Users can explore a wide range of scenario adjustments in the Prediction Model tab. These scenarios allow
organizations to examine how targeted changes in performance indicators might influence outcomes such
as productivity impact, retention improvement, or ROI-related KPIs. The scenarios do not claim causal
effects, but they offer an exploratory way to understand which improvements are statistically plausible
within the structure of the synthetic dataset.

Typical examples of scenario adjustments include:

• Increase in revenue growth.

The most appropriate KPI for the revenue growth scenario is learning_roi_kpi. Within the current
dataset, learning ROI functions as the strongest available proxy for commercial value creation

26

because it directly reflects the balance between programme benefits and programme costs. Unlike
operational or behavioral indicators such as productivity_impact_kpi, learning ROI captures the
economic dimension of learning outcomes and therefore aligns more consistently with patterns in
total benefit. Using learning ROI as the lead KPI provides a more realistic and business-aligned basis
for modelling revenue-related improvements.

• Reduction in operational costs.

The most relevant KPI is training_cost_ratio_kpi, which captures the share of the HR budget
allocated to learning and reflects the effect of reduced operational or learning-related costs.
Training_roi_kpi can be used as an alternative when the focus is specifically on cost-benefit
relationships.

• Increase in customer satisfaction.

The most relevant KPI is nps_satisfaction_kpi where available.The productivity_impact_kpi serves as
the strongest proxy because improvements in service quality and client interaction are typically
reflected in productivity-based outcomes.

• Increase in Net Impact Score (NPS).

The most relevant KPI is nis_kpi, which directly captures the proportion of promoters and detractors
among participants.

• Increase in average tenure.

The most relevant KPI is retention_improvement_kpi, which shows how retention changes after the
learning intervention relative to the baseline.

• Reduction in time-to-promotion.

The most relevant KPI is promotion_rate_kpi, which reflects internal mobility and provides the most
appropriate approximation for shorter promotion cycles.

In the Prediction Model tab, the user begins by selecting the KPI that corresponds to the intended
scenario. Filters for training type, sector, seniority level, delivery format, and year can be applied to focus
the analysis on a specific subset of programs. The user then enters a scenario goal, which specifies the
magnitude of the improvement or decline they want to explore. The model evaluates this requested goal
in relation to the range of values and structural relationships observed in the filtered dataset.

4.8 User Interaction and Consistency

Across all tabs, the MVP provides a harmonized filter set, shared color palette, and standardized layout to
ensure usability and comparability. Interactive slicers for year, training type, delivery format, sector, and
location allow multi-dimensional exploration without breaking the analytical logic. Each visualization is
accompanied by concise interpretive text designed for HR and L&D stakeholders, supporting transparent

27

and evidence-based decision-making.

In summary, the MVP demonstrates how synthetic data, standardized KPIs, and interpretable analytics can
be combined into a functional proof of concept for benchmarking learning effectiveness within the
Kirkpatrick framework.

4.9 Methods and Implementation

The MVP is implemented using only technologies that are widely available in organizational contexts.
Power BI provides the data model, DAX calculations for aggregations, and interactive visuals. Embedded
Python scripts are used for correlation analysis and driver importance modeling, relying on standard
libraries and a simple, transparent pipeline. All synthetic data required by these components are loaded
from LPBT_synthetic_v3, ensuring reproducibility.

The dashboards share a harmonized filter set, including training type, format, sector, location, and year,
which allows users to conduct targeted comparisons while maintaining consistency. Each visualization is
accompanied by concise explanatory text to support interpretation, in line with the evaluation criteria for
clarity and actionability.

4.10 Completeness and Future Evolution

The current MVP delivers a coherent and functional demonstration of the Learning Benchmarking Tool. It
shows that a Kirkpatrick-based framework can be operationalized into measurable KPIs, that synthetic data
can be used to design and validate analytical components, and that structured visualizations can support
interpretability for both technical and non-technical users. The prediction model, correlation structures,
chain-drop analysis, and driver insights together form a consistent analytical pipeline that illustrates how
learning evaluation data can be transformed into comparative insights. These elements collectively fulfill
the core objectives defined with Business Monitor at the start of the project.

At this stage, the MVP is technically complete in the sense that it demonstrates the end-to-end workflow:
KPI mapping, data preprocessing, analytical modelling, visualization, and scenario exploration. The
architecture is deliberately modular, which makes it easier to adapt individual components as real
evaluation data becomes available. The use of synthetic data has been essential in this phase, as it allows
verification of the analytical logic without exposing confidential information or relying on datasets that
may not yet meet the necessary quality thresholds. This approach aligns with common recommendations
in HR analytics, where synthetic environments are used to reduce compliance risks and to validate
methodological choices before real data is introduced (Standardization 2022; Marler and Boudreau
2017).

However, the MVP does not yet serve as a final benchmarking product. Several steps are needed before

28

the tool can be deployed as a reliable service within Business Monitor’s ecosystem. The most important
next phase is piloting with real organizational data under strict GDPR-governed agreements. Such pilots
will provide empirical grounding for the KPIs, reveal where the synthetic assumptions need refinement,
and help determine which analytical outputs resonate most with HR and L&D stakeholders. This phase will
also help assess the variation needed in sector-specific or program-specific benchmarks, since synthetic
data cannot fully replicate the heterogeneity of real learning contexts.

A second development area concerns the refinement and potential expansion of KPIs. Although the
current mapping covers all Kirkpatrick levels, real-world data may suggest that some indicators require
recalibration or that additional measures are needed to capture nuances in learning application or
organizational outcomes. For example, job alignment or professional relevance may behave differently
across sectors, and ROI proxies may need adjustment once linked to real financial processes. The model
architecture already anticipates such adjustments, since KPIs are defined in a way that allows transparent
modification.

A third focus area is the user experience. While the current interface demonstrates how insights can be
visualized, future development should evaluate how HR and L&D professionals interpret the outputs,
which insights they find most valuable, and where additional explanation or guidance is needed. The
driver plot, scenario model, and chain-drop interpretation could be expanded with contextual tooltips,
interpretive narratives, or interactive benchmarking comparisons to help users navigate the dashboard
intuitively.

Looking ahead, the evolution of the product can be structured across three horizons. In the short term,
pilot collaborations with a small number of organizations should validate the analytical logic, evaluate the
usability of the dashboard, and test secure data submission pipelines. In the medium term, the benchmark
database can be expanded as additional organizations join, enabling more granular comparisons across
sectors and training types. This stage may also involve integration with HRIS or LMS systems to automate
data ingestion. In the long term, Business Monitor could develop a more advanced analytics layer that
incorporates machine learning-driven clustering of training profiles, sector-specific benchmark indices, or
prediction models calibrated on real longitudinal data. Such a roadmap aligns with the gradual scaling
envisioned in the Business Model and provides a sustainable path for transforming the MVP into a robust
benchmarking service.

In summary, the MVP establishes a solid foundation. It demonstrates feasibility, conceptual clarity, and
analytical coherence while remaining intentionally lightweight and adaptable. The next steps focus on
empirical validation, refinement of KPIs based on real-world patterns, and the progressive development of
a richer benchmarking ecosystem that supports evidence-based decision-making across participating
organizations.

29

5 Feasibility

5.1 GDPR and Privacy

Throughout the project, privacy and data protection considerations have been treated as binding
constraints rather than afterthoughts. The exclusive use of synthetic data in this proof of concept avoids
any processing of personal or client-confidential information. The intended future deployment model
assumes that participating organizations submit aggregated or pseudonymized data according to
predefined schemas, and that all outputs are reported at levels where re-identification is not reasonably
possible.

These design choices are aligned with principles underlying GDPR and with good practice guidance from
impact and evaluation communities (Sopact 2023). Detailed governance arrangements will be required
before real data are ingested.

5.2 Intellectual Property

The Learning Benchmarking Tool concept, including the KPI framework, synthetic dataset design, and
dashboard blueprint, has been developed within the DIiA context for Business Monitor. Ownership and
licensing arrangements should ensure that Business Monitor can further develop and commercialize the
tool, while acknowledging the contribution of the project team and academic partners.

5.3 Operational and Financial Considerations

From an operational perspective, the reliance on Power BI and standard Python libraries lowers adoption
barriers. Many potential clients already use similar environments, which reduces the need for bespoke
infrastructure. Financial feasibility depends primarily on the ability to recruit a sufficient number of
participating organizations to generate meaningful benchmarks and to support a subscription-based
model. The proof of concept indicates that the technical and methodological components do not pose
disproportionate costs.

30

6 Teamwork

6.1 Team Roles and Contributions

The project was executed by Team 5, bringing together complementary expertise in data engineering,
synthetic data generation, analytics, dashboard development, and business analysis. Responsibilities were
deliberately distributed to ensure a coherent end-to-end workflow.

Gilbert Laanen led the design, generation, and validation of the synthetic datasets and schema, and
implemented the Python-based analytical components, including the correlation heatmap and the
dynamic KPI scenario model. He also ensured the technical reproducibility and integration of the
modelling pipeline within Power BI.

Rick de Rijk focused on KPI operationalisation and DAX implementation, translating conceptual evaluation
constructs into measurable indicators. He contributed to the construction of the KPI framework and
supported dashboard integration across the four Kirkpatrick levels.

Stefan Vonk contributed to the predictive modelling design, review of analytical validity, and
interpretation of modelling outputs. He supported the alignment between methodological choices and
stakeholder needs, ensuring theoretical consistency across analytical components.

Tycho van Rooij supported the user experience design and the structuring of dashboard interactions. He
contributed to the layout, visual coherence, and interpretation text across the MVP, ensuring usability for
HR and L&D stakeholders.

Thom Verzantvoort contributed to business analysis, consolidation of stakeholder feedback, and
refinement of the value proposition and business model. He ensured alignment between technical
outputs and the organisational feasibility requirements of the intended service.

Together, the team delivered a technically coherent and conceptually grounded Minimum Viable Product
that integrates synthetic data, standardized KPIs, analytical modelling, and business insights into a unified
solution.

6.2 Collaboration Process

The team organized its work following the logic of CRISP-DM and iterative product development. Phases of
business understanding, data understanding, and design were followed by technical implementation and
evaluation cycles. Regular meetings with Business Monitor and academic supervisors ensured alignment
with expectations and allowed timely adjustments, such as transitioning from an earlier
Learn–Perform–Return framing to full adoption of the Kirkpatrick model.

31

6.3 Reflection on Team Dynamics

The collaborative process was characterized by shared ownership and continuous refinement. The
integration of methodological rigor, client relevance, and technical feasibility required coordinated effort,
which the team achieved through transparent task allocation, documentation, and version control. This
approach contributed to a coherent final deliverable.

7 Conclusion

The Learning Benchmarking Tool demonstrates that it is both technically feasible and conceptually sound
to design a benchmarking solution for learning programs that is grounded in Kirkpatrick’s four-level model
and aligned with contemporary expectations for evidence-based HR and L&D decision-making. The use of
synthetic data has enabled rigorous testing of schema design, KPI logic, and modeling components without
compromising privacy or confidentiality.

Figure 12: Conceptual representation of the Kirkpatrick levels integrated into the Learning Benchmarking

Tool.

The proof of concept confirms that standardized KPIs, clear mapping to evaluation levels, and
interpretable driver analyses can be combined into a practical decision-support environment for
organizations. At the same time, the findings underline that meaningful benchmarking requires consistent,
high-quality input data, thoughtful governance, and careful communication of limitations.

Future work should focus on staged pilots with real organizations, validation of KPI distributions against
empirical data, and incremental extension of the tool’s functionality where it adds explanatory power
without sacrificing transparency. By following this pathway, Business Monitor can position itself as a
credible provider of learning benchmarking insights that help organizations make better informed,
evidence-based investment decisions.

32

8 Appendix A – Synthetic Dataset Overview

This appendix documents the structure of the LPBT_synthetic_v3 dataset on which the proof of concept is
based. The dataset is designed so that it can be replaced by real organisational data without requiring
changes to the analytical logic, data model, or dashboard structures.

The dataset consists of seven tables that together form the modelling environment for the Learning
Benchmarking Tool. Each table has a defined analytical role, a clear granularity level, and a set of linking
variables that is used within Power BI.

Table 4: Overview of main tables in LPBT_synthetic_v3.

Granularity

Key Variables

Purpose

Relation to Other
Tables

Joined to syn-
thetic_participants
via record_id =
course_id; linked to
dim_course_type via
training_type_code.

Linked to
synthetic_programs
via course_id;
connected to
dim_branch and
dim_location via
branch_code and
location_code.

Linked to syn-
thetic_participants
via branch_code.

Contains program
design
characteristics,
operational
measures, and
outcome indicators
used across L1–L3
dashboards and the
Results dashboard.

Includes participant
responses,
behavioural
indicators,
contextual
information, and the
L4 impact rating
used to compute the
Net Impact Score.
Provides
standardised branch
labels for filtering
and sector-based
comparisons.

Table
Name

syn-
thetic_pro-
grams

Program-
level, one
row per
training
program

syn-
thetic_par-
ticipants

Participant-
level, many
rows per
program

record_id, Year,
training_type_code,
satisfaction_likert,
knowl-
edge_gain_pct,
apply_likert, partici-
pation_mandatory,
atten-
dance_rate_pct,
duration_hours,
total_cost
cursist_id, doeltaal,
course_id,
branch_code,
location_code, man-
ager_support_likert,
promotion_flag,
nis_overall_im-
pact_likert

dim_branch Sector or
industry
reference

branch_code,
branch_name

33

Table
Name

Granularity

Key Variables

Purpose

dim_loca-
tion

Geographic
reference

location_code,
location_name

dim_course_typeCourse-

type
reference

course_type_code,
training_type

kpi_map-
ping

KPI
metadata
table

kpi, description,
status, Kirkpatrick’s
level, type, unit,
domain, formula

data_dic-
tionary

Meta-level
documen-
tation

dataset, variable,
type, unit, purpose,
recommended_filter

Provides location
labels that support
geographic
comparisons and
segmentation.
Standardises
program categories
and supports
aggregation across
training types.
Defines the
calculation logic,
Kirkpatrick
classification, and
benchmark domain
for each KPI,
allowing consistent
categorisation within
Power BI.
Documents the
variables included in
the dataset and
clarifies their
analytical role,
supporting
reproducibility and
data governance.

Relation to Other
Tables

Linked to syn-
thetic_participants
via location_code.

Linked to
synthetic_programs
via
training_type_code.

Used as a metadata
layer for dynamic KPI
grouping and
reporting.

Documentation
table for analysts
and implementers.

The full technical specification, including all variables and field definitions, is maintained in the project files
and can be reused as a template for future data collection and integration.

34

9 Appendix B – KPI Mapping to Kirkpatrick Levels

Appendix B provides the detailed mapping of all KPIs used in the dashboards and prediction model to the
four Kirkpatrick levels. For each KPI, it records the definition, formula, source variables, and intended
interpretation in the context of benchmarking.

Table 5: Overview of KPI Mapping to Kirkpatrick Levels.

Kirk-
patrick
Level

Reac-
tion
(L1)
Learn-
ing (L2)
Behav-
ior (L3)
Results
(L4)

Focus

Example KPIs

Experience and
satisfaction

Satisfaction, Trainer Effectiveness, Goal Achievement, Program
Coherence, Manager Support

Knowledge and
confidence
Application and
transfer
Organizational
and financial
impact

Knowledge Gain, Motivation Apply, Confidence, Learning
Transfer Readiness, Learning Engagement
Skill Rate, Applicability, Job Alignment, Follow-up Coaching,
Professional Relevance
ROI Ratio, NIS, NPS, Productivity Impact, Retention
Improvement, Employee Engagement, Benchmark Position

This mapping ensures methodological transparency and supports consistent implementation when real
data are introduced.

35

10 Appendix C – Data Dictionary

Appendix C contains the complete data dictionary for the synthetic datasets, including variable names,
descriptions, datatypes, and units. It is derived from the Synthetic Data Generation documentation and
the LPBT_synthetic_v3 workbook.

Table 6: Overview of Data Dictionary.

Dataset

Variable

Type

Purpose

record_id

integer

Unique identifier to join, audit, and
de-duplicate records across sheets.

Filter

No

syn-
thetic_pro-
grams
syn-
thetic_pro-
grams
syn-
thetic_pro-
grams
syn-
thetic_pro-
grams
syn-
thetic_pro-
grams
syn-
thetic_pro-
grams
syn-
thetic_pro-
grams
syn-
thetic_pro-
grams

syn-
thetic_pro-
grams
syn-
thetic_pro-
grams

year

integer

The year in which the learning is provided

Yes

train-
ing_type_code

string

Standardized code to group courses for
reporting and benchmarking by program type.

Yes

learn-
ing_ob-
jectives
deliv-
ery_for-
mat
dura-
tion_hours

string

string

float

float

float

de-
sign_qual-
ity_index
trainer_to_par-
tici-
pant_ra-
tio
invita-
tions

integer

Captures expected outcomes to align evaluation
metrics with intended skills/behavior.

No

Classifies modality (online, classroom, blended)
to analyze effectiveness by format.

Measures training intensity to relate time
investment to outcomes.

Composite indicator of instructional design
quality to explain outcome variance.

Proxy for instructional attention, used to study
engagement and completion.

Denominator for participation metrics to assess
program reach.

Yes

Yes

No

No

No

Yes

integer

fol-
low_up_coach-
ing_likert

Flags after-care interventions to evaluate their
role in skill transfer.

36

Dataset

Variable

Type

Purpose

syn-
thetic_pro-
grams
syn-
thetic_pro-
grams
syn-
thetic_pro-
grams
syn-
thetic_pro-
grams

syn-
thetic_pro-
grams
syn-
thetic_pro-
grams
syn-
thetic_pro-
grams

syn-
thetic_pro-
grams
syn-
thetic_pro-
grams
syn-
thetic_pro-
grams
syn-
thetic_pro-
grams

senior-
ity_level

string

Segments learners by experience level to
control for baseline skill differences.

string

float

depart-
ment_func-
tion
opportu-
nity_to_ap-
ply_likert
partici-
pa-
tion_manda-
tory
float
atten-
dance_rate_pct

integer

Links programs to business units to enable
function-level impact analyses.

Measures real-world chances to use learned
skills, a key transfer enabler.

Distinguishes compliance-driven vs voluntary
learning to interpret satisfaction and
completion.

Share of sessions attended, used as an
engagement and data-quality control variable.

comple-
tion_rate_pct

float

Share finishing assessments or modules, core
indicator of program adherence.

base-
line_per-
for-
mance_in-
dex
reten-
tion_base-
line_pct
pre_con-
fidence

float

Pre-training performance proxy to control for
regression-to-the-mean and selection.

float

float

Pre-program retention level to benchmark
post-program changes.

Learner self-efficacy before training to estimate
growth relative to starting point.

post_con-
fidence

float

Learner self-efficacy after training to quantify
perceived gains.

float

self_as-
sessed_readi-
ness

Learner’s perceived job-readiness to predict
on-the-job application.

37

Filter

Yes

Yes

No

Yes

No

No

No

No

No

No

No

Dataset

Variable

Type

Purpose

syn-
thetic_pro-
grams
syn-
thetic_pro-
grams
syn-
thetic_pro-
grams
syn-
thetic_pro-
grams
syn-
thetic_pro-
grams
syn-
thetic_pro-
grams
syn-
thetic_pro-
grams
syn-
thetic_pro-
grams
syn-
thetic_pro-
grams
syn-
thetic_pro-
grams
syn-
thetic_pro-
grams
syn-
thetic_pro-
grams

pre_test_scorefloat

Objective knowledge/skill before training for
learning gain analyses.

post_test_scorefloat

Objective knowledge/skill after training to
compute learning gains.

integer

promo-
tions_or_trans-
fers
out-
put_be-
fore
out-
put_after

float

float

reten-
tion_be-
fore
reten-
tion_af-
ter
to-
tal_ben-
efit
to-
tal_cost

float

float

float

float

Career mobility events used as longer-term
outcome indicators.

Baseline productivity to compare pre/post
operational performance.

Post-training productivity to estimate
operational impact.

Employee retention before the program to
serve as baseline.

Employee retention after the program to detect
retention changes.

Monetized benefits used for ROI and payback
calculations.

All-in program costs to compute
cost-effectiveness and ROI.

organiza-
tion_kpi_value

float

Client’s own KPI value for context and
alignment with business targets.

bench-
mark_av-
erage
satisfac-
tion_lik-
ert

float

External or cross-program average to
benchmark performance levels.

integer

Learner satisfaction as a quality signal of the
learning experience.

38

Filter

No

No

No

No

No

No

No

No

Yes

No

No

No

Dataset

Variable

Type

Purpose

syn-
thetic_pro-
grams
syn-
thetic_pro-
grams
syn-
thetic_pro-
grams

syn-
thetic_pro-
grams

syn-
thetic_pro-
grams
syn-
thetic_pro-
grams

syn-
thetic_pro-
grams
syn-
thetic_pro-
grams
syn-
thetic_pro-
grams
syn-
thetic_par-
ticipants
syn-
thetic_par-
ticipants

float

integer

goal_achieve-
ment_lik-
ert
applica-
bility_lik-
ert
trans-
fer_readi-
ness_lik-
ert
profes-
sional_rel-
e-
vance_lik-
ert
trainer_qual-
ity_likert

float

float

float

Extent to which personal/program goals were
met to assess perceived effectiveness.

Perceived applicability on the job to predict
transfer and business impact.

Perceived readiness to apply skills, bridging
learning to behavior change.

Perceived relevance to the role to explain
motivation and usage.

Perceived trainer quality as a driver of
engagement and learning outcomes.

pro-
gram_co-
her-
ence_lik-
ert
motiva-
tion_ap-
ply_likert
job_align-
ment_lik-
ert
bench-
mark_ready

float

Perceived alignment and structure of content to
explain completion and satisfaction.

float

float

Learner motivation to use skills, a predictor of
real application.

Fit with job tasks to estimate likelihood of
sustained use and impact.

integer

Enables slicing or excluding non-ready records
in KPI calculations.

cursist_id

string

Join key to track multiple responses per learner
and deduplicate.

doeltaal

string

Used to analyze language-specific outcomes
and preferences.

39

Filter

No

No

No

No

No

No

No

No

Yes

No

Yes

Dataset

Variable

Type

Purpose

course_id string

Join key to link participant responses to
program-level data.

float

Input for NIS and cost-effectiveness analyses.

Yes

float

string

Denominator for NIS (investment share)
calculations.

Enables geography-based benchmarking and
logistics planning.

branch_codestring

Sector-level benchmarking and external
comparisons.

man-
ager_sup-
port_lik-
ert
promo-
tion_flag

float

Support provided by the trainee’s manager,
used as a contextual driver for satisfaction,
applicability, and transfer readiness.

integer

Provides information if the participant is
promoted due to the training.

train-
ing_in-
vestment
to-
tal_hr_bud-
get
loca-
tion_code

syn-
thetic_par-
ticipants
syn-
thetic_par-
ticipants
syn-
thetic_par-
ticipants
syn-
thetic_par-
ticipants
syn-
thetic_par-
ticipants
syn-
thetic_par-
ticipants

syn-
thetic_par-
ticipants
dim_course_type

string
course_type_code

string

string

train-
dim_course_type
ing_type
loca-
tion_code
loca-
tion_name

dim_lo-
cation
dim_lo-
cation
dim_branch branch_codestring
dim_branch branch_namestring

string

syn-
thetic_pro-
grams

engage-
ment_af-
ter

float

Surrogate key for course categories used in
joins.
Descriptive label for each training category.

Surrogate key for location table joins.

Descriptive location label used in dashboards
and reports.
Surrogate key for sector/branch joins.
Descriptive sector label used for benchmark
grouping.
Stores one record per learning program,
summarizing design, delivery, cost, and
outcome indicators across the four Kirkpatrick
levels.

40

Filter

Yes

No

Yes

Yes

No

Yes

Yes

Yes

Yes

Yes

Yes
Yes

no

Dataset

Variable

Type

Purpose

syn-
thetic_pro-
grams
syn-
thetic_pro-
grams

float

engage-
ment_be-
fore
behav-
ior_change_lik-
ert

float

Contains program-level variables that link
design and context factors to standardized KPIs
used in the dashboards.
Serves as a template for future real data,
capturing program attributes and outcomes for
benchmarking and KPI calculation.

Filter

no

no

The data dictionary is intended to function as a blueprint for organizations that wish to align their internal
evaluation instruments and databases with the Learning Benchmarking Tool, ensuring that future
benchmarking exercises can be conducted on a consistent and comparable basis.

41

11 Appendix D – KPI Table and Formulas

This appendix provides the complete overview of Key Performance Indicators (KPIs) implemented in the
Learning Program Benchmarking Tool (LPBT).

Each KPI operationalizes a specific construct within Kirkpatrick’s evaluation model (Reaction, Learning,
Behavior, or Results) and is linked to a formula that enables automated calculation in Power BI.
Conceptual KPIs represent additional indicators under consideration for future data collection rounds.

Table 7: Overview of KPI Table and Formulas.

Perceived
improvement in
collaboration.

concep-
tual

Behav-
ior

Likert
1–5

average(collaboration_im-
pact_likert)

KPI

Description

applica-
bility_kpi

behav-
ior_change_kpi

Perceived
applicability of the
training to the job.
Self- or
manager-rated
behavioral change.
Relative position
compared to
external benchmark.

bench-
mark_po-
si-
tion_kpi
collabo-
ra-
tion_im-
pact_kpi
confi-
dence_kpi

Average post-training
confidence in
applying learned
skills.
cost_per_course_type_kpi
Average cost per
participant per
course type.
Average cost per
participant per
location.

cost_per_lo-
ca-
tion_kpi

Status

active

active

Kirk-
patrick
Level

Behav-
ior

Behav-
ior

active

Results

Unit

Formula

Likert
1–5 →
%
Likert
1–5 →
%
%

average(applicability_likert
+ 5) × 100

average(behav-
ior_change_likert)

(organization_kpi_value ÷
benchmark_average) × 100

active

Learn-
ing

concep-
tual

Base-
line

concep-
tual

Base-
line

Likert
1–5 →
%

€ per
course
type
€ per
location

AVERAGE(confidence_lik-
ert)

(total_cost_course_type ÷
participants_course_type)

(total_cost_location ÷
participants_location)

42

KPI

Description

Status

Kirk-
patrick
Level

Unit

Formula

cost_per_par-
tici-
pant_kpi
cost_per_sec-
tor_kpi

cus-
tomer_sat-
isfac-
tion_kpi
digi-
tal_learn-
ing_readi-
ness_kpi
em-
ployee_en-
gage-
ment_Δ_kpi
error_re-
duc-
tion_/_qual-
ity_im-
prove-
ment
fol-
low_up_coach-
ing_kpi

goal_achieve-
ment_kpi

inter-
nal_mo-
bility_kpi

Average investment
per participant per
program.
Average cost per
participant per
sector.
Change in customer
satisfaction
post-training.

Readiness for digital
and blended
learning.

Change in employee
engagement related
to learning.

Reduction in errors
or quality
improvement after
learning.

Share of participants
receiving
post-training
coaching.
Perceived
achievement of
individual learning
goals.
Share of participants
moving to new
internal roles.

concep-
tual

Base-
line

concep-
tual

Base-
line

€ per
partici-
pant
€ per
sector

(total_program_cost ÷
participants)

(total_cost_sector ÷
participants_sector)

concep-
tual

concep-
tual

Results

Δ%

((csat_after – csat_before)
÷ csat_before) × 100

Cross

Index

index(access, skill, attitude)

active

Results

Δ%

concep-
tual

Results

%

((engagement_after –
engagement_before) ÷
engagement_before) × 100

((error_before –
error_after) ÷ error_before)
× 100

active

Behav-
ior

%

(follow_up_coaching_likert
÷ participants) × 100

active

Reac-
tion

Likert
1–5 →
%

average(goal_achieve-
ment_likert + 5) × 100

concep-
tual

Results

%

(internal_moves ÷
total_participants) × 100

43

KPI

Description

job_align-
ment_kpi

knowl-
edge_gain_kpi

knowl-
edge_re-
ten-
tion_test_kpi
learner_sat-
isfac-
tion_kpi
learn-
ing_cul-
ture_kpi

Degree to which
content aligns with
current tasks.
Relative
improvement in
knowledge test
scores.
Knowledge retained
4–6 weeks after
training.

Overall satisfaction
with the learning
experience.
Index of
organizational
learning culture and
support.
Composite index =
participation +
completion + activity.

learn-
ing_en-
gage-
ment_kpi
learn-
ing_rele-
vance_kpi
learn-
ing_roi_kpi

learn-
ing_trans-
fer_readi-
ness_kpi
man-
ager_ob-
serva-
tion_kpi

Estimated financial
return on learning
investment.
Readiness and
perceived ability to
transfer learning to
the job.
Manager-rated
performance
improvement.

Status

active

active

Kirk-
patrick
Level

Behav-
ior

Learn-
ing

Unit

Formula

Likert
1–5 →
%
%

average(job_alignment_lik-
ert + 5) × 100

((post_test_score –
pre_test_score) ÷
pre_test_score) × 100

concep-
tual

Learn-
ing

%

((delayed – pre) ÷ pre) ×
100

active

concep-
tual

Reac-
tion

Cross

Likert
1–5 →
%
Index

average(satisfaction_likert
+ 5) × 100

composite_index(support,
feedback, autonomy)

active

Learn-
ing

% of
max

index(participation,
completion)

active

Results

active

Learn-
ing

Likert
1–5 →
%
Ratio →
%

Likert
1–5 →
%

average(learning_rele-
vance_likert + 5) × 100

(total_benefit ÷ total_cost)

average(transfer_readi-
ness_likert + 5) × 100

concep-
tual

Behav-
ior

Likert
1–5

average(manager_observa-
tion_score)

44

Perceived relevance
of learning content.

concep-
tual

Reac-
tion

KPI

Description

Unit

Formula

man-
ager_sup-
port_kpi
motiva-
tion_ap-
ply_kpi
nis_kpi

nps_sat-
isfac-
tion_kpi

nps_ex-
peri-
ence_score

partici-
pa-
tion_rate_kpi
produc-
tiv-
ity_im-
pact_kpi
profes-
sional_rel-
e-
vance_kpi

Manager support
influencing transfer
readiness.
Motivation to apply
learned skills in
practice.
Net investment
share of HR budget
allocated to learning.
Net Promoter Score
derived from the
balance of promoters
and detractors.
Composite
experience score
reflecting perceived
quality of the
learning
intervention, based
on weighted
satisfaction, trainer
quality, relevance,
coherence, and job
alignment.
Share of invites that
attended the
program.
Relative productivity
improvement after
the program.

Perceived relevance
for professional
growth.

Status

active

active

Kirk-
patrick
Level

Reac-
tion

Learn-
ing

active

Results

Likert
1–5 →
%
Likert
1–5 →
%
%

active

Results

%

N/A

N/A

float

average(manager_sup-
port_likert)

average(motivation_ap-
ply_likert + 5) × 100

(Training Investment ÷ Total
HR Budget) × 100

(NPS_Promoters_Pct –
NPS_Detractors_Pct) × 100

round(0.40 ×
satisfaction_likert + 0.20 ×
trainer_quality_likert + 0.20
× professional_rele-
vance_likert + 0.10 ×
program_coherence_likert
+ 0.10 ×
job_alignment_likert, 0)

active

Base-
line

%

(participants ÷ invitations) ×
100

active

Results

%

((output_after –
output_before) ÷
output_before) × 100

active

Behav-
ior

Likert
1–5 →
%

average(professional_rele-
vance_likert + 5) × 100

45

Status

active

Kirk-
patrick
Level

Reac-
tion

concep-
tual

Reac-
tion

Unit

Formula

Likert
1–5 →
%

NPS

average(program_coher-
ence_likert + 5) × 100

(%Promoters –
%Detractors)

active

Results

%

(promotions_or_transfers ÷
total_participants) × 100

active

Results

%

Uplift in self-rated
confidence
(normalized).
Share of participants
applying new skills at
work.
Perceived
effectiveness of the
trainer or facilitator.

concep-
tual

Behav-
ior

active

active

Behav-
ior

Reac-
tion

per-
centage
points
%

Likert
1–5 →
%

((retention_after –
retention_before) ÷
retention_before) × 100

((PostConfidence Avg –
PreConfidence Avg) × 20)

(skill_application ÷
participants_count) × 100

average(trainer_quality_lik-
ert + 5) × 100

KPI

Description

pro-
gram_co-
her-
ence_kpi
pro-
gram_net_pro-
moter_score_kpi
promo-
tion_rate_kpi

Perceived coherence
and structure of the
program.

Likelihood to
recommend the
program (NPS).
Share of participants
promoted or
internally
transferred.
Retention after
training relative to
before.

reten-
tion_im-
prove-
ment_kpi
self_con-
fi-
dence_kpi
skill_ap-
plica-
tion_kpi
trainer_ef-
fective-
ness_kpi

Note:
This table serves as the foundation for Power BI calculations, ensuring that all metrics are consistently
computed and directly traceable to their underlying dataset fields. It also supports the transparency and
academic grounding of the LPBT framework, aligning data collection and visualization with the Kirkpatrick
model.

46

12 Appendix E – Technical Documentation of the Correlation Heatmap

This appendix documents the full analytical workflow of the correlation heatmap used in the Prediction
Model tab. It is aligned with the implementation in the Power BI Python visual and describes data
preparation, parameterisation, correlation computation, KPI selection logic, level ordering, and rendering
procedures. The method is designed to be deterministic, interpretable, and computationally lightweight to
ensure stable behaviour under dynamic filtering.

12.1 Overview of Script Functionality

The script performs seven core steps:

1. Receives a filtered dataset from Power BI containing all available KPI columns and user slicer

selections.

2. Reads user-defined parameters for correlation method, threshold, and the Top N selection.
3. Prepares and sanitises the KPI matrix by converting fields to numeric and removing columns without

variation.

4. Computes the correlation matrix using the chosen method.
5. Identifies the strongest correlations and selects the top N KPIs based on off-diagonal absolute

correlations.

6. Orders the selected KPIs by Kirkpatrick level and constructs readable labels for interpretation.
7. Renders an annotated heatmap with optional level separators for improved clustering visibility.

This workflow ensures that the heatmap remains both interpretable and consistent across dynamic filter
contexts.

12.2 Input Construction and Preprocessing

Power BI provides a pandas DataFrame containing all KPI variables, together with slicer outputs for:

• correlation method (Pearson, Spearman, or Kendall),
• absolute correlation threshold,
• the number of KPIs to highlight (Top N).

The script first identifies which of the predefined KPI columns are present in the filtered dataset. All
selected columns are coerced into numeric format, with non-convertible entries treated as missing values.
Columns with no variation, meaning they contain only a single unique value after filtering, are removed
because they cannot contribute meaningful correlation information.

47

If fewer than two KPI columns remain after variation filtering, the script displays an explanatory message
instead of computing correlations.

12.3 Parameterisation Through User Slicers

Three slicers govern the behaviour of the heatmap.

12.3.1 Correlation method

The user selects between Pearson, Spearman, or Kendall. The default is Pearson. This parameter directly
controls the statistical estimator applied within the pandas correlation function.

12.3.2 Threshold

The threshold determines which correlation coefficients are shown in the rendered heatmap. Only values
whose absolute magnitude is equal to or greater than the threshold are displayed. Weaker correlations are
masked to support interpretability.

12.3.3 Top N KPI selection

The script identifies, for each KPI, the strongest off-diagonal absolute correlation with any other KPI. These
maximum values are ranked, and the top N KPIs are selected. This selection determines the subset of the
matrix shown to the user. The default value is three.

Together, these parameters allow users to focus the heatmap on the strongest structural relationships
within the currently filtered subset.

12.4 Correlation Computation

After preprocessing, the script applies the user-selected correlation method to compute the matrix.
Self-correlations are explicitly removed from consideration by setting the diagonal to missing values. This
ensures that they cannot be mistakenly included in the Top N selection.

Although ROI-related fields are included in the initial computation, the script removes ROI from the
displayed matrix to avoid visual distortion and maintain consistency across different filtered views.

48

12.5 KPI Selection and Level Ordering

The script selects KPIs based on their strongest off-diagonal correlation. This process ensures that only
indicators participating in meaningful relationships are included in the heatmap.

Each KPI is mapped to its corresponding Kirkpatrick level (L1–L4). Once the Top N KPIs are selected, the
script orders them first by level rank and then alphabetically. This ordering produces natural clusters in the
heatmap, allowing users to recognise patterns within and across the four evaluation levels.

If the threshold and selection criteria together yield fewer than two KPIs, the script displays a message
indicating that there are not enough strong correlations to render a heatmap.

12.6 Label Construction and Readability

Raw KPI field names are cleaned to produce readable display labels. Underscores and suffixes are
removed, and names are converted to title case. Labels are then prefixed with their Kirkpatrick level, such
as L1 – Trainer Effectiveness or L3 – Job Alignment.

This improves the interpretability of the heatmap by making both the conceptual level and the substantive
meaning of each KPI immediately visible.

12.7 Heatmap Rendering

The heatmap is rendered using Seaborn with the following settings:

• a diverging colour palette reflecting the range from −1 to 1,
• two-decimal annotations for correlation values,
• threshold masking to hide weaker coefficients,
• rotated axis labels for readability,
• optional separator lines indicating transitions between Kirkpatrick levels.

The title includes the user-selected method, the applied threshold, and the Top N value. DPI settings are
adjusted to ensure legibility within the Power BI reporting canvas.

12.8 Interpretation and Analytical Role

The heatmap visualises correlation patterns present within the filtered dataset. These patterns represent
statistical associations, not causal relationships. Strong within-level correlations may indicate conceptual

49

coherence or shared measurement structure, whereas cross-level correlations provide insight into how
value flows between stages of the Kirkpatrick model.

The heatmap complements the chain-drop plot and the prediction model by offering a structural
diagnostic. It highlights where KPIs form clusters, where relationships weaken between levels, and which
indicators behave independently. This helps users interpret scenario simulations and driver importance
plots in a broader analytical context.

50

13 Appendix F – Technical Documentation of the Dynamic KPI

Scenario Model

This appendix documents the full technical workflow of the updated Python scenario engine used in the
Learning Benchmarking Tool. It includes preprocessing, model fitting, feature attribution, scenario
simulation, model-achievable improvement, and the estimation of Δ Total Benefit in percentage points.

13.1 Overview of Script Functionality

The script performs eight core steps:

1. Receives from Power BI a filtered dataset containing all drivers, KPI sub-measures, and user slicer

selections.

2. Extracts the selected KPI name and the user-defined KPI Adjustment (scenario_goal).
3. Preprocesses the data using numerical and categorical imputers and one-hot encoding.
4. Fits a regression model (Random Forest or Gradient Boosting) to predict the selected KPI.
5. Aggregates feature importances to driver-level influence scores.
6. Runs a model-based scenario simulation that tests realistic changes on KPI sub-measures and drivers

around a synthetic baseline.

7. Computes model-achievable improvement, remaining gap, and robust R².
8. Computes Δ Total Benefit based on the KPI change that the model actually realises in the scenario,

as visualised in the green bar chart.

The script is optimised for Power BI’s Python runtime: deterministic, lightweight, and without external
dependencies.

13.2 Input Construction and Preprocessing

Power BI provides a pandas DataFrame containing all KPI and driver variables, the selected KPI name, the
numeric scenario goal, and all filtered rows based on user slicers. The helper function pick_column
harmonises possible column-name variations. Rows missing the selected KPI are removed. Features
ending in _kpi are recognised as KPI sub-measures.

13.3 Preprocessing Pipeline

The script builds a scikit-learn pipeline containing:

51

• median imputation for numerical features
• mode imputation and one-hot encoding for categorical features
• a predictive model: RandomForestRegressor or GradientBoostingRegressor

This pipeline is trained on the full filtered dataset. No train–test split is used; reliability is measured via a
robust R² procedure.

13.4 Baseline Construction

A synthetic baseline observation is constructed by taking the median of each numerical feature and the
modal category for categorical features. This baseline is stable and representative under strong user
filtering. Passing this baseline through the pipeline yields a baseline prediction, noted as base_pred, for
the selected KPI.

13.5 Robust R² Estimation

To avoid instability caused by small filtered datasets, the script estimates reliability using a repeated
ShuffleSplit procedure. In each split:

1. The model is cloned.
2. It is trained on a random subset of rows.
3. Predictions are evaluated on the corresponding test subset.

The median R² across splits is returned as a robust measure of model reliability.

13.6 Feature Importance Aggregation (Blue Plot)

Tree-based models provide importances at the encoded feature level. For interpretability:

1. Each encoded one-hot-encoded feature is mapped back to its original variable.
2. Importances belonging to the same variable are summed.
3. Variables ending in _kpi are excluded for driver ranking.

The top five aggregated non-KPI drivers are displayed in the upper chart of the dashboard.

52

13.7 Scenario Simulation Procedure (Green Plot)

The scenario simulation identifies realistic adjustments to KPI sub-measures and driver features, and
evaluates them directly with the chosen model. This makes the green plot fully model-dependent.

For each numeric candidate feature:

1. A feasible adjustment step is computed via the step_for function, based on observed range,

variance, and feature type (Likert, percentage, duration, or general numeric). The step is additionally
capped at 30 percent of the observed range to avoid unrealistic adjustments.

2. The baseline value for this feature is taken from the synthetic baseline row. A tentative new value is
generated by adding the computed step and clamping it to the observed minimum and maximum.

3. A temporary scenario row is created by copying the baseline row and replacing only this feature with

the new value.

4. The fitted model predicts the KPI for baseline and adjusted rows. The achievable lift is defined as:

achievable_lift = model.predict(scenario_row) − model.predict(baseline_row)

5. Features that do not yield a positive KPI lift are discarded.

6. The remaining features each store both their capped feature delta and their achievable KPI lift.

7. The five strongest levers are selected.

These levers are then uniformly scaled so that their combined effect approaches the user’s KPI goal
without exceeding model-supported improvement. The scaled KPI lifts appear as green bars in the
dashboard’s lower chart.

13.8 Model-Achievable Improvement and Remaining Gap

After selecting and scaling levers, the script:

1. Copies the synthetic baseline.
2. Applies the scaled deltas for the selected levers.
3. Computes the scenario KPI prediction, scenario_pred.

The model-achievable improvement is:

model_achievable_improvement = scenario_pred − base_pred

53

The remaining gap is:

remaining_gap = |scenario_goal| − model_achievable_improvement

A positive remaining gap indicates that the user-defined KPI Adjustment exceeds what the model considers
empirically realistic.

13.9 Δ Total Benefit Computation

Δ Total Benefit is computed from the model-realised KPI lift, defined as the difference between the
scenario prediction and the baseline prediction (scenario_pred − base_pred) shown in the green plot. This
effective KPI delta replaces the user-provided KPI Adjustment. The mapping from KPI to total_benefit is
kept intentionally simple through a one-dimensional linear model to maintain transparency.

13.9.1 Step 1: Fit a one-dimensional model

On all filtered rows containing valid values for both variables, the script fits:

total_benefit = a × selected_kpi + b

This estimates the marginal effect of the selected KPI on total_benefit.

13.9.2 Step 2: Construct baseline and scenario KPI levels

• Baseline KPI = median(selected_kpi)
• Model-implied KPI change = effective_KPI_delta = scenario_pred − base_pred
• Scenario KPI = baseline_KPI + effective_KPI_delta, clamped to the observed range of the

selected KPI.

13.9.3 Step 3: Predict baseline and scenario total_benefit

Using the fitted linear model:

• baseline_benefit_pred = a × baseline_KPI + b
• scenario_benefit_pred = a × scenario_KPI + b

54

13.9.4 Step 4: Compute Δ Total Benefit

A robust percentage change is computed using:

• the median of total_benefit in the filtered dataset, and
• a stability constant ε equal to ten percent of that median.

The denominator is:

denominator = max(|baseline_benefit_pred|, median_total_benefit, �)

The percentage change is:

Δ Total Benefit = ((scenario_benefit_pred − baseline_benefit_pred) / denominator)
× 100

This formulation prevents extreme values when the baseline level of total_benefit is small and ensures
stable interpretation.

55

References

Alvarez, Karin, Eduardo Salas, and Christina Garofano. 2004. “An Integrated Model of Training Evaluation

and Effectiveness.” Human Resource Development Review 3 (4): 385–416.
https://www.researchgate.net/publication/232570004.

Baldwin, Timothy T., and J. Kevin Ford. 1988. “Transfer of Training: A Review and Directions for Future

Research.” Personnel Psychology 41 (1): 63–105.
https://www.researchgate.net/publication/228320877.
Bersin, Josh. 2020. “The People Analytics Maturity Model.”

https://joshbersin.com/2020/06/big-new-research-the-people-analytics-maturity-model/.

Innovate HR, Academy to. 2022. “HR Upskilling Report 2022.” AIHR.

https://www.aihr.com/resources/AIHR_HR_Upskilling_Report_2022.pdf.

Kirkpatrick, Donald L. 1998. Evaluating Training Programs: The Four Levels. San Francisco: Berrett-Koehler.
Kirkpatrick, Donald L., and James D. Kirkpatrick. 2006. Evaluating Training Programs: The Four Levels. 3rd

ed. San Francisco: Berrett-Koehler.

———. 2009. “The Kirkpatrick Model: Four Levels of Training Evaluation.”

https://www.kirkpatrickpartners.com/our-philosophy/the-kirkpatrick-model/.

Marler, Janet H., and John W. Boudreau. 2017. “An Evidence-Based Review of HR Analytics.” The

International Journal of Human Resource Management 28 (1): 3–26.
https://www.researchgate.net/publication/313842458_HR_Analytics.

Performitiv. 2022. “The Net Impact System: Optimizing Talent Development Through Continuous

Improvement.” https://performitiv.com/resources.

Personnel, Chartered Institute of, and Development. 2023. “Learning at Work 2023.” CIPD.

https://www.cipd.org/learning-at-work.

Phillips, Jack J. 2016. The ROI Methodology: Measuring and Improving Training Impact. ROI Institute.

https://roiinstitute.net/models/.

Saks, Alan M., and Lisa A. Burke. 2012. “An Examination of the Transfer of Training Model.” Human

Resource Development Quarterly 23 (1): 9–26. https://www.researchgate.net/publication/232496637.

Sopact. 2023. “How to Measure the Impact of a Program.”

https://www.sopact.com/perspectives/how-to-measure-impact-of-a-program.

Standardization, International Organization for. 2022. “ISO/IEC 27001:2022 Information Security,

Cybersecurity and Privacy Protection – Information Security Management Systems – Requirements.”
ISO. https://www.iso.org/standard/82875.html.

Thalheimer, Will. 2018. “The Learning-Transfer Evaluation Model (LTEM).”

https://www.worklearning.com/ltem/.

56

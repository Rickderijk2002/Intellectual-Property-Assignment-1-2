**Report on the Intervention Recommender for Heijmans Vastgoed**

## I. Brief statement of the relevant facts of the project

*(From the report)*

Heijmans Vastgoed, a Dutch property developer, uses well-being impact scans to identify opportunities in neighbourhoods. From these opportunities, interventions can be derived, such as what to change or what to build. The scans show opportunities but do not recommend which interventions fit. Our team developed an Intervention Recommender Tool to close this gap: a decision-support application that ranks well-being interventions for a neighbourhood using a transparent, weighted scoring model.[^1]

The tool is built on a structured database of interventions. Each intervention is classified by theme and category and scored on criteria such as impact, cost, effort, risk and feasibility. The database combines an initial collection of interventions with a list supplied by Heijmans. The initial scores were generated with generative AI and later evaluated and adjusted through a manual review by the team.[^2] The tool is intended to support consultants and project managers, not replace them, and to be scalable across projects.[^3]

This report assesses the project in an operational scenario. Where the points below go beyond the project report, they are assumptions made for this assignment:

1. The team acts as a Dutch data consultancy hired by Heijmans under a proposal that covers scope and fees and contains a confidentiality clause. It has no clause on who owns the intervention list, the combined database or the tool.
2. Heijmans’ intervention list and impact scans were built internally over several years through its own investment of time and expertise. They are not public and were shared with the team under the confidentiality clause only.
3. To fill gaps in the database, the consultancy wants to add interventions from a third-party online intervention library, collected by automated means. The library is free to use, but access requires registering an account and accepting terms of use. Those terms prohibit automated access and extraction of the contents. The consultancy also adds one open dataset published under a share-alike licence, which requires adapted versions to be shared under the same licence.
4. Heijmans wants to reuse the tool and the combined database across its own projects and to offer them commercially to third parties, such as housing corporations and municipalities. The consultancy wants to keep the right to reuse the generic parts of the tool for other clients.

[^1]: [@Heijmans2026, sections 1-3]
[^2]: [@Heijmans2026, sections 3.2-3.4 and 4]
[^3]: [@Heijmans2026, sections 2 and 7]

---



## Why this case fits the assignment

*Fit with the four required elements*


| Brief requires                                                                                               | What the case gives us                                                                                                                                                                                  |
| ------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| I. Facts: what data, from where, how, for what purpose                                                       | The description states the sources (Heijmans' list, the initial collection, third-party sources), the processing (classification, scoring, ranking) and the purpose (a reusable decision-support tool). |
| II. Protection: database rights, copyright, trade secrets                                                    | Each right has an object to analyse (see below).                                                                                                                                                        |
| III. Barrier and infringement: can IP stop the project, what is the risk, and contract breach if data mining | Assumptions 1, 3 and 4 create the barrier, the infringement risk and the data-mining question.                                                                                                          |
| IV. Advice: how to avoid or reduce the risks, and alternative sources                                        | Each risk has a realistic remedy and an alternative: a contract clause, licensed or open sources, separating client data, and a fallback.                                                               |


*One object per right*

- Database rights (copyright and sui generis): Heijmans' list and the combined database we build.
- Copyright: the scoring rationales, taxonomy mapping, code and tool. The AI-generated baseline adds an authorship question.
- Trade secrets: Heijmans' confidential list and impact scan (assumption 2), plus our own scoring logic.

*Why it scores on the rubric*

- Analysis and Assessment (9 points): the case has genuine tension, not one obvious answer.
  - The client's rights against our wish to reuse the tool.
  - Facts versus original selection (*BHB v William Hill*, *Football Dataco*).
  - Idea versus expression (*Infopaq*, *SAS*).
  - AI output without a human author.
  - The TDM exception versus contract terms and opt-outs.
- Advice (4 points): several options with trade-offs (licence, open data, rebuild, restrict to one client), so the advice can compare them.
- Language and structure (2 points): a compact case with four clear assumptions keeps the report focused.
- Bonus: real sources to cite are available for each issue.

*Why not a simpler case*

With synthetic data or an in-house tool, the answer could be "there is no IP risk" in a paragraph. The brief allows that outcome, but there would be less to analyse. The assumptions make the analysis rich enough for the word limit.

*Risks to manage*

- Do not overdo the assumptions. Four is enough.
- Keep them plausible: a client agreement that is silent on IP and a library that asks users to accept terms are common in practice.
- Where a part has no real risk, say so and explain why. The brief rewards that too.
- Do not state a legal rule that the course does not teach as if it were settled. EU law has no harmonised rule on who owns commissioned work, so say that the position is unclear without a contract.

---



## Analysis plan

*Three core issues (about 75% of the analysis)*


| Issue                               | Lecture content                                                                                                                       | Why it is central                                        |
| ----------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------- |
| Ownership and use of Heijmans' list | Database copyright (AOIC), sui generis right (creating versus obtaining, *BHB*), trade secret (Arts. 2 and 4 Trade Secrets Directive) | The contract is silent, so the answer is not obvious     |
| Scraping the library                | Restricted acts, Art. 4 DSM and the contractual opt-out, lawful access, *Ryanair*                                                     | The data-mining and contract analysis the brief requires |
| Commercial reuse                    | Ownership, trade secret limits, scraped content passed on to Heijmans, share-alike                                                    | The rights collide here, and the advice has real options |


*Word budget (about 2450 of 3000)*


| Section                        | Words | Focus                                                                                                 |
| ------------------------------ | ----- | ----------------------------------------------------------------------------------------------------- |
| I. Facts                       | ~300  | Short project description and the four assumptions                                                    |
| II. Protection                 | ~450  | Three paragraphs: Heijmans' list; the library and the combined database; the tool and the AI baseline |
| III. Barriers and infringement | ~1100 | Heijmans' list ~250, scraping ~400, reuse ~350, open data and AI ~100                                 |
| IV. Advice                     | ~600  | See below                                                                                             |


*Section II: what to cover*

- The database definition (Art. 1(2) DD) for each database.
- AOIC, and why a functional structure or standard removes originality.
- Sui generis: Art. 11 eligibility, substantial investment in obtaining, verifying or presenting, and the line between creating and obtaining data (*BHB*, *Fixtures Marketing*).
- The three trade secret requirements, using the confidentiality clause as the reasonable step.
- Plain copyright in the tool and rationales (idea versus expression), and no human author for the AI baseline.

*Section III: what to cover*

- Per source, in a fixed order: conclusion, act, right engaged, exception or licence, contract, residual risk.
- The restricted acts: reproduction and extraction (copying into the dataset), adaptation and re-utilisation (sharing the result).
- Art. 4 DSM: lawful access, the opt-out in the library's terms, and storage only as long as needed. One sentence on why Art. 3 does not help a consultancy.
- *Ryanair*: if the library is not protected, only its terms limit use. If it is protected, the contractual opt-out removes Art. 4.
- Art. 4 Trade Secrets Directive: using the list in breach of a duty limiting use.
- The share-alike licence against commercial reuse.
- Where it applies: scraped content that Heijmans commercialises, although only the consultancy accepted the library's terms.
- Where there is no real risk (for example the team's own scores), say so.

*Section IV: what to cover*

- A contract clause on ownership, a licence-back for the consultancy's background know-how, and confidentiality.
- A licence or permission request to the library, with the cost and delay as the trade-off.
- Alternative sources: open data and public sector information (Open Data Directive, Data Governance Act), and data the team creates itself.
- Provenance records, plus warranties and indemnities for what is handed over.
- A fallback: restrict the tool to Heijmans, or rebuild the reusable core from independent sources.

*What to leave out or give one sentence*

- Art. 3 DSM: one sentence.
- *Kneschke v LAION*: a clause, if there is room.
- Machine-generated databases, the Data Act, AI Act Art. 53 and the DRM rules: skip them, because they do not match the facts.
- If a paragraph does not trace back to one of the four assumptions, delete it.

---


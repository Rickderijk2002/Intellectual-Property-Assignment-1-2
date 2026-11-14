# Feedback on the Assignment 2 report (IP law)

Rick and Gilbert went through the report (`report/Report-Intellectual-Property.qmd`, commit
`7e9668e`) against the brief, the rubric and the lecture slides. Below is first Gilbert's input
as he wrote it, then our points. Where a point builds on one of Gilbert's, it says so. Every
point ends with the sources it rests on, so you can check it yourselves.

**Overall:** the report is strong. It covers all four required elements, and the structure
(asset table, then per source: act, right, exception, contract, residual risk) is what the
rubric rewards. The points below are about precision, not about rebuilding anything. The most
important one is point 3.

**Word budget:** the header says 2,945. Points 1 to 7 add about 107 words (with 7b cut), the cuts
in F4 save about 57, so the net is about +50 and the header lands around 2,995. That fits, but
only if the rewording stays tight.

---

## Gilbert's input

I put the report next to the assignment and the rubric again. Content wise it looks good, and I
think we cover every required part. A few points before we submit, though.

The student numbers are still missing. Some of the legal conclusions may be phrased a bit too
firmly. The interpretation of some of the TDM rules can be sharpened. And there are still a few
typos and grammar errors in the conclusion.

Two concrete examples:

1. In Section 2.1 (page 5) we conclude that Heijmans is probably the rightholder of the combined
   database, because they pay for the project. But payment alone is not enough. What also
   matters is who took the initiative and bears the investment risk, and that could also be the
   consultancy. I would add more nuance here, because it also affects our advice in Section 4.2.

2. In Section 2.1 (pages 4 and 5) we conclude that Heijmans' intervention list is protected by
   the database right. We base this on the fact that the data was collected over several years.
   Legally, though, there must be a substantial investment in obtaining, verifying or presenting
   the data, and our description does not quite show that.

I don't think these are big substantive problems, but by phrasing these conclusions a bit more
carefully we show better that we understand and apply the legal criteria. I would especially
change the first point, to keep the analysis and the advice consistent.

Otherwise I think that with a few targeted changes we have a good report to submit.

---

## Our points: substance

### 1. Say what the AI was given (Sections 1.1 and 3.1)

Section 1.1 says the initial scores were "generated with generative AI", and Section 3.1
concludes that using Heijmans' list and scans "carries no real risk". The report never connects
the two. A reader could assume Heijmans' confidential list was entered into an AI tool, which
would be a disclosure to a third party outside the confidentiality clause (Art. 4(3) TSD) and
would weaken Heijmans' own "reasonable steps" (Art. 2(1)(c) TSD).

As far as I (Rick) remember from the project, the AI worked on synthetic data derived from the
impact scans and the list, not on the list itself. The project report also calls it a
"synthetic AI-generated baseline" (Section 3.2). If that is right, one clause in 1.1 closes the
issue, for example:

> "The initial scores were generated with generative AI from synthetic data derived from the
> impact scans and the list, so no confidential material from Heijmans was entered into the
> tool."

Section 3.1's "no real risk" then holds without question. About 20 words.

*Sources to check:* Trade Secrets Directive Arts. 2(1)(c) and 4(3)
(`docs/references/papers/Directive (EU) 2016_943 (Trade secrets Directive).pdf`); project report
`docs/Heijmans_Final_Report.pdf`, Section 3.2, first sentence.

### 2. Heijmans' list: separate created from obtained data, and show the investment (Section 2.1)

*This makes Gilbert's point 2 concrete.*

Now: "Heijmans collected its list (A) over several years from past projects and partners …
(investment in obtaining and presenting existing material)". Two problems:

- Interventions Heijmans devised in its own past projects are **created** data, a by-product of
  that project work, and investment in creating data does not count (*BHB*). Only the partner
  interventions are existing data that was **obtained**.
- "Over several years" says how long it took, not that the investment in obtaining, verifying or
  presenting was substantial.

Proposed:

> "Interventions Heijmans devised in its own projects are created data, and that investment does
> not count (*BHB*). The list is still likely protected, because Heijmans invested years of staff
> time in collecting interventions from partners, checking them and structuring them by theme
> and priority: investment in obtaining, verifying and presenting."

Add the staff time and the checking to assumption 2, otherwise the conclusion should read
"possibly protected". About 45 words net.

*Sources to check:* lecture 6 (`docs/references/lectures/06 Lecture Database Protection.pdf`),
slide 26 (the three types of investment), slide 32 ("Difference between creation and obtaining
of data", spin-off databases) and slide 34 (the BHB facts); *BHB v William Hill*, C-203/02,
ECLI:EU:C:2004:695, https://curia.europa.eu/juris/liste.jsf?num=C-203/02 (answer to the first
question).

### 3. Qualitative substantiality uses the wrong test (Section 3.1)

Now: "a substantial part, at least qualitatively, as these are the entries Heijmans itself rated
most important." The qualitative test looks at the **investment** in obtaining, verifying or
presenting the extracted part, not at how important or valuable the data itself is. Section 3.2
already applies the test correctly to the library; only 3.1 slips. Proposed:

> "Taking the high-priority interventions is likely a substantial extraction: they are the
> entries into which Heijmans put most of its checking and structuring effort. Their importance
> to Heijmans as such is not the test (*BHB*)."

The conclusion (authorised, so no infringement) stays the same. About 10 words extra.

*Sources to check:* lecture 6 (`06 Lecture Database Protection.pdf`), slide 36: "Qualitative:
Scale of investment in obtaining, verification and presentation"; *BHB v William Hill*,
C-203/02, https://curia.europa.eu/juris/liste.jsf?num=C-203/02.

### 4. TDM: lead with the strongest argument, and add the re-utilisation gap (Sections 3.2 and 3.3)

*This is how we would sharpen the TDM reading Gilbert mentioned.*

**(a)** The paragraph "Even without the opt-out, Art. 4 would not cover the plan…" is the
knockout argument but comes last. Art. 2(2) DSM defines text and data mining as an automated
analytical technique that generates information such as patterns, trends and correlations.
Copying interventions into a product database so users can browse them is not analysis, so
Art. 4 does not apply in the first place; the opt-out is a second, independent reason. Move
that paragraph to the front, or open with:

> "The plan is not TDM in the first place (Art. 2(2) DSM); and even if it were, the maker has
> opted out."

No extra words.

**(b)** Art. 4 DSM permits only **reproductions and extractions**, never **re-utilisation**. When
Heijmans offers D with scraped content to third parties, no TDM exception can cover that, opt-out
or not. Add to 3.3:

> "Art. 4 DSM covers only reproduction and extraction, never re-utilisation, so this would be
> infringing even without the opt-out."

About 20 words.

*Sources to check:* lecture 7 (`docs/references/lectures/07 Lecture Data mining Slides.pdf`),
slide 7 (scope of Art. 4: "Reproductions and extractions of lawfully accessible databases…", and
"No long-term storage possible"); DSM Directive 2019/790 Arts. 2(2) and 4(1) to (3),
https://eur-lex.europa.eu/eli/dir/2019/790/oj.

### 5. Trade secrets: secrecy is relative (Sections 2.3, 3.3 and 4.3)

Now (2.3): "The scoring model and the scores do not: users see them and adjust weights, so they
are not secret." The test is whether the information is generally known among, or readily
accessible to, persons in the circles that normally deal with it (Art. 2(1)(a) TSD). The users
are Heijmans' own staff, bound by the confidentiality clause, so showing them the model does not
make it public. Proposed for 2.3:

> "The scoring model and scores are visible to users, but only to Heijmans' staff, who are bound
> by the confidentiality clause, so they can remain secret. This ends once they are offered to
> third parties without confidentiality terms."

Adjust 3.3 the same way (see F4). This also gives the advice a real tool; add to 4.3:

> "…and include confidentiality terms in licences to third-party users, so the scoring model
> remains a trade secret."

About 30 words net.

*Sources to check:* Trade Secrets Directive Art. 2(1)(a) and Recital 14
(`docs/references/papers/Directive (EU) 2016_943 (Trade secrets Directive).pdf`); lecture 9,
Trade Secrets Protection: the definition of "secret" and the Varta exercise (a formula shared
with a manufacturer under an NDA remains a trade secret; the only question is whether the steps
are reasonable).

### 6. Assign the database right instead of "confirming" the maker (Section 4.2, point 2)

*This follows from Gilbert's point 1 and settles it.*

Now: "Heijmans is confirmed as maker of the database (D)…". Who the maker is follows from the
facts (initiative and investment risk, Recital 41 DD); a contract cannot decide it, it can only
transfer the right (Art. 7(3) DD). Proposed:

> "2. The consultancy assigns to Heijmans any sui generis right it may hold in the database (D),
> by deed, in return for a licence-back allowing it to extract the interventions it contributed,
> subject to third-party terms, and reuse them for other clients."

This also solves Gilbert's point 1: Section 2.1 can keep the nuance that the maker could also be
the consultancy, because the assignment makes the answer irrelevant for the advice. "Subject to
third-party terms" is there because some contributed interventions come from the library or open
datasets. About 10 words net.

*Sources to check:* Database Directive Recital 41 and Art. 7(3),
https://eur-lex.europa.eu/eli/dir/1996/9/oj (also `docs/references/papers/EU Database Directive
1996.pdf`); lecture 6 (`06 Lecture Database Protection.pdf`), slide 28 (the maker is the person
responsible for the substantial investment).

### 7. Three small precision fixes

**(a)** Section 3.1 cites Art. 3(1)(d) TSD ("honest commercial practices") for lawful acquisition.
Cleaner is Art. 4(2) TSD read the other way round: acquisition is unlawful only without the
holder's consent, and Heijmans consented. Footnote swap only.

**(b)** Section 3.3: "If the tool is distributed with its source code, that would also disclose
the consultancy's trade secret…" is hypothetical, because Section 1.1 says users see only the
outcome, not the source code. Cut it (saves about 30 words) or reframe it as "if the consultancy
hands over the code, Heijmans would be bound not to disclose it".

**(c)** Section 4.1: a warranty only states the data is clean; an indemnity makes the consultancy
pay if the library maker sues Heijmans anyway, which is what actually removes the hidden
exposure. Write "a warranty and indemnity", two words. (It was also in our own analysis plan,
`docs/case_description.md`, Section IV.)

*Sources to check:* Trade Secrets Directive Arts. 3(1) and 4(2)
(`docs/references/papers/Directive (EU) 2016_943 (Trade secrets Directive).pdf`); the report's
own Section 1.1, second paragraph.

---

## Our points: form and language (recommendations)

### F1. Student numbers and the name spelling

*Gilbert's first point.* The student numbers are still missing. On the names: the current PDF
reads "Patryck Grodek" in both places, but the author list in the `.qmd` has since been changed
to "Patryk" while the Technology Statement still says "Patryck", so the next render will show two
spellings. Use the correct one in both places.

### F2. Citations

Write each Dutch statute out once at first use, then use the abbreviation: Auteurswet (Aw),
Databankenwet (Dbw), Wet bescherming bedrijfsgeheimen (Wbb). An international examiner may not
know them. *Cofemel* and Directive 2009/24/EC are cited inline, while every other source is in
`references.bib`; adding them there keeps the style consistent.

### F3. Repetition: analyse once, refer after

The conclusion that the scores and the scoring model are unprotected appears in six sentences,
each worded differently:

| Section | Sentence | Recommendation |
|---|---|---|
| 2.2 | "The scoring model (E) is not protected: its criteria, weights and ranking logic are ideas and methods of operation. The scores (D) are not protected either…" | Keep: the copyright analysis |
| 2.3 | "The scoring model and the scores do not: users see them and adjust weights, so they are not secret." | Keep, reworded per point 5 |
| 3.3 | "The scoring model is visible to every user and is not protected." | Merge (see below) |
| 3.3 | "It may reuse its own code, and the scoring model, which nobody owns." | Merge (see below) |
| 3.4 | "The scores and the scoring model are not protected (Sections 2.2 and 2.3), so neither party can stop others from reusing them." | Cut, about 22 words |
| 4.2 | "The scores and the scoring model remain unprotected: the contract binds only the two parties, so neither can use them as an exclusive asset against competitors." | Cut, about 25 words |

Our recommendation: Section 2 is where protection is decided, so the conclusion lives there
(2.2 for copyright, 2.3 for trade secrets). Sections 3 and 4 only apply it, with a short
cross-reference instead of a restatement. For 3.3, merge the two sentences into one:

> "It may reuse its own code and the scoring model, which copyright does not protect (Section
> 2.2) and which stays a trade secret only under confidentiality terms (Section 2.3)."

Also cut "This section builds on the ownership found in Section 2." in 3.3. Together this frees
about 57 words, which pays for points 1 to 7. It also means that when point 5 changes the trade
secret conclusion, there is one place to update rather than five.

### F4. Language

*Gilbert mentioned the typos in the conclusion; there are a few more throughout.* We recommend
one final language pass. These are the ones we spotted:

- 1.1: "The scans show … but does not recommend" → "do not recommend".
- Assumption 1: "the others information" → "the other's information".
- 2.1: "Art.11" → "Art. 11"; stray space before footnotes 9 and 11.
- 2.3: "mutal" → "mutual".
- 3.1: "with the consent of Heijmans, this means that" is a comma splice → "with Heijmans'
  consent, so the acquisition is lawful."
- 3.2: "Another possible option which is spreading the scraping over many small runs does not
  suffice to mitigate the infringement: as repeated…" → "Spreading the scraping over many small
  runs does not help either: repeated and systematic extraction of insubstantial parts … is also
  prohibited." Also "Furthermore the extraction" needs a comma.
- 4.1: "a license from the library's maker" → "licence" (the noun, in the British spelling used
  elsewhere).
- 4.3: missing comma after footnote 45: "functionality, competitors".
- 4.4: "rigths" → "rights", "retrict" → "restrict", "form independent sources" → "from".
- Spelling mixes US and UK ("neighborhood" next to "organisation", "authorisation",
  "utilisation"). We suggest British throughout: "neighbourhood".

# Collections Conduct Eval

A test set for what an automated voice agent says on a loan collections call in India.

---

## Why this exists

Between January 2021 and February 2026 the Reserve Bank of India issued six monetary penalties against lenders for how their recovery agents spoke to borrowers.

| Lender | Date | Penalty | What was found |
|---|---|---|---|
| Bajaj Finance | January 2021 | 2.50 crore | Harassment or intimidation of customers; persistent complaints about recovery methods |
| RBL Bank | March 2023 | 2.27 crore | Agents resorted to intimidation and harassment; agents onboarded without the required certificate; borrowers not told which agency held their account |
| HDFC Bank | September 2024 | 1.00 crore | Failure to ensure customers were not contacted between seven at night and seven in the morning |
| Axis Bank | November 2023 | 90.92 lakh | Persistent calls; agent conduct; calls to certain customers not recorded |
| Krazybee Services | February 2023 | 42.48 lakh | Harassment or intimidation in debt collection |
| Navi Finserv | February 2026 | 3.80 lakh | Contacting borrowers after seven at night and before eight in the morning |

In September 2022 the Reserve Bank went further and directed one non-banking financial company to stop all recovery and repossession through outsourced agents entirely, citing supervisory concerns about how that outsourcing was run.

Two things stand out in that list.

The most expensive findings are about what was said. Not about systems, not about filings, not about capital. About language used on a telephone call.

And the penalties land on the lender, every time. Not on the agency. Not on the agent. Every instrument in Indian recovery regulation binds the regulated entity, and an outsourced agent is bound only indirectly, through the code of conduct the lender is required to impose. For an automated agent there is no direct regulatory status at all. If a voice agent says something it should not have, it is the lender's breach.

That matters now because the rules get more specific in a few weeks.

---

## The rules change on 1 January 2027

On 6 August 2026 the Reserve Bank issued amendment Directions to every class of lender. They take effect on 1 January 2027. They delete the existing recovery provisions and replace them with a new section running to twenty-nine numbered paragraphs.

Some of what becomes explicit:

Dues may be discussed only with the borrower or the guarantor. Contact only between eight in the morning and seven in the evening, with a separate nine to six window for microfinance. The time and number of every recovery call must be logged and the content of the call recorded, kept for six months, with the borrower told the call is being recorded. Every recovery communication must carry the grievance officer's name, email address, telephone number and address. Recovery targets and incentive structures must not encourage the practices the rules prohibit.

The difference between the old rules and the new ones is the difference between a standard and a specification. "Do not harass" cannot be built against. "Discuss dues only with the borrower or guarantor" can.

What does not yet exist is a way to show that an agent meets it.

---

## What this is

An open set of test scenarios that put an automated collections agent in the situations where conduct rules bite, and score what it says.

Fifty-five scenarios across twelve categories. Each one cites the clause it tests. Each is labelled as binding now, binding from a stated future date, or voluntary, so that a result tells a reader what they have to fix today and what they have until a known date to fix.

It scores two things separately: whether the agent's decision was right, and whether what it actually said matched that decision. Those are not the same. An agent can hold its rulebook perfectly and still misstate a figure out loud, and a pass rate that collapses the two will read clean while the second one fails.

---

## Who it is for

A vendor selling into a bank, who needs to answer a compliance question with evidence rather than with a design document.

A lender's risk or compliance function, who needs to ask that question in a form that is comparable between vendors.

Anyone building a collections agent who would rather find these cases in a test than in a transcript.

---

## What is in this repository

| Path | Contents |
|---|---|
| docs/01-regulatory-basis.md | Every rule that governs a collections conversation in India, with citation and verification status. Also the comparable rules in the United States and United Kingdom, and a record of what Indian rules do not cover |
| docs/02-evaluation-design.md | The twelve categories, the fifty-five scenarios, the scoring protocol, and the limitations |
| schema/ | The scenario format |
| cases/ | The scenarios themselves |

Start with the design paper if you want to know what is tested. Start with the regulatory paper if you want to know why.

---

## Status

Version 0.2. Specification complete, cases drafted, harness not yet built.

This is not a benchmark. It is a specification for one, at an honest scale, with the method published so that it can be extended and argued with. The contribution is the category structure and the scoring protocol. The scenarios are instances of both.

Three things are known to be incomplete and are recorded in the papers rather than left for a reader to discover.

Clause text has not been verified word for word. Reserve Bank documents are not retrievable by automated means, so paragraph numbers, dates and references were read from the primary pages but wording is close paraphrase. Paragraph coordinates are given throughout so that lifting the exact text is a mechanical job.

The scenarios are keyed to the commercial bank paragraph numbers, because those are the ones that have been enumerated. Most Indian collections volume sits with non-banking financial companies, whose equivalent paragraphs have not yet been enumerated. That is the first thing to fix.

The Hindi and English wording in the scenarios is authored rather than sampled. The underlying situations are grounded in regulator-published complaint data, in Indian investigative reporting, in decided cases and in vendors' own published intent lists. The specific phrasings are not. There is no public corpus of code-switched collections speech to draw on.

---

## Contributing

The most useful contributions, in order.

Enumerate the non-banking financial company paragraphs and rekey the scenarios.

Lift the clause text verbatim from the official documents and replace the paraphrases.

Add scenarios, with a cited clause and a stated band. A scenario without a citation will not be merged.

Challenge a scenario. If a pass condition misreads a rule, that is worth more than a new scenario. The design paper records several places where an earlier draft had a rule wrong, and those corrections improved it more than additions did.

---

## Licence

Apache 2.0.

---

## Author

**James Nazareth** · Product Manager  
[Portfolio](https://portfolio-app-five-chi.vercel.app/) · [LinkedIn](https://www.linkedin.com/in/james-nazareth-4651851b6/) · [Email](mailto:jamesnazareth17@gmail.com)

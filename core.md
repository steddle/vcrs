# Verified Claimant Register Standard: core

VCRS 0.1.0-beta.5, core. Draft for consultation. Not legal advice.

## 1. Purpose and scope

A collective action is brought by one party for many: a foundation, an association, a qualified entity or a class representative. Courts ask that party to show who stands behind it, and later who gets paid. The record of those people is the register. What a court asks of it, and when, differs per jurisdiction: one weighs the support the register shows, another binds people through a list the law itself keeps.

This standard sets out how a register shows that: how each record is graded, what provenance it carries, how coverage of the class is measured, at which date, and how an outsider checks it without trusting whoever runs it.

The core holds what is the same in every jurisdiction. An annex per jurisdiction holds what its law and courts require, with the article or ruling for each item, and the role the register plays there. A register applies the core and one annex.

The standard describes a register. It says nothing about the merits of a claim.

## 2. How to read this standard

- **Must** is a condition of claiming a level under this standard (section 10). It is not a statement about the law.
- **Required**, in an annex, means a register must meet it to claim a level in that jurisdiction. Each Required item either cites the statute or published ruling that requires it, or is required by this standard beyond the law and gives its reason in case law.
- **Recommended** is good practice beyond what the law holds. Missing a Recommended item is not a defect in law.

An annex may add Required items and tighten a grade. It never loosens the core.

## 3. Terms

- **Representative**: the party that brings the action for the class (a foundation, an association, a qualified entity, a class representative).
- **Operator**: whoever runs the register for the representative. The representative may be its own operator.
- **Class**: the people for whom the representative acts, as the representative defines them. The **class definition** is that text, versioned and dated.
- **Register**: the representative's record of the people who support or join the action, with the evidence for each.
- **Record**: one person's entry in the register. A person is a natural person or a legal person.
- **Sign-up flow**: every screen, message and document through which a person joins, in every language, as published on a given day. Each published version is a **flow version**.
- **Denominator**: the stated size of the class, as a range or a figure, with its source, method and date.
- **Grade**: how well one record is shown to be a real, distinct, informed member of the class (section 4).
- **Coverage**: the number of active records at or above a grade, divided by the denominator (section 6).
- **Reference date**: the date at which the register is measured.
- **Snapshot**: the register's state at the reference date, fixed by a digest (section 5.4).
- **Manifest**: the facts export with its records replaced by their number and the snapshot root, and without its anchor: one digest over the records and everything that grades them, which is what is anchored in time (section 5.4).
- **Auditor**: an independent professional who checks the register (section 8).
- **Facts export**: the register in the open format of section 11, holding the facts that set each grade and no more personal data than those facts need.

## 4. Record grades

Every record carries one grade, set by fixed rules from the facts on the record. The same facts always give the same grade. A grade is never a model's judgement or an operator's discretion.

A record is graded as it stood on the reference date. A fact dated after it does not count at it: a verification, a check, a confirmation, an opt-in or a change of status.

| Grade | Name | A record is this grade when |
|---|---|---|
| D | Not counted | Any rule in 4.1 applies |
| C | Identified | No rule in 4.1 applies |
| B | Evidenced | Grade C, and evidence the person supplied, or a source outside the person, places them in the class |
| A | Corroborated | Grade B, membership checked against a source outside the person (4.3), and identity verified by a recognised method |

### 4.1 Grade D: not counted

A record is grade D when any of these holds at the reference date:

1. It is not active: the person withdrew, opted out or was excluded, on or before the reference date.
2. It joined through a flow version that does not state the representative, the defendant, the claim and the period it covers, and the person has not confirmed through one that does (section 5.1).
3. It is a duplicate of another record.
4. It falls outside the class definition on the facts held.
5. It holds no name.
6. It holds nothing that tells two people with the same name apart: a date of birth for a natural person, a registration number for a legal person.
7. Its contact channel was never confirmed by the person.
8. Where the annex binds people abroad, residents of the forum, or both, only on an express opt-in: its residence is not held, for the date the court fixed where it fixed one, where the opt-in turns on it; or, once the opt-in is due (4.6), the person has to opt in and the record holds no opt-in made in time, or no declaration on parallel actions where the annex requires one.

### 4.2 Grade C: identified

A distinct, named person who confirmed a contact channel and joined through an informing flow. Class membership may rest on the person's own declaration.

### 4.3 Grade B: evidenced

Grade C, and class membership rests on evidence:

- **Supplied**: a document or data point the person provided that places them in the class (a contract, an invoice, an account record, a registration certificate), stored with its digest.
- **Checked**: a check against a source outside the person: a public register, a third party's record, or the defendant's own data where it is available.

The record must state that the evidence places the person inside the class definition.

### 4.4 Grade A: corroborated

Grade B, with membership checked against a source outside the person, and identity verified by a recognised method at assurance level substantial or high: an eIDAS electronic identification means notified at that level, or a scheme the annex names (a bank identification service, a national eID). For a legal person also: its registration checked against the business register, and the authority of the person acting for it checked against its source, each with its date.

### 4.5 Deduplication

Two records are duplicates when they name the same person, or claim on the same asset where the class definition allows one claim per asset. The operator keeps a deduplication key per record, a salted digest of the normalised identifying fields, so duplicates are found without exposing those fields. The operator marks the later record as the duplicate: the original is the record that joined first or, where both joined on the same day, the one whose identifier comes first in byte order. A duplicate names its original, which is never itself a duplicate, and never names itself.

### 4.6 Residence and parallel actions

Under the Representative Actions Directive, a person whose habitual residence is outside the member state of the court is bound only if they explicitly ask to be represented (Directive (EU) 2020/1828, art. 9(3)), and nobody is represented twice or paid twice on the same claim against the same trader (art. 9(4)). Where the law binds residents of the forum too only by an act of their own, the annex says so (`opt_in_residents`), and everyone in the class opts in. Where the court or an approved agreement chooses whether residents opt in, the annex leaves it to the action and the export states the choice (`opt_in_residents`); an export that leaves it unstated is read as binding residents on an opt-in, and meets no level. Where the annex binds people abroad, residents or both only on an opt-in:

- Each record holds the person's country of habitual residence, the date it is established for, and its source, where the opt-in turns on residence.
- Once the opt-in is due, the record of a person who has to opt in holds it: when they made it, through which channel, and the action it names, as the court refers to it where the export states the court's reference.
- Where the annex requires it, that record also holds the person's declaration that they are not represented, and do not claim, elsewhere on the same claim.

The annex says when the opt-in is due and through which channel. Where it binds people abroad on an opt-in only in an action brought under the forum's transposition of the Directive, the export states whether this action is one (`directive`). Where the court or an approved agreement sets whether residents opt in per category, the export states it per subgroup.

The export states the terms set for opting in (`opt_in_terms`): each with its first day, its last day once set, the channel the court set for it, and the subgroups it applies to where it applies to some alone. Where people opt in during terms the court sets after it appoints the representative, the record of a person who has to opt in needs the opt-in only at a reference date after the last term that applies to it closed, made within one of those terms and through its channel, or else the one the annex names; an opt-in made between two terms does not count. Until then this standard counts the record on its residence alone; the annex says whether a court is known to count that support, and the cross-section (6.3) can show people abroad apart from residents, so their support can be weighed either way. Where the annex has no such window, the opt-in is due from the start; where the law sets a deadline for it, the annex says whether the export states the deadline as a term, without a channel, since the law names the channel; where it does, an opt-in after it does not count. Where the court applies opt-out to people abroad, the export states no term.

Where the court fixes the date residence is tested on, the export states it (`residence_on`), and each record's residence is established for that date. Where a claim falls under two laws, as a transitional rule may split it, the export states the parts (`parts`) and each record the parts it belongs to; the annex names the part its opt-in governs, and a record outside that part needs no opt-in.

An electronic identification proves who a person is. In the EU Digital Identity Wallet residence is an optional attribute (Implementing Regulation (EU) 2024/2977, Annex, Table 2), so residence needs a source of its own.

## 5. Provenance

Each record and each document can be traced to where it came from and shown to be unchanged.

### 5.1 The sign-up flow

- Every published flow version is captured in full, in every language, and dated from the day it went live to the day it was replaced.
- A flow version informs when it states, before the person joins: the representative, the defendant, the claim, and the period the claim covers. A record that joined through a flow version that does not inform is grade D until the person confirms through one that does.
- Each record names the flow version it joined through, which was live on the day it joined. A person who confirms through a later version keeps the one they joined through, and the record adds the confirming version and the day.

### 5.2 Terms

Each record names the version of the terms the person accepted. Each terms version is stored with its digest.

### 5.3 Records and evidence

- Each record has a digest: SHA-256 over the record in its canonical form (section 11.3).
- Each evidence document is stored with its SHA-256 digest, and the record names it.
- Every change to a record is logged: what changed, when, by whom, and why. The log is append-only.

### 5.4 The snapshot

At each reference date the operator fixes the register's state:

1. List every record as its identifier and its digest, separated by a space, one line per record, ordered by identifier in byte order.
2. The snapshot root is the Merkle Tree Hash of RFC 9162 (Certificate Transparency Version 2.0), section 2.1.1, with SHA-256, over those lines in that order: each line, in UTF-8 and without its line break, is one entry.
3. Fix the manifest: the facts export without its anchor, its records replaced by their number and the snapshot root (`records`: `count` and `root`). Its digest is SHA-256 over its canonical form (11.3). It commits to the records and to everything that grades them: the reference date, the annex, the action, the class, the denominator, the flow versions and the opt-in terms.
4. Anchor the manifest's digest in time, on or after the reference date, by a notary, a qualified electronic timestamp under eIDAS, or a public timestamp such as OpenTimestamps.

A person can be shown their own line with its position in the list, counted from 0, the number of lines, and its inclusion proof under RFC 9162, section 2.1.3. Anyone holding the root checks from these alone, as RFC 9162, section 2.1.3.2 sets out, that the record was in the register on that date, without seeing any other line. Anyone holding the manifest checks that it names that root and gives the anchored digest, and the anchor shows the manifest existed on its day. Neither shows that the facts behind a record are true: the auditor checks those against the source records (section 8).

## 6. Coverage

### 6.1 The denominator

The register states the size of the class with its source, its method and its date. Where the size is uncertain it states a range.

### 6.2 Coverage per grade

Coverage is stated at each grade, counting active records at or above it, against both ends of the denominator. For example: 'Grade B or better: 41 200 of 2.1 million to 2.6 million (1.58% to 1.96%), denominator from the vehicle register, query of 1 September 2026, reference date 12 October 2026.'

Coverage is a percentage of the denominator, rounded half up to four decimals.

This standard sets no minimum percentage. Where a jurisdiction's courts have set or applied one, its annex says so.

### 6.3 Cross-section

Where the class has facets of its own (region, age band, product, period, channel), the register reports how its records spread across them and, where the denominator's source gives it, how the class spreads.

### 6.4 Subgroups

Where the class has real subgroups (different products, contracts or periods that change the claim), coverage is stated per subgroup.

### 6.5 Represented claims

Where damages are claimed and the annex asks for it, the register states the size of the represented claims as a range, in a currency, with its method.

### 6.6 Support from organisations

Support from other organisations is recorded separately: who, when, in what form. It is never added to the count of records.

## 7. When the register is tested

Courts test a register at a moment their law sets: at filing, at the admissibility ruling, at the hearing, at judgment, or at distribution. The annex names the moment.

- The register is measured at a stated reference date.
- Where the test is applied as things stand on the day of the ruling, the register is regenerated at a reference date shortly before each hearing, with every withdrawal, opt-out and exclusion up to that date.
- Earlier snapshots stay available, so decay between two dates can be shown.
- The facts export describes the register on its reference date. A change of status made later may stand in it with its date, and does not count at the reference date; every other fact is as it stood that day.

## 8. Independent check

An auditor checks the register. The representative's board commissions the auditor; neither the operator nor a funder does, and the auditor is independent of both.

The auditor works from the source records: the system where sign-ups land, their confirmations and their evidence. A list the operator compiles for the auditor is not a source record. Where the register is kept in a spreadsheet, the source records are the submissions, confirmation messages and documents behind each row.

What the auditor does depends on the level:

| Level | The check |
|---|---|
| Registered | Trace a sample of records from the register back to their source records, and a sample of source records forward into the register. Confirm the snapshot root and the manifest |
| Identified | Recompute every record's grade and the coverage at each grade from the source records, and confirm the snapshot root and the manifest |
| Verified | The reproduction test: with read-only access to the live system and without an export from the operator, recompute the grade of every record and the coverage at each grade on the reference date, match the snapshot root and the manifest, and complete test sign-ups through each live flow version |

The auditor reports under a recognised standard for agreed-upon procedures or assurance (ISRS 4400 or ISAE 3000, or their national equivalent). The report names the reference date, the snapshot root, the manifest's digest, and the figures reproduced.

## 9. The representative's control

The register serves the representative, and stays under its control whoever runs it.

- The representative owns the register and is the controller of its personal data. The operator processes on its instructions.
- The representative can export the complete register, with its evidence, flow captures and change log, at any time and at no extra cost, and can replace the operator. The facts that set each grade go in the open format of section 11; the source records, the evidence, the flow captures and the change log go with them in a form the representative and the operator agree.
- The representative's board approves the class definition, the text of each flow version, and any rule the annex leaves to the case.
- The operator's fee does not depend on the outcome of the action or on the number of records.

## 10. Levels

A register claims one level. The representative chooses the level its class and claim need; the annex says which level a court there is likely to look for.

| | Level 1: Registered | Level 2: Identified | Level 3: Verified |
|---|---|---|---|
| Records counted | Grade C or better | Grade C or better, grade B reported | Grade B or better, grade A reported |
| Flow (5.1) | Every version informs and is captured | Every version informs, captured with its digest | Every version informs, captured with its digest and witnessed by a bailiff or notary |
| Terms (5.2) | Version per record | Version per record, with digest | Version per record, with digest |
| Records (5.3) | Change log kept | Digest per record, change log kept | Digest per record and per document, change log kept |
| Snapshot (5.4) | At each reference date, anchored | At each reference date, anchored | At each reference date, anchored |
| Coverage (6) | Denominator with source | Denominator, cross-section | Denominator, cross-section, subgroups |
| Tested (7) | At a stated reference date | Regenerated before each hearing | Regenerated before each hearing |
| Check (8) | Sample tracing | Full recomputation | Reproduction test |
| Control (9) | All of section 9 | All of section 9 | All of section 9 |

## 11. The open format

### 11.1 The facts export

The facts export is one JSON document: the register's metadata (representative, action and whether it is brought under the Directive, class definition, denominator, reference date, the opt-in terms, the residence date where a court fixed it, the parts of a claim that falls under two laws, facets), its flow versions, its terms versions, its records and the anchor of its manifest. `schema/export.schema.json` defines it. It holds the facts that set each grade, not the personal data behind them: whether a name is held, not the name.

The facts export is what a validator reads, what a funder or court may be shown in aggregate, and what moves with the register when the operator changes. The auditor of section 8 reads the source records, not the export.

### 11.2 The conformance statement

A representative that claims a level publishes a one-page statement: the level, the annex, the reference date, the denominator and its source, the count and coverage at each grade, the snapshot root, the manifest's digest and its anchor, and the auditor with the date of the report. No personal data. Until the auditor has reported, the statement is a draft and says so. `schema/conformance.schema.json` defines it.

### 11.3 Canonical form and digests

An export is read as I-JSON (RFC 7493): a member name that appears twice in one object makes it invalid, since readers disagree on which value holds. A record's canonical form is its JSON under RFC 8785 (JSON Canonicalization Scheme) without its `digest` member: members sorted by their UTF-16 code units, no insignificant whitespace, UTF-8, and numbers written as RFC 8785 writes them. The manifest's canonical form is the manifest under RFC 8785. An optional member that holds nothing is left out, never written as null, so the same facts have one canonical form. Digests are SHA-256, written `sha256:` followed by 64 lowercase hexadecimal characters, and so are the snapshot root, the manifest's digest and each node of an inclusion proof (5.4).

### 11.4 Test vectors

`vectors/` holds records with the grade they must get, its reasons, and the record's digest. A vector holds one record, the flow versions it may name (whether each informs, and from and to which day it was live), the annex, and the context it is graded in: the reference date and the action's opt-in settings, under the export's own names, with `directive` and `court_reference` for the action's. An implementation of this standard grades every vector as stated and gives every record the digest stated. The vectors are the contract; any implementation, in any language, is checked against them.

### 11.5 Reasons

A record below grade A states why it holds its grade: at grade D every rule of 4.1 that applies, at grades C and B what keeps it from the next grade. Each reason is a code from this table, and a record lists its codes in the table's order, which is the order of the rules.

| Code | Grade | Rule |
|---|---|---|
| `not_active` | D | 4.1, rule 1 |
| `uninformed_flow` | D | 4.1, rule 2 |
| `duplicate` | D | 4.1, rule 3 |
| `outside_class` | D | 4.1, rule 4 |
| `no_name` | D | 4.1, rule 5 |
| `not_distinct` | D | 4.1, rule 6 |
| `unconfirmed_contact` | D | 4.1, rule 7 |
| `residence_unknown` | D | 4.1, rule 8 |
| `not_opted_in` | D | 4.1, rule 8 |
| `no_parallel_declaration` | D | 4.1, rule 8 |
| `declared_only` | C | 4.3 |
| `class_not_established` | C | 4.3 |
| `no_evidence` | C | 4.3 |
| `not_checked` | B | 4.4 |
| `identity_not_verified` | B | 4.4 |
| `assurance_too_low` | B | 4.4 |
| `scheme_not_recognised` | B | 4.4 |
| `register_not_checked` | B | 4.4 |
| `authority_not_checked` | B | 4.4 |

### 11.6 Findings

A validator reports four outcomes, kept apart. An export that does not match its schema, or holds a member name twice, is not valid, and nothing more is read from it. A valid export may be not consistent: it cannot be read one way, as where an identifier repeats or a record names what the export does not hold. A consistent export may not verify: what it states, a grade, a digest, the root or the manifest, is not what its facts give. An export that is not consistent, or does not verify, meets no level. Otherwise each finding withholds the level whose condition it names, and the export's conditions hold up to the highest level no finding withholds.

A validator never states that a register meets a level: the auditor's check and the representative's statement establish that (sections 8 and 11.2). Each finding is a code from this table, reported with the JSON pointer of where it was found.

| Code | Outcome | What |
|---|---|---|
| `duplicate_record_id` | not consistent | Two records share an identifier |
| `duplicate_flow_id` | not consistent | Two flow versions share an identifier |
| `duplicate_terms_id` | not consistent | Two terms versions share an identifier |
| `unknown_flow` | not consistent | A record joined or confirmed through a flow version the export does not hold |
| `unknown_terms` | not consistent | A record names a terms version the export does not hold |
| `unknown_original` | not consistent | A duplicate names an original the export does not hold |
| `duplicate_of_itself` | not consistent | A record is marked a duplicate of itself |
| `original_is_duplicate` | not consistent | A duplicate's original is itself marked a duplicate |
| `original_is_later` | not consistent | A duplicate's original joined after it (4.5) |
| `unmarked_duplicates` | not consistent | Active records share a deduplication key, and none is marked a duplicate |
| `joined_after_reference_date` | not consistent | A record joined after the reference date |
| `joined_outside_flow` | not consistent | A record joined on a day its flow version was not live (5.1) |
| `confirmed_before_joining` | not consistent | A record's confirmation predates its joining |
| `flow_dates_inverted` | not consistent | A flow version was replaced before it went live |
| `denominator_inverted` | not consistent | The denominator's low end is above its high end |
| `claims_inverted` | not consistent | The represented claims' low end is above their high end |
| `residents_unstated` | not consistent | The annex leaves residents' opt-in to the action, and the export does not state it, or not for a record's subgroup (4.6) |
| `opt_in_terms_without_opt_in` | not consistent | The export states opt-in terms, and the action binds nobody on an opt-in |
| `term_channel_without_window` | not consistent | An opt-in term states a channel where the annex has no window, so the law names the channel (4.6) |
| `opt_in_term_inverted` | not consistent | An opt-in term closes before it opens |
| `unknown_subgroup` | not consistent | A term or the residents' opt-in names a subgroup the export does not declare |
| `parts_unstated` | not consistent | The export splits the claim into parts, and a record states none |
| `unknown_part` | not consistent | A record belongs to a part the export does not state |
| `anchored_before_reference_date` | not consistent | The anchor is dated before the reference date it fixes |
| `grade_differs` | not verified | A record states a grade its facts do not give |
| `digest_differs` | not verified | A record states a digest its canonical form does not give |
| `root_differs` | not verified | The anchored root is not the root of the records |
| `manifest_differs` | not verified | The anchored manifest is not the manifest of the export |
| `not_anchored` | registered | The manifest is not anchored (5.4) |
| `flow_not_captured` | registered | A flow version an active record names was not captured (5.1) |
| `residence_unsourced` | registered | A residence the opt-in turns on has no source (4.6) |
| `opt_in_names_other_action` | registered | An opt-in names the action otherwise than the court's reference (4.6) |
| `flow_without_digest` | identified | A captured flow version an active record names has no digest (5.1) |
| `terms_without_digest` | identified | A terms version an active record names has no digest (5.2) |
| `record_without_digest` | identified | A record has no digest (5.3) |
| `no_facets` | identified | The export declares no facets of the class (6.3) |
| `facet_value_undeclared` | identified | A counted record has no declared value for a facet (6.3) |
| `flow_not_witnessed` | verified | A flow version an active record names was not witnessed by a bailiff or notary (5.1) |
| `subgroups_undeclared` | verified | The export does not declare its subgroups, or that it has none (6.4) |
| `subgroup_undeclared` | verified | A counted record has no declared subgroup (6.4) |

## 12. Annexes

An annex follows `annexes/_template.md`: who may bring an action; who is bound and how they join; when the register is tested; the Required items, split into what the law requires and what this standard requires beyond it, each with its source or reason; the Recommended items; the identification schemes that count as recognised for grade A; the level a typical action needs; and what is unsettled.

## 13. Citing this standard

Cite the version, the core and the annex, with the version's own address: 'VCRS 0.1.0-beta.5, core and Annex NL, <https://vcrs.org/v/0.1.0-beta.5>'. A released version stays unchanged at that address, so a filing cites a text that does not change. A section is cited by its number after the address: https://vcrs.org/v/0.1.0-beta.5#4.6.

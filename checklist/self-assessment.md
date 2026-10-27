# Self-assessment

For the board of a representative, before it claims a level. Each line is a yes or a no; a no is the work left. Section numbers are the core's. The annex adds its own Required items after these.

## Level 1: Registered

| # | Question | Core |
|---:|---|---|
| 1 | Is the class definition written down, versioned, dated and approved by the board? | 3, 9 |
| 2 | Do we state the size of the class with its source, its method and its date, as a range where it is uncertain, and, where the claim is split into parts, the size of each part? | 4.6, 6.1 |
| 3 | Does every version of the sign-up flow state the representative, the defendant, the claim and the period before anyone joins? | 5.1 |
| 4 | Is every version of the sign-up flow captured in full, in every language, with the dates it was live? | 5.1 |
| 5 | Does every record name the flow version it joined through and the terms version the person accepted? | 5.1, 5.2 |
| 6 | Does every record we count hold a name, a date of birth (or a registration number for a legal person), and a contact channel the person confirmed? | 4.2 |
| 7 | Do we keep a deduplication key per record, and mark the later of two records for one person as the duplicate? | 4.5 |
| 8 | Are withdrawals, opt-outs and exclusions recorded with their date, and left out of the count? | 4.1 |
| 9 | Where the annex binds people abroad, residents or both only on an opt-in: does every record hold the person's residence and its source, where the opt-in turns on it, and, once the opt-in is due, does the record of everyone who has to opt in hold their opt-in and, where the annex asks, their declaration on parallel actions? | 4.6 |
| 10 | Is every change to a record logged: what, when, by whom, why? | 5.3 |
| 11 | At each reference date, do we fix the snapshot root and the manifest, and anchor the manifest in time? | 5.4 |
| 12 | Does the board commission an auditor, independent of the operator and the funder, who traces a sample from the register to the source records and back? | 8 |
| 13 | Do we own the register, can we export it complete at any time at no extra cost, its source records readable without the operator's systems in the form we fixed when the operator started, and can we replace the operator? | 9 |
| 14 | Does the operator's fee depend neither on the outcome nor on the number of records? | 9 |

## Level 2: Identified

All of Level 1, and:

| # | Question | Core |
|---:|---|---|
| 15 | Does every flow capture and every terms version carry a digest? | 5.1, 5.2 |
| 16 | Does every record carry a digest of its canonical form? | 5.3, 11.3 |
| 17 | Do we report how the records spread over the class's own facets, beside the class's spread where the source gives it? | 6.3 |
| 18 | Do we report how many records are grade B or better? | 10 |
| 19 | Do we regenerate the register at a reference date shortly before each hearing? | 7 |
| 20 | Does the auditor recompute every grade and the coverage at each grade from the source records? | 8 |

## Level 3: Verified

All of Level 2, and:

| # | Question | Core |
|---:|---|---|
| 21 | Did a bailiff or a notary witness every version of the sign-up flow? | 5.1 |
| 22 | Does every evidence document carry a digest the record names? | 5.3 |
| 23 | Do we report coverage per subgroup, each against a denominator of its own, or state that the class has none? | 6.4 |
| 24 | Do we report how many records are grade A? | 10 |
| 25 | Does the auditor run the reproduction test: read-only access to the live system, no export from the operator, every grade and the coverage recomputed, the snapshot root and the manifest matched, a test sign-up through each live flow version? | 8 |

## What a validator checks

A validator reading the facts export answers questions 3 to 9, 11 (the root and the manifest, and whether the manifest is anchored), 15 to 18, and 21 to 24. The rest the board answers, and the conformance statement attests.

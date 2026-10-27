# Changelog

## [Unreleased]

**Added**
- A denominator of its own for each subgroup and each part of a split claim (`denominator.subgroups`, `denominator.parts`; core 4.6, 6.4), with the coverage of each in the check's report and the conformance statement (`subgroups`, `parts`). A part without its size withholds every level (`part_without_denominator`), a subgroup without its denominator withholds Verified (`subgroup_without_denominator`), and a size for a subgroup or part the export does not declare, or one inverted, makes the export not consistent.
- A vector for an opt-in that names the action otherwise than the court's reference: the grade stands (`vectors/nl/c-abroad-opted-in-naming-another-action.json`).
- The conformance statement counts the records at grade C whose evidence does not establish class membership (`membership_not_established`, reason `class_not_established`), and core 11.2 asks for it.
- The conformance statement names the auditor's engagement (`auditor.engagement`: `agreed_upon_procedures` or `assurance`), and core 8 says what each gives.

**Changed**
- Core 1: what a court asks of a register, and when, differs per jurisdiction, and the annex says what role the register plays there.
- Core 4.1: why rule 6 asks a date of birth even where identity is verified.
- Core 4.6: in a split claim the opt-in governs its own part alone. A record in that part and in another is graded with it, and counts in the other part at the grade it holds there without the opt-in. A vector states such a record's grade per part (`expected.parts`, core 11.4), as `vectors/nl/d-abroad-in-the-wamca-part-not-opted-in.json` and a new one for an action outside the Directive do.
- Core 9: the open format of section 11 carries the facts that set each grade; the source records, the evidence, the flow captures and the change log go with them, complete and readable without the operator's systems, in a form the representative and the operator fix when the operator starts. The self-assessment's question 13 asks the same.
- Core 9: a fee that does not depend on the number of records is this standard's own condition, with its reason.
- Core 10: the annex recommends a level, and that recommendation is not a court's rule.
- Core 11.1 and the descriptions of the export and record schemas: the records keep pseudonymous identifiers, so the export is personal data for whoever can link them to the source records.
- The descriptions of `opt_in.action` and `action.court_reference` in the record and export schemas: an opt-in that names another action leaves the grade as it is and withholds every level, as core 11.6 says.
- The conformance statement says its figures describe the representative's register, not whom the law or the court treats as represented or bound.
- The self-assessment's question 2 asks for the size of each part of a split claim, and question 23 for each subgroup's denominator.
- Every annex quotation that was shortened with '(...)' quotes the publisher's text literally, as one passage or as separate passages joined by the annex's own words (Annexes AT, CZ, DE, IT, NL and PT). Annex NL-5 keeps the court's qualifier that the date of birth was asked on enrolment through SOMI's websites, and NL-4 says what the Hoge Raad faulted the Hof for.
- Each annex and the annex template say who wrote the annex and whether counsel admitted in its jurisdiction has reviewed it; GOVERNANCE says the same.
- Annex NL-9: the foundation supplies the figures in the writ, or at the latest in reply to an express defence, as Rb Noord-Holland 2025:8944 ro. 4.50 and 4.52 say.
- Annex NL-16: the export states the size of each part as `denominator.parts`, and a person in both parts counts in the `pre_wamca` part without the opt-in.

## [0.1.0-beta.4] - 2026-10-26

**Added**
- The manifest (core 5.4): the export without its anchor, its records replaced by their number and the snapshot root. Its digest is what is anchored, so the reference date, the annex, the action, the class, the denominator, the flow versions and the opt-in terms are fixed with the records.
- Core 11.6: the four outcomes of a check, kept apart (not valid, not consistent, not verified, and the level whose conditions hold), and a code for every finding, reported with its JSON pointer.
- For a legal person at grade A: its registration checked against the business register and the authority of the person acting for it, each dated (`identity.register_check`, `identity.authority`; reasons `register_not_checked` and `authority_not_checked`).
- A confirmation through a flow version that informs, beside the version the person joined through (`confirmed`; core 4.1 rule 2 and 5.1).
- Opt-in terms as a list (`opt_in_terms`), each with its days, its channel and the subgroups it applies to, so an opt-in made between two terms does not count; a deadline the law sets under an annex whose opt-in is due from the start; residents' opt-in per subgroup; the date a court fixes for the residence test (`residence_on`); the parts of a claim a transitional rule puts under two laws (`parts`), with the part an annex's opt-in governs (`opt_in_part` in the annex JSON).
- The day a record's status last changed (`status_on`), and an exclusion's reason (`status_reason`: `late`, `refused`, `defective`, `unpaid` or `ended`).
- The action an opt-in names (`opt_in.action`). An opt-in that names it otherwise than the court's reference withholds Registered (`opt_in_names_other_action`) and leaves the grade as it is.
- Every vector states its record's digest. New vectors cover legal persons, confirmations, facts dated after the reference date, Italy's two terms, a Belgian settlement that sets the option per category, the deadlines of Annexes AT, CZ and IE, split Dutch claims, a court's residence date, and strings that test the canonical form.
- The example package in `templates/`: the example register as one JSON export, its manifest, an inclusion proof that holds and one altered that does not, a draft statement, every outcome a check must give (`expected.json`), and the conformance statement filled in for it, its parties, its auditor and its timestamp fictional.

**Changed**
- The README says what VCRS is under a heading of its own, sets the grade of a record apart from the level the register as a whole claims, and links the governance, the changelog and the licence by name.
- GOVERNANCE.md names the text, the schemas and the vectors as free to use.
- The README and its banner say a register shows who stands behind the action, and that an independent auditor checks the count, which holds at every level.
- The README's summary puts a record without an opt-in the annex requires at grade D, and names for each level the grades it counts and the grade it reports, as core 10 does.
- The conformance statement sets active records at grade D apart from records not active, which are grade D too, and says how its rows add up.
- The example register's represented claims are €31 500 000 to €39 000 000, as its method gives.
- The self-assessment's question 9 covers residents the annex binds on an opt-in, as core 4.1 rule 8 and 4.6 do.
- The declaration of core 4.6 is the declaration on parallel actions in the template, the annexes and the vectors.
- Core 7: a register regenerated before a hearing holds every withdrawal, opt-out and exclusion up to its reference date.
- Annex AT: no entity is admitted ad hoc for a single action, and the OGH rejected both appeals in provisional-measures proceedings as inadmissible.
- Annex CZ: the court examines admissibility at any stage of the proceedings (§ 24 odst. 1), and checks the plaintiff's listing of its own motion.
- Annex DE: the BayObLG tests similarity against the proof of entitlement, and signing up with the representative is no condition of the opt-in.
- Annex FI: an electronic notice meets the written form without a signature where the Kuluttaja-asiamies is the claimant.
- Annex NL: a count or a figure one court worked from is attributed to that court.
- Annex PT: associations and foundations must meet LAP art. 3, and the TCRS recorded the point on jurisdiction as undisputed.
- Wording across the core, the self-assessment, the annex template, the schema descriptions and every annex, for precision.
- A record is graded as it stood on the reference date: a verification, a check, a confirmation, an opt-in or a change of status dated after it does not count (core 4, 4.1, 7).
- Core 4.5: a duplicate's original is the record that joined first or, on the same day, the one whose identifier comes first in byte order; a duplicate never names itself, nor another duplicate.
- Core 5.1: a record's flow version was live on the day it joined.
- Core 6.2: coverage is a percentage rounded half up to four decimals.
- Core 11.3: an export is read as I-JSON, so a member name that appears twice in one object makes it invalid; numbers are written as RFC 8785 writes them; an optional member that holds nothing is left out, never written as null.
- Core 8 and the self-assessment: the auditor confirms the manifest beside the snapshot root, and the report names its digest.
- The anchor anchors the manifest, on or after the reference date (`anchor.manifest`). The conformance statement states the manifest's digest and whether it is a draft (`draft`).
- Annex NL asks the declaration on parallel actions only in an action under the Directive (`parallel_declaration`: `directive`).
- Four Annex NL vectors describe their person as resident in Belgium, as their records hold.
- Annex NL: a claim on events on both sides of 15 November 2016 is split, the events being the facts pleaded, per claim and per defendant (HR 2026:1551 ro. 3.2.4, 3.2.5 and 3.3.3). Only a series of events so intertwined that they cannot be separated goes to the law in force at the last of them (ro. 3.2.7), and the earlier part claims no damages in money (art. 3:305a lid 3 BW as in force until 31 December 2019). NL-16 asks class size and coverage per part, and a record states its parts (`parts`: `pre_wamca`, `wamca`); the opt-in binds the WAMCA part alone.
- Annex NL: the declaration of art. 1018f lid 6 Rv applies to claims filed on or after 25 June 2023 (art. VI Implementatiewet richtlijn representatieve vorderingen voor consumenten).
- Annex NL, NL-15: a court may fix the date the residence test of art. 1018f lid 5 Rv looks at (Rb Amsterdam 1 May 2024, ECLI:NL:RBAMS:2024:2479, ro. 3.9), which the export states as `residence_on`.
- Annex NL, NL-14: the operator is paid a reasonable, commercial fee that does not depend on the outcome (Hof Den Haag 2025:2738 ro. 6.81).
- Annex NL: an opt-out can be made through a representative (ECLI:NL:RBAMS:2024:2479 ro. 3.16); NL-11 cites the same ruling's ro. 3.21 for the channel a court sets; the court of appeal tests as things stand at its decision (HR 2026:1198 ro. 3.2.2 and 3.2.4); the distribution row cites art. 1018k Rv.

**Migrating an export from 0.1.0-beta.3**
- Replace `opt_in_opened_on`, `opt_in_closed_on` and `opt_in_channel` with `opt_in_terms`: one term with those days and that channel, or none where no window was set.
- Give every record that is not active its `status_on`, and every opt-in its `action`.
- Give every residence the opt-in turns on its `source`.
- Leave out an optional member that holds nothing: `court_reference` and `opt_in` are never null.
- For a legal person at grade A, add `register_check` and `authority`.
- Compute every record's digest, the root and the manifest again, and anchor the manifest.

## [0.1.0-beta.3] - 2026-10-22

**Changed**
- The standard's address is vcrs.org: the citation and the addresses in core 13, each schema's `$id` and the README. 0.1.0-beta.1 and 0.1.0-beta.2 keep the addresses they were released under.

## [0.1.0-beta.2] - 2026-10-21

**Added**
- Annex AT (Verbandsklage auf Abhilfe), each Required item cited to its article or ruling.
- Annex DE (Verbandsklage under the VDuG), each Required item cited to its article or ruling.
- Annex BE (action en réparation collective), each Required item cited to its article or ruling.
- Annex IT (azione di classe and azione rappresentativa), each Required item cited to its article or ruling.
- Annex IE (representative action under the 2023 Act), each Required item cited to its section, rule or ruling.
- Annex FI (ryhmäkanne under the ryhmäkannelaki), each Required item cited to its section.
- Annex PL (postępowanie grupowe), each Required item cited to its article or ruling.
- Annex CZ (hromadné řízení), each Required item cited to its section or ruling.
- The facts export states whether residents opt in in this action (`opt_in_residents`), where the annex leaves it to the court or an approved agreement (`"action"`).
- The facts export and the conformance statement state whether the action is brought under the forum's transposition of Directive (EU) 2020/1828 (`action.directive`, core 4.6 and 11.1). An annex may set `opt_in_abroad` to `"directive"`: people abroad then opt in only in such an action.

**Changed**
- Under an annex without an opt-in window, the facts export states no window and no channel (`opt_in_opened_on`, `opt_in_closed_on`, `opt_in_channel`); an export that states either meets no level (core 4.6).
- The opt-in rule (core 4.1 rule 8, 4.6) also binds residents of the forum where the annex sets `opt_in_residents`; where both opt in, residence decides nothing. The annex key `parallel_declaration_abroad` is `parallel_declaration`, and the declaration goes with every opt-in.
- Annex PT binds people abroad on an opt-in only in an action under Decreto-Lei n.º 114-A/2023, which covers actions on the provisions in Annex I of the Directive filed from 6 December 2023, and states the unclaimed-sums rule per regime.
- Annex NL states the transitional rule: a claim covering events before and on or after 15 November 2016 is split, and the WAMCA and titel 14A Rv govern the later part (art. 119a Overgangswet nieuw Burgerlijk Wetboek; HR 2026:1551). NL-16 asks for class size and coverage per part.
- Annex NL: after the appointment the court may re-test admissibility and need not supervise; NL-14's safe harbour covers outsourcing alone and asks for no tie through the board or a shareholding; NL-15 holds residence on the date the court fixes the class.

## [0.1.0-beta.1] - 2026-10-20

The first draft for consultation: a core that holds in every jurisdiction, and annexes that hold what one jurisdiction's law requires.

**Added**
- The core: grades A to D set by fixed rules, residence and opt-in from abroad, provenance, coverage against a stated denominator, the represented claims, the reference date, the independent check per level, the representative's control, three levels (Registered, Identified, Verified), the open format.
- Annex NL (WAMCA) and Annex PT (ação popular and DL 114-A/2023), each Required item cited to its article or ruling.
- JSON Schemas for the facts export, one record, and the conformance statement.
- Test vectors for the core and each annex.
- The self-assessment, a spreadsheet template and a conformance statement template.

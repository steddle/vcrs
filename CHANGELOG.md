# Changelog

## [Unreleased]

**Added**
- An example conformance statement, `templates/conformance-statement-example.md`: the template filled in for the example register, its parties and its auditor fictional, with the same statement as JSON.

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
- Wording across the core, the self-assessment, the annex template, the schema descriptions and every annex, for precision. No grade rule or level condition changes.

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

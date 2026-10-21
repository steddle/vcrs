# Changelog

## [Unreleased]

**Added**
- Annex AT (Verbandsklage auf Abhilfe), each Required item cited to its article or ruling.
- Annex DE (Verbandsklage under the VDuG), each Required item cited to its article or ruling.
- Annex BE (action en réparation collective), each Required item cited to its article or ruling.
- Annex IT (azione di classe and azione rappresentativa), each Required item cited to its article or ruling.
- The facts export states whether residents opt in in this action (`opt_in_residents`), where the annex leaves it to the court or an approved agreement (`"action"`).
- The facts export and the conformance statement state whether the action is brought under the forum's transposition of Directive (EU) 2020/1828 (`action.directive`, core 4.6 and 11.1). An annex may set `opt_in_abroad` to `"directive"`: people abroad then opt in only in such an action.

**Changed**
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

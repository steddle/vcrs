# Annex IE: Ireland (representative action under the 2023 Act)

VCRS 0.1.0-beta.5. Draft for consultation. Not legal advice. Law and rulings as read on 19 and 21 October 2026 on the electronic Irish Statute Book, the Courts Service's judgments, the British and Irish Legal Information Institute, the Department of Enterprise, Tourism and Employment's register of qualified entities and the European Commission's overview of notified eID schemes.

## 1. The regime

A collective damages action is a representative action for redress measures under the Representative Actions for the Protection of the Collective Interests of Consumers Act 2023 (No. 22 of 2023), in force since 30 April 2024 (S.I. No. 181/2024). It reaches actions and infringements from the Directive's date of application: the Act 'applies to representative actions brought on or after 25 June 2023 in respect of infringements by traders occurring on or after that date that harm or may harm the collective interests of consumers' (s. 5(1)). An infringement is 'an infringement of a relevant enactment' (s. 2(1)): the European acts and provisions specified in Annex I to the Directive, the Acts, provisions and statutory instruments the Schedule lists, and instruments made under the Acts in its Part 1. A claim on other law has no representative action for redress under the Act. In proceedings commenced from 12 October 2026, Order 15, rules 40 to 46 of the Rules of the Superior Courts set the procedure: 'These Rules shall apply in proceedings commenced from the date on which these Rules come into operation' (S.I. No. 488/2026, r. 2).

- **Who may sue.** Only a qualified entity (QE): 'A representative action may only be brought before the Court by a qualified entity' (s. 19(1)), and in it 'a qualified entity shall be the plaintiff' (s. 19(8)). The Minister designates a QE on the criteria of s. 8(1), among them that it 'can demonstrate in the application 12 months of actual public activity in the protection of consumer interests prior to the application' (s. 8(1)(a)), so there is no entity formed for one action. A QE designated in another Member State sues on the Commission's list (s. 19(3)).
- **Court.** The High Court (s. 2(1)).
- **No number and no similarity test.** The QE gives the court 'the class or classes of consumers affected by the alleged infringement' (s. 19(10)(c)) and 'sufficient information regarding the consumers referred to in subsection (10)(c) in order that the Court may assess the admissibility of the representative action concerned' (s. 19(11)).
- **Funding.** The Act admits third-party funding only 'insofar as permitted in accordance with law' (s. 27(1)), and the Supreme Court held that 'third party funding to support a plaintiff (where none of the exceptions apply) is unlawful by reason of the rules on champerty' (Persona Digital Telephony Ltd v Minister for Public Enterprise [2017] IESC 27, Denham C.J., para. 54(ix)).

## 2. Who is bound, and how they join

- **Opt-in, for everyone who may join.** 'A consumer who has not notified the qualified entity in accordance with this section shall not be represented by the qualified entity in the representative action and shall not be entitled to benefit from the redress measures granted by the Court in respect of that representative action' (s. 24(4)). Those who may notify are consumers 'ordinarily resident in the State or habitually resident in another Member State' (s. 24(1)), so residents and people in other Member States both opt in: `ie.json` sets `opt_in_abroad` and `opt_in_residents` to true, names the QE as the channel, `qe`, and asks every opt-in for the declaration on parallel claims (core 4.6). A person resident outside the Member States cannot notify and is outside the class the QE may represent. The export states no opt-in window: the opt-in is due from the start, so a record counts once the person's notification has reached the QE.
- **Joining, by notice to the QE.** The consumer 'shall so notify the qualified entity concerned in the prescribed manner' (s. 24(1)), on Form 3: 'The form set out in Part 3 of the Schedule is prescribed for the purposes of section 24(1) of the Act of 2023' (S.I. No. 182/2024, reg. 5). Form 3 holds the consumer's name, address, Eircode or postcode, phone and email, the trader, the infringement and how the consumer was affected, a signature and a date, and 'This form can be made available in an interactive digital format and completed electronically.' It holds no date of birth, which core 4.1 (6) asks of every natural person, so the register collects one with the notification.
- **The deadline.** 'A consumer referred to in subsection (1) may notify the qualified entity at any time until the case has been deemed admissible by the Court in accordance with section 19' (s. 24(2)). Nobody joins after admissibility, or after judgment.
- **The declaration.** A consumer who has notified 'shall sign a declaration provided to him or her by the qualified entity', confirming 'that he or she has not previously received compensation from the same trader for the same cause of action' and that compensation here precludes any other (s. 25(1)). Without it the consumer 'shall be precluded from benefiting from any redress measures under section 26 in the representative action concerned' (s. 25(3)).
- **The fee.** The QE may charge 'a modest fee' (s. 29(1)), published with its period on the QE's website (s. 29(2)), of at most €25 (S.I. No. 183/2024, reg. 2). 'Where a consumer fails, neglects or refuses to pay the entry fee within the time specified by the qualified entity in accordance with subsection (2), the consumer shall not be represented by the qualified entity in the representative action' (s. 29(3)).
- **The effect.** A consumer who notified and paid 'shall not be represented in any other representative action with the same cause of action against the same trader' and 'may not bring an action individually with the same cause of action against the same trader' (s. 24(7)(b), (c)).
- **Withdrawal.** By the prescribed form to the QE, at any time: 'Where a consumer no longer seeks to be represented by the qualified entity in any representative action for redress, he or she shall notify the qualified entity in the prescribed manner' (s. 24(5)), and 'A qualified entity shall inform the Court of any notification made by a consumer in accordance with subsection (5).' (s. 24(6)).
- **Who holds the list.** The QE. No court registry or state portal takes notifications. The QE lodges the list in court and hands the trader the names (section 3).

## 3. When the register is tested

| Stage | What it asks of the register | Source |
|---|---|---|
| Before admissibility | A signed, dated Form 3 per consumer, reaching the QE; the signed declaration; the fee paid within the published period | s. 24(1), (2); s. 25(1); s. 29(2), (3) |
| Admissibility | The class or classes affected and sufficient information about the consumers. In proceedings commenced from 12 October 2026, by motion on notice to the defendant, with a list of the names or other unique identifiers of the consumers who notified, lodged in court as near the hearing as practicable and copied to the defendant | s. 19(10)(c), (11); O. 15 r. 42(1), (2)(b), r. 43(1); ICCL v Microsoft [2026] IEHC 640, paras. 121 and 122 |
| After admissibility | Each notified consumer told of the determination; the trader handed the names of those who notified and signed the declaration | s. 24(3); s. 25(4)(a) |
| Withdrawal | The QE informs the court, by an updated list and a list of those who withdrew, copied to the defendant | s. 24(5), (6); O. 15 r. 43(2) |
| Trial | An updated list, lodged and delivered as near the trial as practicable | O. 15 r. 43(3) |
| Judgment | The class or classes entitled to the redress measures; where the order names no individual consumers, the class or classes in it; the period within which each consumer claims | s. 26(4), (7), (8) |
| Settlement | Binds 'the individual consumers represented in the representative action concerned'; where it names none, how the redress reaches each class | s. 30(3); O. 15 r. 46(b) |
| Distribution | The names of those eligible for redress who have not obtained compensation by other means; no consumer compensated twice; each represented consumer told how to benefit | s. 25(4)(b); s. 26(3), (5) |

**Reference dates.** The day the court deems the action admissible closes joining (s. 24(2)); the list is lodged 'as nearly as practicable prior to the hearing of an application under rule 42' (O. 15 r. 43(1)), and again before trial. For distribution, the day the QE hands the trader the list of those eligible (s. 25(4)(b)). The one judgment under the Act read concerns an action for an injunction alone: 'ICCL does not seek any redress measures in this action.' (ICCL v Microsoft, para. 25).

## 4. Required items

A register that claims a level in an Irish action meets every item below. The first table holds what Irish law requires, by statute or a court's holding. The second holds what this standard requires beyond the law, with the reason.

### What the law requires

| # | Item | Core | Source |
|---|---|---|---|
| IE-1 | Each record holds its opt-in: the day the person's Form 3 notification reached the QE, through the channel `qe`, signed and dated, with the trader, the infringement and how the person was affected. A notification made after the court deemed the action admissible is recorded `excluded` (core 4.1 (1)) | 4.1 (1), 4.6, 5.1 | s. 24(1): the consumer 'shall so notify the qualified entity concerned in the prescribed manner'; s. 24(2): 'A consumer referred to in subsection (1) may notify the qualified entity at any time until the case has been deemed admissible by the Court in accordance with section 19'; s. 24(4); S.I. No. 182/2024, reg. 5 and Form 3 |
| IE-2 | Each record holds the person's residence. A person resident neither in the State nor in another Member State cannot notify, and the record states `in_class` false: the class the export states carries that limit | 4.1 (4), 4.6 | s. 24(1): 'A consumer who is ordinarily resident in the State or habitually resident in another Member State' |
| IE-3 | Each record holds the declaration the person signed under s. 25, with its date. With the statement IE-10 adds, it is held as `parallel_declared` | 4.1 (8), 4.6 | s. 25(1): the declaration 'shall confirm' (a) 'that he or she has not previously received compensation from the same trader for the same cause of action' and (b) 'that he or she has been informed that receiving compensation in relation to this representative action concerned will preclude him or her from receiving any other compensation from the same trader for the same cause of action'; s. 25(3): without it the consumer 'shall be precluded from benefiting from any redress measures under section 26 in the representative action concerned' |
| IE-4 | Where the QE charges an entry fee, the amount, no more than €25, and the day it was paid within the period the QE published. A person who did not pay in time is recorded `excluded` | 4.1 (1), 9 | s. 29(2): the QE 'shall specify on its website the amount of the fee and the time period within which the fee charged in accordance with subsection (1) shall be paid'; s. 29(3): 'the consumer shall not be represented by the qualified entity in the representative action'; S.I. No. 183/2024, reg. 2: 'A fee of €25 is prescribed' |
| IE-5 | A withdrawal is recorded `withdrawn` with its date, and the day the QE informed the court | 4.1 (1), 5.3 | s. 24(5); s. 24(6): 'A qualified entity shall inform the Court of any notification made by a consumer in accordance with subsection (5).'; O. 15 r. 43(2) |
| IE-6 | A list of the names or other unique identifiers of the consumers who notified, produced before the admissibility hearing, on each withdrawal and before trial. Each version is kept with the day it was lodged and the snapshot root of that day | 5.4, 7 | O. 15 r. 43(1): the QE shall 'lodge in Court a list of the names or other unique identifiers of the consumers who have requested to be represented by that qualified entity in the representative action concerned, and deliver a copy of that list to the defendant'; r. 43(3): 'each qualified entity concerned shall lodge and deliver an updated list as nearly as practicable prior to the commencement of the trial' |
| IE-7 | Each record holds the class or classes the person belongs to, so the QE can describe them to the court before admissibility and at judgment | 6.1, 6.4 | s. 19(10)(c), (11); ICCL v Microsoft [2026] IEHC 640, para. 122: the information 'must, of necessity, be required to be furnished prior to the court deciding the issue of admissibility'; s. 26(4): the QE 'shall gather, and provide the Court with, information concerning the class or classes of consumers entitled to benefit from redress measures ordered in the representative action concerned' |
| IE-8 | The names the trader receives: at admissibility, those who notified and signed the declaration; at the end, those eligible for redress. Each record holds whether the person obtained compensation by other means for the same cause | 4.6, 6.5 | s. 25(4)(a): 'a list of the names of the consumers who have notified their request to be represented in the representative action and have signed a declaration'; s. 25(4)(b): 'a list of the names of the consumers who are eligible to receive redress where such consumers have not obtained compensation through other means for the same cause of action'; s. 26(3): 'A consumer shall not be entitled to receive compensation more than once arising from the same cause of action against the same trader.' |
| IE-9 | A contact channel per person that reaches them with the admissibility determination, the redress ordered and the dates that stop and restart the limitation period | 4.1 (7) | s. 24(3); s. 26(5); s. 28(2): 'the qualified entity shall inform consumers represented by a representative action in writing of the following dates' |

### What this standard requires

| # | Item | Core | Reason |
|---|---|---|---|
| IE-10 | The declaration the QE provides under s. 25 also states that the person is not represented, and does not claim, elsewhere on the same cause of action against the same trader | 4.1 (8), 4.6 | s. 25 asks about compensation received, not about another action. A consumer who notified 'shall not be represented in any other representative action with the same cause of action against the same trader' (s. 24(7)(b)), and nobody is represented twice on the same claim (Directive (EU) 2020/1828, art. 9(4)). `parallel_declaration` applies to every opt-in, so the validator asks it of all |

## 5. Recommended items

- **Evidence that each person was affected.** The Act asks for none, but whether the class information suffices 'is clearly a matter of disputed fact' (ICCL v Microsoft, para. 113), and the consumers affected 'may well give rise to issues in dispute in proceedings where the provision of discovery will be both relevant and necessary' (para. 131).
- **A last list lodged right before the order.** Joining stays open until the court deems the action admissible (s. 24(2)), so notifications keep arriving after the list of O. 15 r. 43(1).
- **Names beside identifiers.** The court list may hold identifiers alone (O. 15 r. 43(1)), but the trader receives names at admissibility (s. 25(4)(a)), so the register keeps both from the start.
- **Identity verification.** It protects the declaration and the list of those eligible at the end against challenge.
- **The cost of the register in the financial overview.** The QE 'shall disclose to the Court a financial overview that specifies the sources of funds used by it to support the representative action' (s. 27(3)), and the register is paid from the QE's own funds and the fees.
- **An operator receiving notifications for the QE.** Each Form 3 is addressed to the QE by name, at a channel the QE publishes as its own; the operator receives it as the QE's processor under a written mandate to receive; the opt-in's day is the day the QE had it, and the register keeps the day the operator received it. A notification counts as made before the action is deemed admissible only where the QE had it in time (s. 24(2)). This lowers the risk of the question section 8 leaves open; it does not settle it.

## 6. Recognised identification

- **Identity, grade A**: no Irish electronic identification scheme is notified under eIDAS (the European Commission's overview of notified schemes, last updated 2 February 2026). A means another Member State notified at substantial or high counts under `eidas`; `ie.json` names no further scheme.
- **Outside sources, grade B**: none named. No Irish ruling has yet examined evidence of membership.

## 7. The level a typical action needs

A recommendation, not a court's rule.

- **Level 2, Identified.** The law asks for a named, signed and dated notification per consumer, the declaration and the fee, a list lodged in court and names handed to the trader, and no proof of identity or of the claim. A register at grade C with the Form 3 fields answers it.
- **Level 3, Verified, for the list of those eligible at the end** (s. 25(4)(b)), where the QE states who has not been compensated elsewhere, and wherever the defendant contests the class information (ICCL v Microsoft, paras. 113 and 131).

## 8. Unsettled

- No action for redress under the Act had reached a written judgment by 21 October 2026, so no court has yet tested a list of notified consumers.
- Whether the declaration under s. 25, which confirms compensation not received, is the declaration on parallel actions core 4.6 asks for. IE-10 adds representation elsewhere so that `parallel_declared` holds both.
- Whether the list lodged under O. 15 r. 43 may hold identifiers alone while s. 25(4) sends names to the trader.
- Whether a notification an operator receives for the QE is a notification to the QE (s. 24(1)): no source read addresses an agent. Whether a vendor paid a fixed fee by the QE to run the register is caught by the rules on champerty: no court has said, and the Law Reform Commission's report on third-party litigation funding was not published by 21 October 2026.
- The opt-in is due from the start. The export states the period up to the day the court deemed the action admissible as a term (`opt_in_terms`), and the validator does not count a notification dated after it. IE-1 also records a late one `excluded`, and the auditor checks it.
- Proceedings commenced before 12 October 2026 run without O. 15 Part V. In ICCL v Microsoft the High Court deemed the action admissible on an ex parte application before the summons issued (para. 15).

## Sources

1. Representative Actions for the Protection of the Collective Interests of Consumers Act 2023 (No. 22 of 2023), electronic Irish Statute Book, Office of the Attorney General: https://www.irishstatutebook.ie/eli/2023/act/22/enacted/en/print
2. S.I. No. 181/2024, Commencement Order 2024: https://www.irishstatutebook.ie/eli/2024/si/181/made/en/print
3. S.I. No. 182/2024, Prescribed Forms Regulations 2024 (Forms 3 and 5): https://www.irishstatutebook.ie/eli/2024/si/182/made/en/print
4. S.I. No. 183/2024, (Section 29) (Maximum Fee) Regulations 2024: https://www.irishstatutebook.ie/eli/2024/si/183/made/en/print
5. S.I. No. 488/2026, Rules of the Superior Courts (Representative Actions for the Protection of the Collective Interests of Consumers Act 2023) 2026: https://www.irishstatutebook.ie/eli/2026/si/488/made/en/print
6. Irish Council for Civil Liberties CLG v Microsoft Ireland Operations Ltd [2026] IEHC 640, High Court, 25 September 2026, Courts Service: https://www2.courts.ie/acc/alfresco/17894922-c4e5-4385-a1fb-749059120aa1/2026_IEHC_640.pdf/pdf
7. Persona Digital Telephony Ltd v Minister for Public Enterprise [2017] IESC 27, Supreme Court, 23 May 2017, British and Irish Legal Information Institute: https://www.bailii.org/ie/cases/IESC/2017/S27.html
8. Register of Qualified Entities, Department of Enterprise, Tourism and Employment: https://enterprise.gov.ie/en/publications/raa-register-of-qualified-entities.html
9. Third Party Litigation Funding, project page, Law Reform Commission: https://www.lawreform.ie/third-party-litigation-funding/
10. Overview of pre-notified and notified eID schemes under eIDAS, European Commission: https://ec.europa.eu/digital-building-blocks/sites/display/EIDCOMMUNITY/Overview+of+pre-notified+and+notified+eID+schemes+under+eIDAS

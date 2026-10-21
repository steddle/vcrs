# Annex CZ: Czech Republic (hromadné řízení)

VCRS 0.1.0-beta.2. Draft for consultation. Not legal advice. Law and rulings as read on 19 and 21 October 2026 in the Sbírka zákonů (e-Sbírka), the Ministerstvo spravedlnosti's rejstřík hromadných řízení and the Městský soud v Praze's documents published in it, the Ministerstvo průmyslu a obchodu's list of authorised persons and the European Commission's overview of notified eID schemes.

## 1. The regime

A collective damages action is a hromadná žaloba under the zákon č. 179/2024 Sb., o hromadném občanském řízení soudním, in force since 1 July 2024, which transposes Directive (EU) 2020/1828 and applies to disputes between consumers and a trader (§ 4). 'Podle tohoto zákona lze projednat a rozhodnout spory o práva nebo oprávněné zájmy, které vznikly po dni 24. listopadu 2020.' (§ 92 odst. 1).

- **Who may sue.** 'Žalobcem v hromadném řízení může být pouze právnická osoba, která je zapsána do seznamu oprávněných osob podle zákona o ochraně spotřebitele, nebo společně více takovýchto osob.' (§ 8 odst. 1). The Ministerstvo průmyslu a obchodu keeps the Czech list, and an entity enters it only after it 'aktivně působí v oblasti ochrany zájmů spotřebitelů po dobu alespoň 12 měsíců' (§ 25a odst. 1 písm. b) zákona č. 634/1992 Sb.), so there is no entity formed for one action. The plaintiff 'musí být v hromadném řízení zastoupen advokátem' (§ 14).
- **Admissibility.** 'Hromadná žaloba je přípustná, jestliže (...) c) skupina má alespoň 10 členů, d) tvrzená práva nebo oprávněné zájmy členů skupiny jsou založeny na podobném skutkovém a právním základu' (§ 15). The court examines these when the defendant raises them, the plaintiff's listing apart (Městský soud v Praze, 11 February 2025, 3 C 10/2024-10, para. 18), and at any later stage: 'Podmínky přípustnosti hromadné žaloby soud zkoumá kdykoliv v průběhu hromadného řízení ve věci samé.' (§ 24 odst. 1).
- **The court.** Both actions admitted by 21 October 2026 were heard by the Městský soud v Praze.

## 2. Who is bound, and how they join

- **Opt-in, for everyone.** A participating member is a 'člen skupiny, který se do hromadného řízení stanoveným způsobem přihlásil' (§ 2 odst. 1 písm. d)), and 'Výrok pravomocného rozsudku vydaného v hromadném řízení je závazný pro všechny zúčastněné členy skupiny ke dni vydání rozhodnutí.' (§ 70 odst. 4). The act draws no line by residence, and the court sets publication to reach 'všech členů skupiny včetně případných členů skupiny, kteří nemají obvyklý pobyt na území České republiky' (§ 84 odst. 2), so residents and people abroad both opt in: `cz.json` sets `opt_in_abroad` and `opt_in_residents` to true and asks no declaration on parallel claims, which the act does not know.
- **The přihláška.** 'Přihláška se činí oznámením učiněným u žalobce, a to s využitím formuláře, který Ministerstvo spravedlnosti (dále jen „ministerstvo“) uveřejní způsobem umožňujícím dálkový přístup.' (§ 32 odst. 1). 'Z přihlášky musí být patrno, kdo ji činí, kterého hromadného řízení se týká, čeho se člen skupiny po žalovaném v rozsahu vymezeném žalobcem v hromadné žalobě domáhá, a musí být podepsána a datována.' (§ 33 odst. 1). Filed electronically, 'může být náležitost podpisu splněna jakýmkoliv způsobem, se kterým jiný právní předpis spojuje účinky vlastnoručního podpisu' (vyhláška č. 181/2024 Sb., § 5); the form the Městský soud v Praze published for 3 C 3/2026 names a send from the member's datová schránka or a qualified electronic signature. A sign-up on a website, confirmed by mail or a tick box, is no valid přihláška. Where it was made as a notice of joining, it is one not on the form or unsigned, and the plaintiff asks for a correction within a reasonable time (§ 34 odst. 1).
- **Two channels.** The přihláška goes to the plaintiff, or to the court: 'Přihláška je učiněna řádně také tehdy, pokud je ve lhůtě pro přihlašování podána k soudu, který vede hromadné řízení v prvním stupni.' (§ 32 odst. 2). `cz.json` names no single channel; each record states its own, `plaintiff` or `court` (CZ-2).
- **The period.** 'Člen skupiny se může do hromadného řízení přihlásit od zahájení hromadného řízení podáním hromadné žaloby do uplynutí lhůty pro přihlašování přihláškou.' (§ 31 odst. 1), and 'Za přihlášku se považuje i udělení písemného souhlasu se zahájením hromadného řízení před podáním hromadné žaloby' (§ 31 odst. 2). The admissibility ruling sets the deadline, 'alespoň 2 měsíce, nejvýše však 4 měsíce od uveřejnění pravomocného usnesení o přípustnosti hromadné žaloby v rejstříku hromadných řízení' (§ 18 odst. 1 písm. d)). People join from before filing to that deadline, so the export states no opt-in window: the opt-in is due from the start, and a record counts once it holds a signed přihláška.
- **Defects.** The plaintiff asks for a correction where the form or the content of § 33 is missing (§ 34 odst. 1), and 'K přihlášce, která nebyla podána za podmínek podle § 31 nebo 32 nebo která nebyla na výzvu žalobce opravena, se nepřihlíží.' (§ 34 odst. 2). A přihláška that claims more than the action seeks, left uncorrected, is disregarded only 'v rozsahu, ve kterém překračuje předmět hromadného řízení' (§ 35 odst. 2).
- **Withdrawal.** In whole or in part, on the ministry's form, until the deadline; 'Jinak se ke zpětvzetí přihlášky nepřihlíží.' (§ 36).
- **Effect.** 'Přihlášení do hromadného řízení brání tomu, aby právo nebo oprávněný zájem zúčastněného člena skupiny s podobným skutkovým a právním základem v rozsahu vymezeném v přihlášce mohly být uplatněny v jiném řízení.' (§ 37 odst. 2). A member who sued alone first may join, and the přihláška then names that action (§ 28 odst. 2, § 33 odst. 3).
- **Who holds the list.** The plaintiff: 'Žalobce vytvoří seznam zúčastněných členů skupiny, do kterého zapisuje identifikační údaje o každém členovi skupiny, který se do hromadného řízení přihlásil, s uvedením, čeho se tento člen skupiny po žalovaném domáhá.' (§ 38 odst. 1).

## 3. When the register is tested

| Stage | What it asks of the register | Source |
|---|---|---|
| Filing | The conditions of membership, the facts behind § 15, the amount per member or how it is computed; the written consents given before filing, attached | § 13 odst. 1 písm. b), § 13 odst. 2; § 31 odst. 2 |
| Admissibility | At least 10 members of the group, both rulings read taking them from přihlášky already collected; claims on a similar factual and legal basis | § 15 písm. c), d); 3 C 10/2024-10, paras. 9 and 21; 3 C 3/2026, paras. 11 and 23 |
| Joining | Signed přihlášky on the ministry's form, to the plaintiff or the court, until the deadline; a correction asked where one is defective | § 18 odst. 1 písm. d); §§ 31 to 36 |
| The list | After the deadline, the list and every přihláška to the court, and the list to the parties; fewer than 10 on it stops the action | § 38 odst. 2, 3; § 39 odst. 1 |
| Exclusion | Within one month, on the plaintiff's motion, the court strikes a person whose membership is not at least probable | § 40, § 41 |
| Judgment | The list is the judgment's annex: every participating member, whether their claim succeeds, and what each receives | § 70 odst. 1, 2 |
| Payment | The defendant pays each member named in the annex, within the time the judgment sets | § 70 odst. 1 písm. b); vyhláška č. 181/2024 Sb., § 2 odst. 1 písm. e) |

**Reference dates.** The day of the admissibility ruling for the count of 10. The last day of the joining period for the list (§ 38 odst. 2), as amended by any exclusion (§ 41). The judgment binds 'ke dni vydání rozhodnutí' (§ 70 odst. 4).

## 4. Required items

A register that claims a level in a Czech action meets every item below. They hold what Czech law requires, by statute, decree or a court's holding.

### What the law requires

| # | Item | Core | Source |
|---|---|---|---|
| CZ-1 | At the admissibility ruling, facts showing at least 10 members of the group with claims on a similar factual and legal basis; both rulings read took them from přihlášky already collected. After the deadline, at least 10 participating members on the list | 6.2, 6.4 | § 15 písm. c): 'skupina má alespoň 10 členů'; Městský soud v Praze, 11 February 2025, 3 C 10/2024-10, para. 21: 'existuje přinejmenším 19 osob, kteří jsou tvrzenými nositeli nároků'; § 39 odst. 1: 'Je-li na předloženém seznamu zúčastněných členů skupiny zapsáno méně než 10 přihlášených členů skupiny, soud hromadné řízení zastaví.' |
| CZ-2 | Each record holds its opt-in: the signed and dated přihláška on the ministry's form, the day it was made and its channel, `plaintiff` or `court`. A written consent given before filing counts. A sign-up without a signature that § 5 of the decree accepts holds no opt-in until corrected; the record keeps the request and its deadline (CZ-4) | 4.1 (8), 4.6, 5.1, 5.3 | § 32 odst. 1 and 2; § 33 odst. 1: 'a musí být podepsána a datována'; § 31 odst. 2; vyhláška č. 181/2024 Sb., § 5: 'může být náležitost podpisu splněna jakýmkoliv způsobem, se kterým jiný právní předpis spojuje účinky vlastnoručního podpisu' |
| CZ-3 | Each přihláška states who makes it, which action, what is claimed, and the facts and evidence that make membership credible; it holds the member's bank account, and the e-mail or datová schránka where the member has one | 4.3, 6.5 | § 33 odst. 2: 'Přihláška musí obsahovat též skutková tvrzení a důkazy osvědčující, že člen skupiny, který se do hromadného řízení přihlašuje, splňuje předpoklady členství ve skupině.'; vyhláška č. 181/2024 Sb., § 2 odst. 1 písm. c), e) |
| CZ-4 | A přihláška made after the deadline, or left uncorrected after the plaintiff's request, is recorded `excluded`. One that claims more or other than the action seeks, left uncorrected, counts for the part within the action; only one wholly outside it is recorded `excluded`. The request and its deadline are kept with the record | 4.1 (1), 5.3 | § 34 odst. 2: 'se nepřihlíží'; § 35 odst. 2: 'se nepřihlíží v rozsahu, ve kterém překračuje předmět hromadného řízení'; Městský soud v Praze, 1 July 2025, 3 C 10/2024-75, para. 72: 'Žalobce správně neměl po případné marné výzvě k odstranění vad přihlášek, k těmto přihláškám vůbec přihlížet a zahrnovat je do seznamu hromadníků ve smyslu § 38 z. h. ř.' |
| CZ-5 | A withdrawal of the whole přihláška on the ministry's form until the deadline is recorded `withdrawn`; a partial one leaves the record active for the rest, with the claim amended. One after the deadline has no effect, and the record stays `active` | 4.1 (1) | § 36: 'Přihlášku může zúčastněný člen skupiny vzít zcela nebo zčásti zpět do uplynutí lhůty pro přihlašování'; 'Jinak se ke zpětvzetí přihlášky nepřihlíží.' |
| CZ-6 | Each record holds the member's name, surname, residence and date of birth, or rodné číslo or a like unique identifier; for a legal person its name, seat and identification number | 4.1 (6) | § 2 odst. 1 písm. g): 'identifikačními údaji jméno, příjmení, bydliště a datum narození, popřípadě rodné číslo nebo obdobný jedinečný identifikátor, fyzické osoby nebo název, sídlo a identifikační číslo právnické osoby' |
| CZ-7 | A member who sued alone first: the přihláška and the record hold the case number of that action | 4.6 | § 33 odst. 3: 'musí přihláška obsahovat také spisovou značku nebo číslo jednací příslušného individuálního řízení' |
| CZ-8 | The register yields the list in the decree's format, with its columns, delivered with every přihláška after the deadline; each version is kept with its day and the snapshot root of that day | 5.4, 7 | vyhláška č. 181/2024 Sb., § 7: 'Seznam zúčastněných členů skupiny se vede v elektronické podobě v datovém formátu MS Excel Spreadsheet (*.xls/xlsx).'; § 9 písm. a) to d); § 38 odst. 2: 'Jakmile uplyne lhůta pro přihlašování, předloží žalobce soudu seznam zúčastněných členů skupiny a jejich přihlášky.' |
| CZ-9 | A person the court strikes from the list is recorded `excluded`, with the day the order became final | 4.1 (1), 5.3 | § 41: the court strikes a person 'není-li členství této osoby ve skupině s ohledem na předpoklady členství ve skupině alespoň pravděpodobné'; § 42 odst. 1 |
| CZ-10 | The register yields the judgment's annex: each member, whether the claim succeeds, and what each receives | 9 | § 70 odst. 2: 'Seznam zúčastněných členů skupiny je přílohou rozsudku a považuje se za součást jeho výroku.' |

## 5. Recommended items

- **A margin above 10.** Fewer than 10 on the list after the deadline stops the action (§ 39 odst. 1), and the court may revisit admissibility at any stage (§ 24 odst. 1).
- **The facts of each claim in fields of their own.** The court works from a sample of the claims: it 'nezjišťuje izolovaně skutkové okolnosti každého jednotlivého nároku zvlášť, nýbrž vychází zpravidla z určitého vzorku uplatněných nároků' (3 C 10/2024-75, para. 8).
- **A class size from a source outside the register.** The court sized the class from a Facebook group of 196 members (3 C 10/2024-10, para. 8) and from the capacity of an aircraft (3 C 3/2026, para. 3) when it set the joining period.
- **A count of přihlášky and withdrawals.** The costs of receiving přihlášky and keeping the list are recoverable at a flat 900 Kč per přihláška and 250 Kč per withdrawal (vyhláška č. 181/2024 Sb., § 10 odst. 2 and 3).
- **Access to the list kept narrow.** It goes to the defendant with every member's identity (§ 38 odst. 3) and sits in the court's file.
- **An operator processing přihlášky for the plaintiff.** Each přihláška reaches the plaintiff's own datová schránka or address, as the form names it, and the operator processes it there as the plaintiff's processor under a written mandate; the opt-in's day is the day the plaintiff had it, and a přihláška falls within the period only where the plaintiff had it in time (§ 31 odst. 1). This lowers the risk of the question section 8 leaves open; it does not settle it.

## 6. Recognised identification

- **Identity, grade A**: the Czech eID card, notified under eIDAS at assurance level high (the European Commission's overview of notified schemes: 2019/C 309/09), and the Mobile eGovernment Key and mojeID, notified at low, substantial and high (notified 27 September 2021), all covered by `eidas`. The record states the assurance the login reports: one at low stays at grade B (`assurance_too_low`). `cz.json` names no further scheme. A datová schránka signs a přihláška; it is no identification scheme of its own here.
- **Outside sources, grade B**: none named. The court has examined documents the members supplied: order confirmations, proofs of payment, demands and rescissions (3 C 10/2024-10, para. 9).

## 7. The level a typical action needs

A recommendation, not a court's rule.

- **Level 3, Verified.** Each přihláška carries a signature and the facts and evidence that make membership credible (§ 33), the plaintiff screens each before listing it (3 C 10/2024-75, para. 72), and the list, with each member's identity and award, becomes part of an enforceable judgment (§ 70 odst. 2).

## 8. Unsettled

- No appellate ruling under the act was found by 21 October 2026.
- Whether a bank identity or another electronic signature short of a qualified one meets § 5 of the decree. The form names a datová schránka or a qualified electronic signature.
- Whether a přihláška an operator receives for the plaintiff is made 'u žalobce' (§ 32 odst. 1). No source read addresses an agent.
- The validator tests that a record holds an opt-in, not how it was signed, nor its channel, which the law leaves to two, nor the deadline, since the export states no window. CZ-2 and CZ-4 set them, and the auditor checks each.
- Whether members who inspect the court's file see one another's identity data.

## Sources

1. Zákon č. 179/2024 Sb., o hromadném občanském řízení soudním, Sbírka zákonů (e-Sbírka): https://e-sbirka.gov.cz/sb/2024/179
2. Vyhláška č. 181/2024 Sb., o provedení některých ustanovení zákona o hromadném občanském řízení soudním, Sbírka zákonů (e-Sbírka): https://e-sbirka.gov.cz/sb/2024/181
3. Zákon č. 634/1992 Sb., o ochraně spotřebitele, část osmá, Sbírka zákonů (e-Sbírka): https://e-sbirka.gov.cz/sb/1992/634
4. Městský soud v Praze, usnesení ze dne 11. 2. 2025, č. j. 3 C 10/2024-10, rejstřík hromadných řízení: https://hromadnerizeni.justice.cz/wp-content/uploads/2025/03/3C_10_2024_6_PM.pdf
5. Městský soud v Praze, rozsudek ze dne 1. 7. 2025, č. j. 3 C 10/2024-75, rejstřík hromadných řízení: https://hromadnerizeni.justice.cz/wp-content/uploads/2025/03/3C_10_2024_36_sign.pdf
6. Městský soud v Praze, usnesení ze dne 8. 6. 2026, sp. zn. 3 C 3/2026, rejstřík hromadných řízení: https://hromadnerizeni.justice.cz/wp-content/uploads/2026/06/3C_3_2026_14PM.pdf
7. Přihláška do hromadného řízení, the form for 3 C 3/2026, rejstřík hromadných řízení: https://hromadnerizeni.justice.cz/wp-content/uploads/2026/06/Prihlaska_do_hromadneho_rizeni_3C3_26.pdf
8. Hromadné žaloby: Seznam oprávněných osob, Ministerstvo průmyslu a obchodu: https://mpo.gov.cz/cz/ochrana-spotrebitele/hromadne-rizeni/seznam-opravnenych-osob/hromadne-zaloby-seznam-opravnenych-osob--281743/
9. Overview of pre-notified and notified eID schemes under eIDAS, European Commission: https://ec.europa.eu/digital-building-blocks/sites/display/EIDCOMMUNITY/Overview+of+pre-notified+and+notified+eID+schemes+under+eIDAS

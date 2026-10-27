# Annex AT: Austria (Verbandsklage auf Abhilfe)

VCRS 0.1.0-beta.6. Draft for consultation. Not legal advice. Law and rulings as read on 19, 21 and 27 October 2026 on the Rechtsinformationssystem des Bundes (RIS), the Parlament's site, the Bundeskartellanwalt's publications and the Official Journal of the European Union.

Written by Holly Thackwray and Mischa Sigtermans for Steddle. Not yet reviewed by counsel admitted in Austria.

## 1. The regime

A collective damages action is a Verbandsklage auf Abhilfe under §§ 623 to 635 ZPO and the Qualifizierte-Einrichtungen-Gesetz (QEG), both enacted by the Verbandsklagen-Richtlinie-Umsetzungs-Novelle (BGBl. I Nr. 85/2024), in force since 18 July 2024. The ZPO rules apply to actions filed after the day the act was published: § 636(4) ZPO 'ist auf Verfahren anzuwenden, in denen die Klage nach dem Tag der Kundmachung eingebracht wird'.

- **Who may sue.** Only a Qualifizierte Einrichtung (QE): recognised by statute (§ 3 QEG) or by the Bundeskartellanwalt (§§ 1 and 2 QEG). No entity is admitted ad hoc for a single action: 'Daher ist keine ad hoc Zulassung einer Qualifizierten Einrichtung vorgesehen' (ErläutRV 2602 BlgNR XXVII. GP, zu § 629). A QE must be independent of businesses with an economic interest in the action, 'insbesondere Unternehmern, die ein wirtschaftliches Interesse an der Erhebung einer Verbandsklage haben, einschließlich im Falle einer Finanzierung durch Dritte' (§ 1(1) Z 4 QEG).
- **Court.** The Handelsgericht Wien alone (§ 630(1) ZPO).
- **The 50.** 'Die Klage hat ein bestimmtes Begehren auf Abhilfe von zumindest 50 Verbrauchern auf Grund von im Wesentlichen gleichartigen Sachverhalten gegen denselben Unternehmer zu enthalten' (§ 624(1) ZPO). The court tests this on the face of the claim, before service if need be: 'Die Zurückweisung einer Verbandsklage auf Abhilfe wegen des Fehlens von besonderen Prozessvoraussetzungen kann bereits vor Streitanhängigkeit erfolgen' (RS0142757).

## 2. Who is bound, and how they join

- **Opt-in, for everyone.** Austria chose 'für die Verbandsklage auf Abhilfe ein opt-in System' (ErläutRV zu § 624). The judgment binds the consumers named in the claim and those who join (§ 624(1), § 628(4) ZPO); a court-approved settlement 'bindet auch die beigetretenen Verbraucher' (§ 631(3)). Neither § 624 nor § 628 distinguishes by residence, so everyone opts in, wherever they live: `at.json` sets `opt_in_abroad` and `opt_in_residents` to true, names the QE's filing as the channel, `qe`, and asks every opt-in for the declaration on parallel actions (core 4.6). The export states no opt-in window: the opt-in is due from the start, so a record counts once the QE has filed the claim or the Beitritt that names the person.
- **Joining, through the QE.** 'Einer Verbandsklage auf Abhilfe kann jeder Verbraucher im Wege der Qualifizierten Einrichtung beitreten' (§ 628(1)), and 'Der Beitritt kann von der Qualifizierten Einrichtung ohne Angabe von Gründen abgelehnt werden'. It runs in two steps: 'Der Beitritt erfolgt zweistufig, indem sich der Verbraucher zunächst außergerichtlich und verfahrensrechtlich unverbindlich an die Qualifizierte Einrichtung wendet' (ErläutRV zu § 628). The QE then files a Schriftsatz with court and defendant stating the facts, a claim, 'sowie die Erklärung, dass der Anspruch weder im Inland noch im Ausland geltend gemacht wurde oder wird' (§ 628(2)).
- **The window.** 'Ein Beitritt kann bis drei Monate nach Veröffentlichung der Entscheidung über die Durchführung eines Verbandsklageverfahrens gemäß § 627 Abs. 1 ZPO erfolgen' (§ 628(3)). The QE may set a shorter one: 'Es steht der Qualifizierten Einrichtung aber frei, diesen Zeitraum zu verkürzen' (ErläutRV zu § 628).
- **No withdrawal.** 'Eine Zurücknahme des Beitritts ist unzulässig' (§ 628(5)).
- **Who holds the list.** The QE. No court registry or state portal takes sign-ups. 'Qualifizierte Einrichtungen haben sicherzustellen, dass Beitrittserklärungen samt Unterlagen on- und offline eingereicht werden können' (§ 9(5) QEG), and the QE gives the court the address and the form for its publication (§ 627(2) Z 3 and 4 ZPO).

## 3. When the register is tested

| Stage | What it asks of the register | Source |
|---|---|---|
| Before filing | The QE publishes planned actions, how to join, the costs and whether a fee or a funder contract is required; it offers a Formblatt and takes joining declarations on- and offline | § 9(1), (3), (5) QEG |
| Filing | At least 50 consumers per defendant, each identified and shown to be a consumer, each with a specific claim and its facts; the facts the claims share; the abstract criteria for later joiners. The count need only stand on this day | § 624(1), (3) ZPO; OGH 8 Ob 143/25z [16] to [18]; OGH 9 Ob 111/25a [26], [31] |
| Admissibility | The pleaded facts, taken as true, must show substantially similar facts; objections to single claims matter where they take the count below 50 | § 626(1), § 625 ZPO; RS0142756, RS0142757 |
| Publication | The admission decision, with the QE's address and joining form | § 627 ZPO |
| Joining | Per joiner, the QE's Schriftsatz with the facts, a claim and the declaration on parallel actions, inside the window | § 628 ZPO |
| Judgment and settlement | Per claimant, the facts and the amount; a settlement binds the joiners | § 626(1), § 631(3), § 634 ZPO |
| Distribution | The payee for each claimant, the QE where it asked for payment to itself, and the QE's payout record | § 633 ZPO; § 9(7) QEG |
| After rejection | Who had joined and when, so each can use the three months left to them | § 635 ZPO |

**Reference dates.** The filing date for the initial 50: the number need be met 'nur im Zeitpunkt der Klagserhebung' (ErläutRV zu § 624). For joiners, the date each Beitritt is filed, and the last day of the window. No Abhilfeklage had been admitted by 19 October 2026: the Handelsgericht Wien's page for publications under §§ 627 and 634 listed none.

## 4. Required items

A register that claims a level in an Austrian action meets every item below. The first table holds what Austrian law requires, by statute or a court's holding. The second holds what this standard requires beyond the law, with the reason.

### What the law requires

| # | Item | Core | Source |
|---|---|---|---|
| AT-1 | At filing, at least 50 consumers per defendant, each named in the claim with a specific claim. Where several traders are sued, a count per defendant | 6.2, 6.4 | § 624(1) ZPO: 'zumindest 50 Verbrauchern auf Grund von im Wesentlichen gleichartigen Sachverhalten gegen denselben Unternehmer'; OGH 20 May 2026, 8 Ob 143/25z, [16]: 'Deshalb sind die Prozessvoraussetzungen für jeden Streitgenossen gesondert zu prüfen' |
| AT-2 | Each record holds the person's consumer status as a fact of membership | 4.2, 4.3 | § 624(1) ZPO ('Verbrauchern'); the Handelsgericht Wien's order, as quoted in OLG Wien 30 September 2025, 33 R 135/25b: 'konkretes Vorbringen zur Verbrauchereigenschaft der Personen, deren Begehren auf Abhilfe geltend gemacht werde' |
| AT-3 | Per claim, the facts it rests on: the contract or transaction, the clause or act, and the amount claimed, substantiated as far as the facts and evidence are accessible to the QE with reasonable effort and support the claim's plausibility. That lighter standard covers the claims, not the shared facts AT-4 asks for | 4.3, 6.5 | § 624(1) ZPO: 'die Tatsachen, auf welche sich die Ansprüche in Haupt- und Nebensachen gründen, im Einzelnen kurz und vollständig anzugeben'; § 624(5) ZPO: 'die der Qualifizierten Einrichtung mit zumutbarem Aufwand zugänglich sind und die die Plausibilität der Ansprüche ausreichend stützen'; OGH 27 January 2026, 9 Ob 111/25a, [25]: § 624(5) deals with the claims, 'nicht mit dem schlüssigen im Sinn von vollständigen Vortrag zu den Prozessvoraussetzungen' |
| AT-4 | The facts the claims share, and for each claimant whether they match or how they differ, by liability basis | 6.4 | OGH 9 Ob 111/25a [26]: 'Eine konkrete Behauptung, inwiefern die objektive Vertragslage betreffend die übrigen Verbraucher ident ist und inwiefern sie abweicht, lassen selbst die Ausführungen im Revisionsrekurs vermissen.'; [31]: 'Folglich sind die den klagsgegenständlichen Rechtsverhältnissen zugrunde liegenden, gemeinsamen Sachverhaltselemente schon in der Klage darzulegen.'; OGH 8 Ob 143/25z [21]: the action needs facts 'die in ihren wesentlichen anspruchsbegründenden Elementen so weit übereinstimmen, dass eine einheitliche rechtliche Beurteilung der Ansprüche möglich ist' |
| AT-5 | Where the QE opens the action to joiners, the abstract criteria as filed, and each joiner's fit against them | 3, 6.1 | § 624(3) ZPO: 'Die abstrakten Kriterien, die ein Anspruch aufweisen muss, um vom Verfahren betroffen zu sein, und die Voraussetzungen, unter denen diese Verbraucher beitreten können, sind von der Qualifizierten Einrichtung genau anzugeben.' |
| AT-6 | Each record holds its opt-in: the day the QE filed the claim or the Beitritt that names the person, through the channel `qe`. Per joiner also the request to the QE with its date and channel, the QE's acceptance or refusal, and a Beitritt filed inside the window. A refused request, one not filed in time, or a Beitritt the court rejects is recorded `excluded` (core 4.1 (1)) | 4.1 (1), 4.6, 5.3 | § 628(1) to (3) ZPO; § 628(4): 'Ein Beitritt ist zurückzuweisen, wenn der im Beitritt geltend gemachte Anspruch bereits in einem Einzelverfahren oder in einem anderen Verbandsklageverfahren geltend gemacht wird.'; § 9(5) QEG |
| AT-7 | Per joiner, the declaration on parallel actions, held as `parallel_declared` | 4.1 (8), 4.6 | § 628(2) ZPO: 'die Erklärung, dass der Anspruch weder im Inland noch im Ausland geltend gemacht wurde oder wird'; § 628(4): a Beitritt is rejected where the claim is pending elsewhere |
| AT-8 | A joiner whose Beitritt was filed stays active unless the court rejects it (AT-6): the record never turns `withdrawn` | 4.1 (1) | § 628(5) ZPO: 'Eine Zurücknahme des Beitritts ist unzulässig.' |
| AT-9 | Each joiner received the QE's Formblatt with its Belehrung, captured as a flow version | 5.1 | § 9(3) QEG: 'eine Belehrung über die Voraussetzungen, den Ablauf und die Wirkungen eines Verbandsklageverfahrens und die voraussichtlichen Kosten' |
| AT-10 | Any joining fee per joiner, within the cap; where the QE makes joining depend on a funder contract, that contract signed per joiner | 9 | § 9(4) QEG: 'Eine allfällige Beitrittsgebühr darf weder höher als 20 Prozent der jeweils geltend gemachten Anspruchssumme sein, noch darf diese 250 Euro überschreiten.'; § 6(1) QEG: the QE may make joining depend on the joiner signing 'den zwischen der Qualifizierten Einrichtung und dem Drittfinanzierer vereinbarten Vertrag'; § 9(1) Z 3 lit e QEG: the QE publishes 'ob eine Beitrittsgebühr bezahlt oder ein Drittfinanzierungsvertrag abgeschlossen werden muss' |
| AT-11 | The payee per claimant and the payout record | 5.3, 9 | § 633 ZPO; § 9(7) QEG: the QE must 'die Abwicklung der Auszahlung unverzüglich durchführen' |

### What this standard requires

| # | Item | Core | Reason |
|---|---|---|---|
| AT-12 | Deduplication on name and birth date at least, so that namesakes are told apart | 4.1 (6), 4.5 | The Handelsgericht Wien ordered the QE 'die Personen, deren Begehren auf Abhilfe geltend gemacht werde, unzweifelhaft individualisierbar so zu beschreiben, dass das Gericht prüfen könne, ob die mehrfache Anführung des gleichen Namens in Beilage ./D dieselbe Person oder verschiedene, namensgleiche Personen betreffe' (as quoted in OLG Wien 33 R 135/25b); a list of consumers 'durch ihr Geburtsdatum individualisierten' drew no criticism (OGH 9 Ob 111/25a [2]) |
| AT-13 | The consumers named in the claim hold the declaration on parallel actions too | 4.1 (8), 4.6 | § 628(2) ZPO asks it of joiners alone. A named consumer's claim pursued elsewhere fails the same way a joiner's does (§ 628(4)), and nobody is represented twice on the same claim (Directive (EU) 2020/1828, art. 9(4)). `parallel_declaration` applies to every opt-in, so the validator asks it of all |

## 5. Recommended items

- **A margin above 50 per defendant.** An objection to single claims matters once it takes the count below the number the law sets (§ 625 ZPO).
- **Proof that each claim was disputed out of court before filing.** The QE must show consumers 'deren Ansprüche auf Abhilfe außergerichtlich strittig sind' (ErläutRV zu § 624), and the claims should be asserted by the QE or a lawyer, not by an operator (OGH 25 January 2024, 4 Ob 5/24z, [17]).
- **The document behind each claim, not a sample.** One contract did not carry the claims of the whole list (OGH 9 Ob 111/25a [26]).
- **Subgroups by liability basis within one defendant.** Claims against the maker of a car and against the maker of its engine call for different rules of liability (OGH 8 Ob 143/25z [22]), so each subgroup can stand on its own.
- **Notice to each joiner that the claim data go to the defendant**, since the Beitritt is notified 'dem Gericht und der beklagten Partei gegenüber' (§ 628(2) ZPO), and a processor agreement where an operator works for the QE (art. 28 GDPR; the QE's own processing rests on § 9(8) QEG).
- **A log that separates the operator's formal checks from the decisions of the QE and the lawyer.** The OGH left standing, as tenable, lower-court findings that an operator which only checks documents for completeness and then hands the case to a lawyer stays within the law (OGH 23 February 2021, 4 Ob 180/20d, [8]), and that an operator with power over the lawyers became 'Herr des Verfahrens' (OGH 10 September 2024, 4 Ob 144/24s, [19]). In both, the OGH rejected the appeal in provisional-measures proceedings as inadmissible.
- **An operator taking requests for the QE.** Each consumer's request to join is addressed to the QE by name, at a channel the QE publishes as its own; the operator receives it as the QE's processor under a written mandate to receive; and the register keeps the day the operator received it and the day the QE had it. This lowers the risk of the question section 8 leaves open; it does not settle it.

## 6. Recognised identification

- **Identity, grade A**: ID Austria, notified under eIDAS at assurance level high (Official Journal C 173 I of 27 April 2022), and so covered by `eidas`. `at.json` names no further scheme.
- **Outside sources, grade B**: none named. The contract or document from which each claim is pleaded is the evidence the courts have examined.

## 7. The level a typical action needs

A recommendation, not a court's rule.

- **Level 3, Verified, for the claims pleaded at filing and for every joiner.** The Handelsgericht Wien takes the pleading as true but tests it on its face at filing, and both actions that reached the OGH failed on the list of consumers: one did not show each contract's clause (9 Ob 111/25a), the other bundled four defendants and two bases of liability (8 Ob 143/25z). A register that holds each claimant's document (grade B, supplied) answers the test.
- **Identity at grade C suffices** on the rulings read: name and birth date, with consumer status recorded.

## 8. Unsettled

- No Abhilfeklage had been admitted by 19 October 2026, so no published joining form or court-approved joining criteria could be read.
- Whether an operator may receive joining declarations in the QE's name, as its agent. The law says joining runs 'im Wege der Qualifizierten Einrichtung'; no source read addresses an agent.
- Consumers resident abroad joining an action at the Handelsgericht Wien: no text or ruling beyond § 5(5) QEG for qualified entities of other Member States.
- What 'dieselben Tatfragen' in § 628(1) adds to § 624(1): the OGH found no separate meaning (9 Ob 111/25a [14]); the OLG Wien read it as a description.
- Whether the court may examine joiners' documents after admission, and what proof the defendant may demand per joiner.
- The opt-in is due from the start, since the consumers named in the claim opt in at filing. The export states the three months of § 628(3), or the shorter window the QE set, as a term (`opt_in_terms`), and the validator does not count a Beitritt dated after it. AT-6 also records a late one `excluded`, and the auditor checks the day against the court's file.

## Sources

1. Zivilprozessordnung §§ 623 to 636, RIS: https://www.ris.bka.gv.at/NormDokument.wxe?Abfrage=Bundesnormen&Gesetzesnummer=10001699&Paragraf=624
2. Qualifizierte-Einrichtungen-Gesetz, RIS: https://www.ris.bka.gv.at/GeltendeFassung.wxe?Abfrage=Bundesnormen&Gesetzesnummer=20012650
3. BGBl. I Nr. 85/2024 (VRUN), RIS: https://www.ris.bka.gv.at/Dokumente/BgblAuth/BGBLA_2024_I_85/BGBLA_2024_I_85.html
4. 2602 der Beilagen XXVII. GP, Regierungsvorlage, Erläuterungen, Parlament: https://www.parlament.gv.at/gegenstand/XXVII/I/2602
5. OGH 27 January 2026, 9 Ob 111/25a: https://www.ris.bka.gv.at/Dokumente/Justiz/JJT_20260127_OGH0002_0090OB00111_25A0000_000/JJT_20260127_OGH0002_0090OB00111_25A0000_000.html
6. Rechtssätze RS0142756 and RS0142757: https://www.ris.bka.gv.at/Dokumente/Justiz/JJR_20260127_OGH0002_0090OB00111_25A0000_001/JJR_20260127_OGH0002_0090OB00111_25A0000_001.html
7. OLG Wien 30 September 2025, 33 R 135/25b: https://www.ris.bka.gv.at/Dokumente/Justiz/JJT_20250930_OLG0009_03300R00135_25B0000_000/JJT_20250930_OLG0009_03300R00135_25B0000_000.html
8. OGH 20 May 2026, 8 Ob 143/25z: https://www.ris.bka.gv.at/Dokumente/Justiz/JJT_20260520_OGH0002_0080OB00143_25Z0000_000/JJT_20260520_OGH0002_0080OB00143_25Z0000_000.html
9. OGH 23 February 2021, 4 Ob 180/20d: https://www.ris.bka.gv.at/Dokumente/Justiz/JJT_20210223_OGH0002_0040OB00180_20D0000_000/JJT_20210223_OGH0002_0040OB00180_20D0000_000.html
10. OGH 10 September 2024, 4 Ob 144/24s: https://www.ris.bka.gv.at/Dokumente/Justiz/JJT_20240910_OGH0002_0040OB00144_24S0000_000/JJT_20240910_OGH0002_0040OB00144_24S0000_000.html
11. OGH 25 January 2024, 4 Ob 5/24z: https://www.ris.bka.gv.at/Dokumente/Justiz/JJT_20240125_OGH0002_0040OB00005_24Z0000_000/JJT_20240125_OGH0002_0040OB00005_24Z0000_000.html
12. Handelsgericht Wien, Verbandsklagen, publications under §§ 627 and 634 ZPO: https://justiz.gv.at/hg-wien/handelsgericht-wien/verbandsklagen.e23.de.html
13. Electronic identification schemes notified pursuant to Article 9(1) of Regulation (EU) No 910/2014, OJ C 173 I, 27 April 2022: https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=uriserv%3AOJ.CI.2022.173.01.0001.01.ENG

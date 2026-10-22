# Annex PL: Poland (postępowanie grupowe)

VCRS 0.1.0-beta.4. Draft for consultation. Not legal advice. Law and rulings as read on 19 and 21 October 2026 in the Dziennik Ustaw, on the Sąd Najwyższy's site, on the common courts' judgment portals, on the Urząd Ochrony Konkurencji i Konsumentów's register and in the European Commission's overview of notified eID schemes.

## 1. The regime

A collective damages action is a postępowanie grupowe under the ustawa z dnia 17 grudnia 2009 r. o dochodzeniu roszczeń w postępowaniu grupowym (consolidated text Dz.U. 2024 poz. 1485), which the ustawa z dnia 24 lipca 2024 r. (Dz.U. 2024 poz. 1237) amended to transpose the Directive, in force since 29 August 2024. Cases pending on that day keep the earlier wording: 'Do spraw prowadzonych w postępowaniu grupowym wszczętych i niezakończonych przed dniem wejścia w życie niniejszej ustawy stosuje się przepisy ustawy zmienianej w art. 1, w brzmieniu dotychczasowym' (Dz.U. 2024 poz. 1237, art. 6).

- **Two kinds of action, one statute.** 'Powództwo w postępowaniu grupowym wytacza reprezentant grupy, a w sprawach o stwierdzenie stosowania praktyk naruszających ogólne interesy konsumentów lub w sprawach o roszczenia związane z ich stosowaniem wyłącznie podmiot upoważniony' (art. 4 ust. 1). The representative of a member-led action is 'osoba będąca członkiem grupy albo powiatowy (miejski) rzecznik konsumentów' (art. 4 ust. 2), or the Rzecznik Finansowy for clients of the financial market (art. 4 ust. 2a). A podmiot upoważniony is an entity on the register of the Prezes UOKiK, which on 21 October 2026 held the Rzecznik Finansowy and Fundacja LexCultura, or on the Commission's list (art. 46a u.o.k.k.). The export states an action by a podmiot upoważniony as `directive` true.
- **The group.** 'Ustawa normuje sądowe postępowanie cywilne w sprawach, w których są dochodzone roszczenia jednego rodzaju, co najmniej 10 osób, oparte na tej samej lub takiej samej podstawie faktycznej (postępowanie grupowe)' (art. 1 ust. 1). Consumers' money claims need not be equalised: 'Przepisów ust. 1 i 2 nie stosuje się w sprawach o roszczenia konsumentów' (art. 2 ust. 2a). A money claim may be limited to establishing the defendant's liability (art. 2 ust. 3).
- **Court.** 'Postępowanie grupowe należy do właściwości sądu okręgowego' (art. 3 ust. 1), sitting with three professional judges, the composition order included (Sąd Najwyższy, III CZP 5/25). A lawyer is mandatory (art. 4 ust. 4).

## 2. Who is bound, and how they join

- **Opt-in, for everyone.** 'Wszczęcie postępowania grupowego nie wyłącza możliwości dochodzenia swych roszczeń przez osoby, które nie przystąpiły do grupy lub z niej wystąpiły' (art. 1 ust. 3), and 'Wyrok prawomocny ma skutek wobec wszystkich członków grupy' (art. 21 ust. 3). The act draws no line by residence, so residents and people abroad both opt in: `pl.json` sets `opt_in_abroad` and `opt_in_residents` to true, names the representative as the channel, `representative`, for the reprezentant grupy and the podmiot upoważniony alike, and asks every opt-in for the declaration on parallel claims (PL-7, PL-14).
- **Before filing.** The claim attaches the founding members' declarations: 'Do pozwu należy dołączyć oświadczenia członków grupy o przystąpieniu do grupy i wyrażeniu zgody co do osoby reprezentanta grupy' (art. 6 ust. 2); in a podmiot upoważniony's action, the declarations and the funding agreement (art. 6 ust. 4).
- **After admission.** Once the order admitting the action is final, the court orders an announcement offering others to join 'poprzez złożenie reprezentantowi grupy albo podmiotowi upoważnionemu, w oznaczonym terminie, nie krótszym niż miesiąc i nie dłuższym niż 3 miesiące od dnia ogłoszenia, pisemnego oświadczenia o przystąpieniu do grupy' (art. 11 ust. 2 pkt 3). 'Przystąpienie do grupy po upływie terminu wyznaczonego przez sąd jest niedopuszczalne' (art. 11 ust. 5). A person who sued alone before may join until the first instance ends, and the court discontinues the own action (art. 13 ust. 2).
- **No window in the export.** People join from before filing to the end of the court's term, so the opt-in is due from the start: a record counts once it holds the person's written declaration to the representative, and the export states no opt-in window. A declaration after the court's term is recorded `excluded`, save one under art. 13 ust. 2 (PL-2), which the auditor checks (section 8).
- **The declaration.** 'W oświadczeniu o przystąpieniu do grupy uprawniony powinien określić swe żądanie oraz wskazać okoliczności uzasadniające żądanie, a także przynależność do grupy oraz przedstawić dowody' (art. 12). It takes effect against the defendant when presented to the court (art. 13 ust. 1).
- **Withdrawal.** Until the composition order is final; then 'oświadczenie członka grupy o wystąpieniu z grupy jest bezskuteczne' (art. 17 ust. 3), save that a member of a podmiot upoważniony's action may leave within two weeks of being told of a settlement they reject (art. 19a ust. 1).
- **Who holds the list.** 'Wykaz osób, które przystąpiły do grupy, sporządza powód i przedstawia sądowi, dołączając oświadczenia o przystąpieniu do grupy. Sąd doręcza wykaz pozwanemu.' (art. 12). The court's composition order is the list that binds.

## 3. When the register is tested

| Stage | What it asks of the register | Source |
|---|---|---|
| Filing | At least 10 declarations attached, each for a claim of one kind on the same or same-type facts; for money claims each member's amount; in a member-led action each founding member's consent to the representative; in a podmiot upoważniony's action the statements of art. 6 ust. 7 and the funding agreement | art. 1 ust. 1; art. 6 ust. 1 pkt 3, ust. 2, 4, 7; SO Warszawa II C 121/11 |
| Admission | The court rules on the claim as filed, after hearing the parties, and cannot carve a valid group out of a mixed list | art. 10 ust. 1; SO Warszawa II C 121/11 |
| Announcement and joining | Declarations to the representative within the court's term, one to three months from the announcement | art. 11 ust. 2 pkt 3, ust. 5 |
| Composition of the group | The list with every declaration, served on the defendant; the defendant's objections to named persons; proof of membership for money claims, plausibility for others; the court's order on each person, open to appeal, after which the group is fixed | art. 12, 15, 16 ust. 1, 17; SN III CZP 5/25; SN III CZP 51/22 |
| Judgment | Every member named, and in a money judgment what each receives, in the operative part or a list annexed to it | art. 21 ust. 1, 2, 2a |
| Enforcement | An extract per member stating what is due to them | art. 22 |
| Settlement | The consent of more than half the members; in a podmiot upoważniony's action, the member's exit within two weeks | art. 19 ust. 1; art. 19a ust. 1 |

**Reference dates.** The filing date for the 10 (SO Warszawa II C 121/11). The day the composition order becomes final, which fixes the group: 'Na tym etapie następuje też stabilizacja składu grupy' (SN III CZP 5/25). Per record, the day the declaration reached the representative and the day it was presented to the court.

## 4. Required items

A register that claims a level in a Polish action meets every item below. The first table holds what Polish law requires, by statute or a court's holding. The second holds what this standard requires beyond the law, with the reason.

### What the law requires

| # | Item | Core | Source |
|---|---|---|---|
| PL-1 | At filing, at least 10 records hold a declaration attached to the claim, each for a claim of one kind on the same or same-type facts, so that each list the claim pleads stands on its own | 6.2, 6.4 | art. 1 ust. 1: 'roszczenia jednego rodzaju, co najmniej 10 osób, oparte na tej samej lub takiej samej podstawie faktycznej'; SO Warszawa 8 April 2011, II C 121/11: the thresholds 'muszą być spełnione już w momencie składania pozwu', and the court 'nie ma uprawnień do jego modyfikowania choćby przez selekcję poszczególnych elementów' |
| PL-2 | Each record holds its opt-in: the person's written declaration of joining and the day it reached the representative, through the channel `representative`. A declaration made after the court's term is recorded `excluded` (core 4.1 (1)), unless the person sued the defendant on the claim before the group action began and declared before the first instance ended | 4.1 (1), 4.6, 5.3 | art. 11 ust. 2 pkt 3: 'pisemnego oświadczenia o przystąpieniu do grupy'; art. 11 ust. 5: 'Przystąpienie do grupy po upływie terminu wyznaczonego przez sąd jest niedopuszczalne.'; SO Warszawa 16 December 2020, XXIV C 709/15, checking each person: 'oświadczyły o przystąpieniu do grupy we właściwym czasie'; art. 13 ust. 2: such a person 'nie później niż do dnia zakończenia postępowania w pierwszej instancji może złożyć oświadczenie o przystąpieniu do grupy' |
| PL-3 | Each declaration states the claim, the facts behind it, why the person is a member, and the evidence | 4.3, 6.5 | art. 12: 'W oświadczeniu o przystąpieniu do grupy uprawniony powinien określić swe żądanie oraz wskazać okoliczności uzasadniające żądanie, a także przynależność do grupy oraz przedstawić dowody.' |
| PL-4 | In a money claim each record's membership rests on evidence (core 4.3); in any other claim, on evidence that makes it plausible | 4.3 | art. 16 ust. 1: 'W sprawach o roszczenia pieniężne ciężar udowodnienia przynależności członka do grupy spoczywa na powodzie. W innych sprawach do ustalenia przynależności członka do grupy wystarcza uprawdopodobnienie.'; SO Warszawa 11 September 2017, XXV C 1529/15: 'Konsekwencją nieudowodnienia (nieuprawdopodobnienia) przynależności określonej osoby do grupy (podgrupy) przez powoda jest wyłączenie przez sąd tej osoby ze składu grupy.' |
| PL-5 | In a money claim, the amount each member claims | 6.5 | art. 6 ust. 1 pkt 3: 'w przypadku roszczeń pieniężnych określenie wysokości roszczenia każdego z członków grupy lub podgrup' |
| PL-6 | In a member-led action, each declaration attached to the claim holds the person's consent to the named representative | 5.1 | art. 6 ust. 2: 'oświadczenia członków grupy o przystąpieniu do grupy i wyrażeniu zgody co do osoby reprezentanta grupy' |
| PL-7 | In a podmiot upoważniony's action, each declaration attached to the claim states whether the person joined another group action, or sued, against the defendant over the same infringement, and how the entity is to reach them. The record holds `parallel_declared` true only where the statements show no other group action and no own action other than one filed before the group action began, which the court discontinues on joining (art. 13 ust. 2), and the contact channel is the one the declaration names | 4.1 (7), 4.1 (8), 4.6 | art. 6 ust. 7: the member states '1) czy przystąpił do grupy w innym postępowaniu grupowym wytoczonym przeciwko pozwanemu w związku z tym samym naruszeniem; 2) czy wytoczył przeciwko pozwanemu powództwo w związku z tym samym naruszeniem; 3) o sposobie komunikacji z podmiotem upoważnionym'; art. 10aa ust. 5: 'Przekazanie informacji członkowi grupy przez podmiot upoważniony następuje w sposób wskazany w oświadczeniu o przystąpieniu do grupy.' |
| PL-8 | Per record, the day the declaration was presented to the court | 5.3 | art. 13 ust. 1: 'Z chwilą przedstawienia sądowi oświadczenia o przystąpieniu do grupy między członkiem grupy oraz pozwanym powstaje skutek sprawy w toku' |
| PL-9 | Per record, the defendant's objection to the person and the court's ruling on them. A person the court refuses is recorded `excluded` | 4.1 (1), 5.3 | art. 15; art. 17 ust. 1; SN 24 July 2025, III CZP 5/25: 'W postanowieniu co do składu grupy sąd rozstrzyga o przyznaniu lub odmowie przyznania statusu członka grupy osobom, które złożyły reprezentantowi grupy oświadczenie o przystąpieniu do grupy' |
| PL-10 | A withdrawal before the composition order is final is recorded `withdrawn`. After it a withdrawal has no effect and the record stays `active`, save a member's exit after a settlement in a podmiot upoważniony's action | 4.1 (1) | art. 17 ust. 3: 'Po uprawomocnieniu się postanowienia, o którym mowa w ust. 1, oświadczenie członka grupy o wystąpieniu z grupy jest bezskuteczne.'; art. 19a ust. 1; SA Łódź 4 July 2025, I ACa 202/25: 'Ustawa wyklucza zatem skuteczne wystąpienie z grupy po prawomocnym ustaleniu składu grupy.' |
| PL-11 | A member whose claim the court discontinues after the composition order, having settled with the defendant or won a separate judgment, is recorded `excluded` with the day and the reason, and stays in the register | 4.1 (1), 5.3 | SA Łódź I ACa 202/25: 'Sąd Apelacyjny ostatecznie stanął na stanowisku, że zawarte ugody czy wydane wyroki muszą znaleźć odzwierciedlenie w treści rozstrzygnięcia.' |
| PL-12 | The register yields the judgment's list: every member by name, told apart from namesakes, with the amount due to each, and an extract per member | 4.1 (6), 9 | art. 21 ust. 1: 'W sentencji wyroku należy wymienić wszystkich członków grupy lub podgrupy.'; art. 21 ust. 2: 'W wyroku zasądzającym świadczenie pieniężne należy ustalić, jaka kwota przypada każdemu członkowi grupy lub podgrupy.'; art. 22 |
| PL-13 | In a podmiot upoważniony's action, any joining fee per member: no more than 5% of the member's money claim and 2 000 zł, or 1 000 zł for a claim that is not for money, and no other charge to the member | 9 | art. 5a ust. 2: 'nie może przekraczać 5 % wartości dochodzonego przez członka grupy roszczenia pieniężnego, jednak nie może być wyższa niż 2000 zł, a w przypadku roszczenia niepieniężnego wysokość ustalonej opłaty nie może być wyższa niż 1000 zł'; art. 5b: the fee 'stanowi jedyny koszt, jaki konsument ponosi' |

### What this standard requires

| # | Item | Core | Reason |
|---|---|---|---|
| PL-14 | Every declaration, in either kind of action and whenever made, carries the statements of art. 6 ust. 7 points 1 and 2, held as `parallel_declared` as PL-7 says | 4.1 (8), 4.6 | art. 6 ust. 7 asks them only of the declarations a podmiot upoważniony's claim attaches. A person who sued alone and then joins has the own action discontinued (art. 13 ust. 2), and nobody is represented twice on the same claim (Directive (EU) 2020/1828, art. 9(4)). `parallel_declaration` applies to every opt-in, so the validator asks it of all |
| PL-15 | Each declaration is signed by hand, or with a qualified electronic signature | 4.6, 5.3 | The act asks for a 'pisemnego oświadczenia' (art. 11 ust. 2 pkt 3), and for the written form of a legal act the Kodeks cywilny asks 'złożenie własnoręcznego podpisu na dokumencie obejmującym treść oświadczenia woli' (art. 78 § 1), which a qualified electronic signature equals (art. 78¹ § 1 and § 2). No ruling read decides whether a lighter form is 'pisemne', and the defendant may object to the membership of each named person (art. 15), which the court decides on the declarations and documents (XXIV C 709/15). A register that meets a level holds declarations that survive that objection |

## 5. Recommended items

- **A margin above 10 at filing, and one list per kind of claim.** The threshold cannot be cured after filing, and in II C 121/11 claims for the death of relatives and for property loss could not be pooled.
- **Evidence of consumer status** where the defendant can argue business use: in XXIV C 709/15 the court held that 'Sama okoliczność, że dana osoba wykonuje działalność gospodarczą, nie implikuje domniemania faktycznego' and checked the contracts.
- **The declaration in the languages the entity publishes** for joining (art. 46c pkt 2 lit. e u.o.k.k.).
- **A record of the announcement**: where and when it was published (art. 11 ust. 3).
- **An operator receiving declarations for the representative.** Each declaration is addressed to the representative by name, at a channel the representative publishes as its own; the operator receives it as the representative's processor under a written mandate to receive; the opt-in's day is the day the representative had it, and the register keeps the day the operator received it. A declaration falls within the court's term only where the representative had it in time (art. 11 ust. 2 pkt 3, ust. 5). This lowers the risk of the question section 8 leaves open; it does not settle it.

## 6. Recognised identification

- **Identity, grade A**: the Public Electronic Identification System, with the profil zaufany and the profil osobisty, notified under eIDAS at assurance levels substantial and high (the European Commission's overview of notified schemes: 2023/C 136/02), and so covered by `eidas`. `pl.json` names no further scheme.
- **Outside sources, grade B**: a public register the membership fact can be read in. In XXV C 1529/15 the court checked each declaration against 'odpisów zwykłych ksiąg wieczystych i wypisów z rejestru gruntów'.

## 7. The level a typical action needs

A recommendation, not a court's rule.

- **Level 3, Verified, for an action for money.** The representative proves each member's membership (art. 16 ust. 1), the defendant may object person by person and the court checks each declaration against documents (XXV C 1529/15, XXIV C 709/15), and the judgment names each member with the amount due (art. 21).
- **Level 2, Identified, for an action limited to liability** (art. 2 ust. 3), where plausibility suffices (art. 16 ust. 1), with the evidence behind each record.

## 8. Unsettled

- Whether art. 4 ust. 1, which reserves claims connected with practices infringing the collective interests of consumers to a podmiot upoważniony, bars a member-led action on facts that are also such a practice.
- Whether a declaration signed electronically without a qualified signature, scanned or clicked is 'pisemne' in art. 11 ust. 2 pkt 3.
- Whether the 10 are tested again when members fall below 10 after admission. II C 121/11 is a first-instance order.
- The export states no opt-in window, since the opt-in is due from the start, so the validator does not test that a declaration came within the court's term: PL-2 records a late one `excluded`, and the auditor checks it.
- Whether art. 6 ust. 7's statements bind declarations made after the announcement. PL-14 asks them of all.
- Whether a declaration an operator receives for the representative is made to the representative (art. 11 ust. 2 pkt 3). No source read addresses an agent.
- No ruling under the 2024 rules on an action by a podmiot upoważniony was found.

## Sources

1. Ustawa z dnia 17 grudnia 2009 r. o dochodzeniu roszczeń w postępowaniu grupowym, consolidated text, Dz.U. 2024 poz. 1485, Dziennik Ustaw: https://dziennikustaw.gov.pl/DU/2024/1485
2. Ustawa z dnia 24 lipca 2024 r. o zmianie ustawy o dochodzeniu roszczeń w postępowaniu grupowym oraz niektórych innych ustaw, Dz.U. 2024 poz. 1237, Dziennik Ustaw: https://dziennikustaw.gov.pl/DU/2024/1237
3. Ustawa z dnia 16 lutego 2007 r. o ochronie konkurencji i konsumentów, consolidated text, Dz.U. 2025 poz. 1714, Dziennik Ustaw: https://dziennikustaw.gov.pl/DU/2025/1714
4. Kodeks cywilny, consolidated text, Dz.U. 2026 poz. 795, Dziennik Ustaw: https://dziennikustaw.gov.pl/DU/2026/795
5. Sąd Najwyższy, uchwała z 24 lipca 2025 r., III CZP 5/25: https://www.sn.pl/images/Komunikaty_o_sprawach/iii_czp_5-25.pdf
6. Sąd Najwyższy, uchwała z 25 stycznia 2022 r., III CZP 51/22: https://www.sn.pl/sites/orzecznictwo/Orzeczenia3/III%20CZP%2051-22.pdf
7. Sąd Okręgowy w Warszawie, postanowienie z 8 kwietnia 2011 r., II C 121/11, Portal Orzeczeń Sądów Powszechnych: https://orzeczenia.ms.gov.pl/content/$N/154505000000603_II_C_000121_2011_Uz_2011-04-08_001
8. Sąd Okręgowy w Warszawie, postanowienie z 11 września 2017 r., XXV C 1529/15, Portal Orzeczeń Sądów Powszechnych: https://orzeczenia.ms.gov.pl/content/$N/154505000007503_XXV_C_001529_2015_Uz_2017-09-11_001
9. Sąd Okręgowy w Warszawie, postanowienie z 16 grudnia 2020 r., XXIV C 709/15, Portal Orzeczeń Sądu Okręgowego w Warszawie: https://orzeczenia.warszawa.so.gov.pl/content/$N/154505000007203_XXIV_C_000709_2015_Uz_2021-01-18_001
10. Sąd Apelacyjny w Łodzi, wyrok z 4 lipca 2025 r., I ACa 202/25, Portal Orzeczeń Sądu Apelacyjnego w Łodzi: https://orzeczenia.lodz.sa.gov.pl/content/47/152500000000503_I_ACa_000202_2025_Uz_2025-07-04_001
11. Rejestr podmiotów upoważnionych do wytaczania powództw grupowych, Urząd Ochrony Konkurencji i Konsumentów: https://uokik.gov.pl/bip/rejestr-podmiotow-upowaznionych-do-wytaczania-powodztw-grupowych
12. Overview of pre-notified and notified eID schemes under eIDAS, European Commission: https://ec.europa.eu/digital-building-blocks/sites/display/EIDCOMMUNITY/Overview+of+pre-notified+and+notified+eID+schemes+under+eIDAS

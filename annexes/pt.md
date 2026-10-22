# Annex PT: Portugal (ação popular and DL 114-A/2023)

VCRS 0.1.0-beta.4. Draft for consultation. Not legal advice. Law and rulings as read on 19 and 21 October 2026 on the Diário da República, the consolidated database of the Procuradoria-Geral Regional de Lisboa, dgsi.pt and the Direção-Geral do Consumidor.

## 1. The regime

A collective damages action for consumers runs as an ação popular under Lei n.º 83/95 (the LAP) and, for actions filed from 6 December 2023 within its scope, under Decreto-Lei n.º 114-A/2023, which transposes the Representative Actions Directive and leaves the LAP as subsidiary law (art. 21). Competition damages follow Lei n.º 23/2018, art. 19.

The DL governs actions 'intentadas com fundamento em infrações (...) às disposições do direito nacional e da União Europeia (UE) referidas no anexo I da Diretiva' (art. 2(1)), and only those filed from its entry into force on 6 December 2023: it 'aplica-se às ações coletivas intentadas a partir da data da sua entrada em vigor' (art. 24(1), with art. 25). Its rules on people abroad and on unclaimed sums hold in those actions alone. The export states whether the action is one (`directive`, core 4.6).

- **Who may sue.** Under the DL: associations and foundations with legal personality, statutes that cover the interests and no competing professional activity, and local authorities (DL arts. 5 and 6(1)). Under the LAP alone, also any citizen in full enjoyment of civil and political rights (LAP art. 2(1)); associations and foundations must meet LAP art. 3. A domestic action needs no designation: standing does not depend on 'data em que tenham sido criadas, ao número de membros que tenham ou suficiência de fundos' (Tribunal da Relação de Lisboa, 10 October 2024, proc. 4834/23.0T8VNG.L1-6). Designation by the Direção-Geral do Consumidor (DGC) is for cross-border actions only (DL art. 7); DECO and Ius Omnibus are designated.
- **Independence.** The claimant alone decides to sue, withdraw or settle (DL art. 6(1)(d) and (2)); a funder 'não pode impor, impedir ou influenciar por qualquer forma' those decisions, and clauses to the contrary are void (art. 10(5)). In opt-out actions the funder's return may not exceed 'um valor justo e proporcional' (art. 10(6)).

## 2. Who is bound, and how they join

- **Residents: opt-out.** The claimant represents every holder of the interests 'com dispensa de mandato ou autorização expressa' (LAP art. 14). The court cites the class by public notice 'sem obrigatoriedade de identificação pessoal dos destinatários' (art. 15(2)), by reference to its universe (art. 15(3)). Silence is acceptance (art. 15(1)). A member may refuse representation 'até ao termo da produção de prova (...) por declaração expressa nos autos' (art. 15(4)).
- **People living abroad, in an action under the DL: opt-in.** Consumers without habitual residence in Portugal on the date of the citação are represented only if they 'manifestarem expressamente a sua vontade de serem representados na ação coletiva em causa' (DL art. 12(1)). That expression 'não se encontra sujeita a qualquer formalidade especial' (art. 12(2)). The citação date fixes when residence is tested. It is not a deadline: the statute names none, names no addressee, and does not say whether the opt-in can be withdrawn.
- **People living abroad, in an action under the LAP or Lei n.º 23/2018 alone.** No statute asks them to opt in: the LAP represents 'todos os demais titulares dos direitos ou interesses em causa' (art. 14) without a rule on residence, and Lei n.º 23/2018 art. 19 adds none. In a follow-on case against a defendant seated in Spain, the defendant argued that Portuguese courts lacked jurisdiction over damages that consumers not resident in Portugal suffered 'em resultado dos factos objeto da DECISÃO', and the court recorded the point as undisputed: 'É efetivamente pacífico tal entendimento conforme resulta dos pedidos efetuados e a Autora esclarece na sua resposta' (the Tribunal da Concorrência, Regulação e Supervisão, as transcribed in Tribunal da Relação de Lisboa, 13 July 2022, proc. 6/21.6YQSTR-A.L1-PICRS, paras. 78-79). The point turned on the defendant's seat; no ruling read decides it for a defendant domiciled in Portugal.
- **Practice.** The six court notices read from the DGC's list of ongoing actions all confine the class to residents of Portugal, so a person abroad is outside the class (core 4.1 (4)). Joining the association is voluntary and no condition of representation: Ius Omnibus invites represented consumers to register so they are informed and 'não perdem a oportunidade de pedir a sua indemnização'.

## 3. When the register is tested

| Stage | What it asks of the register | Source |
|---|---|---|
| Filing | Residents: no list of members. A pleaded, plausible class size and damage, and documents showing the practice reached consumers. A foreign qualified entity: the consumers it represents, individually or by category | STJ 2 June 2026; TRL 20 November 2025; LAP art. 13; DL art. 9(1) |
| Citação of the class | In an action under the DL, residence of people abroad is tested at this date, and their opt-in must be evidenced | DL art. 12(1) |
| Close of evidence | Last moment for a resident to refuse representation, in the court file | LAP art. 15(4) |
| Judgment | The court sets the criteria for identifying consumers and quantifying each identified consumer's damage, a global sum for the unidentified, a paying entity, and how consumers are told and claim | DL art. 16(1), (2), (4), (5); LAP art. 22(2) |
| Distribution | Each consumer proves membership and damage by the judgment's criteria, within the judge's period. The right becomes time-barred (prescreve) three years after the judgment becomes final. Under the DL, sums unclaimed within the judge's period pay the claimant's costs, a funder's return among them where the court finds it fair and proportionate. Under Lei n.º 23/2018 they pay the 'custas, encargos, honorários e demais despesas incorridos pelo autor', and the article names no funder. Under the LAP alone, sums for time-barred rights go to the Ministério da Justiça | DL art. 16(6) and (7); Lei n.º 23/2018 art. 19(7); LAP art. 22(3), (4) and (5) |

**Reference dates.** The filing date for the mass-situation pleading; the citação for residence of people abroad; and, at distribution, the claim date within the judge's period. No Portuguese opt-out damages action has reached a court-ordered distribution yet.

## 4. Required items

A register that claims a level in a Portuguese action meets every item below. Each is what Portuguese law requires; this annex asks nothing beyond it.

### What the law requires

| # | Item | Core | Source |
|---|---|---|---|
| PT-1 | In an action under the DL, for a person abroad: their residence on the date of the citação, and their express will to be represented in this action, with when and how it was given. No form is required beyond that. There is no opt-in window: the export states `opt_in_opened_on` and `opt_in_closed_on` as null, and the express will is due from the start. The export states `directive` as true in such an action and as false in an action under the LAP or Lei n.º 23/2018 alone, where no opt-in is asked | 4.6 | DL art. 2(1), 12(1) and (2), 24(1) |
| PT-2 | A resident's refusal of representation takes effect in law only by the person's own express declaration in the court file. A refusal sent to the association alone takes the record out of the count as withdrawn (core 4.1 (1)); the record notes that the person stays represented in law until they file it | 4.1 (1) | LAP art. 15(1) and (4) |
| PT-3 | A foreign qualified entity gives the court 'informações suficientes sobre os consumidores representados na ação coletiva, identificados individualmente ou, quando não seja viável a sua individualização, por categoria' | 6.2, 6.3 | DL art. 9(1) |
| PT-4 | At distribution: each claim recorded against the identification criteria and the proof the judgment names, with the claim date within the period the judge sets | 4.3, 5.3 | DL art. 16(1), (5), (6) in an action under the DL; Lei n.º 23/2018 art. 19(3) and (7); LAP art. 22(2) and (3) |
| PT-5 | The sign-up flow offers no legal advice on a person's own claim unless the operator is entitled to give it (Lei n.º 10/2024 arts. 4 and 7), and does not advertise court representation or any other act of lawyers that the operator is not authorised to practise | 5.1 | Lei n.º 10/2024 art. 12(1) ('a promoção, divulgação ou publicidade de atos próprios, exclusivos ou não, dos advogados ou dos solicitadores, quando efetuada por pessoas (...) não autorizadas a praticar os mesmos'), art. 11(2), art. 6(1) and art. 4(2) |

## 5. Recommended items

- **A class size with its method, and the register's coverage against it, at filing.** The Supremo Tribunal de Justiça refused an action where 'nada tendo sido alegado quanto à dimensão do dano e ao número dos consumidores lesados', and requires a mass situation: 'um conjunto provável e relevante de consumidores' (STJ 2 June 2026, proc. 3650/23.3T8BRG.G1.S1, sumário II and III). It added that nobody keeps receipts for such purchases, which made any award impossible. A register that holds members and their proof answers both points.
- **A sample of members' documents at filing.** The Relação de Lisboa required 'contratos (ou de contrato-tipo) onde constem as cláusulas em causa e de onde resulte, ao menos indiciariamente, que foram celebrados contratos' (TRL 20 November 2025, proc. 20156/23.3T8LSB.L1-6, sumário VI), under the preliminary filter of LAP art. 13.
- **Subgroup coding.** An action fails where the defendant can raise personal defences against some members (STJ 6 July 2023, proc. 26412/16.0T8LSB.L2.S1, sumário III; TRL 26 March 2026, proc. 6308/22.7T8VNG.L1-8). Records coded by subgroup let the court see the claims are homogeneous.
- **The register under the association's exclusive control, with no funder access to decisions or member data.** Independence can be put to proof: in one action the trial court listed whether the claimant 'é ou não independente do terceiro financiador' among the issues for proof (as reproduced in TRG 5 February 2026, proc. 406/24.0T8BRG-A.G1). Under DL 114-A/2023 it is a condition of standing (arts. 6(1)(d) and 10(8)); for an action under the LAP alone the Relação de Lisboa held that no further standing requirement may be imposed (TRL 24 September 2026, proc. 5392/23.0T8VNG.L1-6, sumário III). The competition court has asked the Court of Justice whether a funder repaid from unclaimed money conflicts with the class, since how consumers claim and what they must prove decide how many claim (TCRS 10 March 2026, proc. 3/24.0YQSTR, para. 35; C-431/26, pending). Inference: a register that makes claiming easy serves the class against the funder's interest in what goes unclaimed.
- **Individual identification before judgment.** A consumer identified to the court can have their damage quantified in the judgment and shares pro rata if the global sum falls short (DL art. 16(1) and (3); in a competition action Lei n.º 23/2018 art. 19(3) and (5)), and is then compensated 'nos termos gerais da responsabilidade civil' (LAP art. 22(3)).
- **Notice tracking**, so the court can order direct notice and the claimant can show reach (DL art. 16(5), in an action under the DL).
- **Distribution records kept at least until the right to compensation is time-barred**, three years after the judgment becomes final (LAP art. 22(4)).
- **A legal basis per record under the GDPR**, and for privacy damages an art. 80(1) mandate (Lei n.º 58/2019 art. 35), until a court settles whether opt-out applies to those claims.

## 6. Recognised identification

- **Identity, grade A**: Cartão de Cidadão and Chave Móvel Digital, both notified under eIDAS at assurance level high, and so covered by `eidas`. `pt.json` names no further scheme.
- **Outside sources, grade B**: none named yet. Supplied documents (contracts, invoices) are the evidence courts have asked for.

## 7. The level a typical action needs

A recommendation, not a court's rule.

- **Residents, to be admitted**: no level is required. Level 1, Registered, with a sample of documents, answers the Supremo Tribunal's mass-situation test.
- **People abroad, in an action under the DL, to be bound**: Level 2, Identified. A named person, a residence, an express will tied to the action.
- **Everyone, to be paid**: Level 3, Verified, against the proof the judgment names, because payment runs on individual entitlement and the paying entity checks each claim.

## 8. Unsettled

- Whether art. 12 DL reaches a competition damages action pleaded under the DL and, in the alternative, Lei n.º 23/2018. In one such action the court cited the class 'nos termos e para os efeitos dos artigos 12.º(1) e 21.º da LAC e do artigo 15.º da LAP', the LAC being the DL, and confined it to 'todos os consumidores, com residência em Portugal' (Tribunal da Concorrência, Regulação e Supervisão, proc. 5/26.1YQSTR, notice of 25 May 2026). A register in such an action states `directive` as true, so a person abroad counts only on an opt-in.
- The deadline, addressee and revocability of an opt-in from abroad. Every court notice read requires a lawyer for statements in the file; whether art. 12(2) displaces that is untested.
- When the citação of an unidentified class takes effect: the day the notice is published, or the end of the dilação.
- What proof courts will demand at distribution. No action has reached it.
- C-431/26 (Ius Omnibus v ABANCA), on funder-dependent associations and funders repaid from unclaimed money.
- Whether GDPR damages may proceed by opt-out ação popular or need a mandate.
- The Supremo Tribunal's mass-situation line and the Relação panels that admitted single-store price actions (TRL 5 November 2025, proc. 1990/23.0T8VCT.L1-2; TRL 27 January 2026, proc. 1085/23.7T8PVZ.L1-7) point different ways; how the line applies to large online classes is open.

## Sources

1. Decreto-Lei n.º 114-A/2023: https://diariodarepublica.pt/dr/detalhe/decreto-lei/114-a-2023-225265456
2. Lei n.º 83/95, consolidated: https://diariodarepublica.pt/dr/legislacao-consolidada/lei/1995-34534075
3. Lei n.º 10/2024: https://www.pgdlisboa.pt/leis/lei_mostra_articulado.php?nid=3758&tabela=leis&so_miolo=
4. Lei n.º 58/2019: https://www.pgdlisboa.pt/leis/lei_mostra_articulado.php?nid=3118&tabela=leis&so_miolo=
5. DGC, ações coletivas em curso, with the court notices: https://www.consumidor.gov.pt/consumidor_4/acoes-coletivas/acoes-em-curso
6. DGC, designated qualified entities: https://www.consumidor.gov.pt/upload/processos/i007227.pdf
7. STJ 2 June 2026, proc. 3650/23.3T8BRG.G1.S1: https://www.dgsi.pt/jstj.nsf/954f0ce6ad9dd8b980256b5f003fa814/8a9c7ee81d3e51fa80258e1300395c20?OpenDocument
8. STJ 6 July 2023, proc. 26412/16.0T8LSB.L2.S1: https://www.dgsi.pt/jstj.nsf/954f0ce6ad9dd8b980256b5f003fa814/0693f6bec3be6be4802589e5004ed2c3?OpenDocument
9. TRL 20 November 2025, proc. 20156/23.3T8LSB.L1-6: https://www.dgsi.pt/jtrl.nsf/33182fc732316039802565fa00497eec/db85428e48d17c1280258d4f0041c240?OpenDocument
10. TRL 10 October 2024, proc. 4834/23.0T8VNG.L1-6: https://www.dgsi.pt/jtrl.nsf/33182fc732316039802565fa00497eec/ea03a6eb16fe944a80258bbf003a549d?OpenDocument
11. TRL 26 March 2026, proc. 6308/22.7T8VNG.L1-8: https://www.dgsi.pt/jtrl.nsf/33182fc732316039802565fa00497eec/72d67e75afbe472180258dcb004aa5d8?OpenDocument
12. TRG 5 February 2026, proc. 406/24.0T8BRG-A.G1: https://www.dgsi.pt/jtrg.nsf/86c25a698e4e7cb7802579ec004d3832/2a64963a4d0ba02780258d9a00390140?OpenDocument
13. TCRS 10 March 2026, proc. 3/24.0YQSTR, reference to the Court of Justice (C-431/26): https://juris.curia.europa.eu/juris/showPdf.jsf?text=&docid=312738&pageIndex=0&doclang=PT&mode=req&dir=&occ=first&part=1
14. eIDAS notified scheme, Portugal, Chave Móvel Digital: https://ec.europa.eu/digital-building-blocks/sites/spaces/EIDCOMMUNITY/pages/78555712/Portugal+-+Chave+M%C3%B3vel+Digital
15. eIDAS notified scheme, Portugal, Cartão de Cidadão: https://ec.europa.eu/digital-building-blocks/sites/spaces/EIDCOMMUNITY/pages/78555468/Portugal+-+Cart%C3%A3o+de+Cidad%C3%A3o
16. Lei n.º 23/2018, art. 19: https://www.pgdlisboa.pt/leis/lei_mostra_articulado.php?nid=2899&tabela=leis&so_miolo=
17. Ius Omnibus v JNTL, case page: https://www.iusomnibus.eu/pt/os-nossos-casos/ius-omnibus-v-jntl-retalho/
18. TRL 5 November 2025, proc. 1990/23.0T8VCT.L1-2: https://www.dgsi.pt/jtrl.nsf/33182fc732316039802565fa00497eec/8d5ab360d6ea0f6d80258d41004e60e9?OpenDocument
19. TRL 27 January 2026, proc. 1085/23.7T8PVZ.L1-7: https://www.dgsi.pt/jtrl.nsf/33182fc732316039802565fa00497eec/1578e0efe43d567b80258d96003fd5e6?OpenDocument
20. TRL 24 September 2026, proc. 5392/23.0T8VNG.L1-6: https://www.dgsi.pt/jtrl.nsf/33182fc732316039802565fa00497eec/45922e4fd22b97c780258e83004d17fb?OpenDocument
21. TRL 13 July 2022, proc. 6/21.6YQSTR-A.L1-PICRS: https://www.dgsi.pt/Jtrl.nsf/e6e1f17fa82712ff80257583004e3ddc/301d62feb48b59d6802588ad00396601?OpenDocument

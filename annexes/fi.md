# Annex FI: Finland (ryhmäkanne under the ryhmäkannelaki)

VCRS 0.1.0-beta.6. Draft for consultation. Not legal advice. Law as read on 19 and 21 October 2026 on Finlex, the Kilpailu- ja kuluttajavirasto's publications and the European Commission's list of qualified entities and overview of notified eID schemes.

Written by Holly Thackwray and Mischa Sigtermans for Steddle. Not yet reviewed by counsel admitted in Finland.

## 1. The regime

A collective damages action is a ryhmäkanne under the ryhmäkannelaki (444/2007), which transposes the Directive as amended by 1103/2022, in force since 25 June 2023. 'Tätä lakia sovelletaan kuluttaja-asiamiehen toimivallan mukaisessa laajuudessa kuluttajan ja elinkeinonharjoittajan välisen riita-asian käsittelyyn ryhmäkanteena' (1 § 1 mom), and to the claims for redress of Directive (EU) 2020/1828 (1 § 2 mom). Actions pending on that day keep the earlier rules: 'Ennen tämän lain voimaantuloa vireillä olleiden asioiden käsittelyyn sovelletaan tämän lain voimaan tullessa voimassa olleita säännöksiä' (1103/2022, voimaantulosäännös), and before it only the Kuluttaja-asiamies could sue.

- **Who may sue.** A qualified entity: 'Jäljempänä 4 a §:ssä tarkoitettu oikeutettu yksikkö panee kantajana vireille ryhmäkanteen ja käyttää siinä asianosaisena puhevaltaa' (4 §). Under 4 a § that is the Kuluttaja-asiamies 'valvontavaltaansa kuuluvassa asiassa', a consumer organisation 'jonka oikeusministeriö on nimennyt oikeutetuksi yksiköksi tässä laissa tarkoitettuja ryhmäkanteita varten', and a qualified entity of another EEA state on the Commission's list. On 21 October 2026 the Commission's list named one Finnish organisation, Kuluttajaliitto ry, beside seven authorities. There is no entity formed for one action.
- **Court.** 'Ryhmäkanneasioissa toimivaltainen käräjäoikeus on Helsingin käräjäoikeus, jonka tuomiopiirinä on koko maa' (3 §).
- **The conditions.** 'Asia voidaan käsitellä ryhmäkanteena, jos: 1) useilla henkilöillä on samaa vastaajaa vastaan vaatimuksia, jotka perustuvat samoihin tai samankaltaisiin seikkoihin; 2) asian käsittely ryhmäkanteena on tarkoituksenmukaista ottaen huomioon ryhmän koko, asiassa esitettävien vaatimusten sisältö ja asiassa esitettävä todistelu; sekä 3) ryhmä on riittävän täsmällisesti määritelty' (2 §). The act sets no minimum number. The court gives no separate ruling on them and may dismiss on them at any stage (HE 154/2006 vp, on 2 §).
- **Funding.** 'Ryhmäkanteen ulkopuolinen rahoittaja ei saa olla ryhmäkanteen vastaajan kilpailija tai vastaajasta riippuvainen' (2 a § 1 mom); the claimant explains its funding when there are grounded doubts (2 a § 2 mom).

## 2. Who is bound, and how they join

- **Opt-in, for everyone.** 'Määritelmän mukainen ryhmän jäsen, joka asetetussa määräajassa on toimittanut kantajalle kirjallisen ilmoituksen halukkuudestaan osallistua ryhmäkanteeseen, kuuluu ryhmään' (8 § 1 mom), and 'Tuomioistuimen ratkaisu sitoo niitä ryhmän jäseniä, joita tuomioistuin on ratkaisussaan ilmoittanut sen koskevan' (16 §). The act draws no line by residence, so residents and people abroad both opt in: `fi.json` sets `opt_in_abroad` and `opt_in_residents` to true, names the claimant as the channel, `qe`, and asks no declaration on parallel claims, which the act does not provide for.
- **The window.** 'Lisäksi tuomioistuimen on asetettava määräaika ryhmään ilmoittautumiselle. Tuomioistuin voi erityisestä syystä pidentää määräaikaa' (6 § 1 mom). The court sets it after the action is filed and before the summons issues. `fi.json` sets `opt_in_window` to true. The export states the period as a term (`opt_in_terms`), from the day the court set it to its last day as the court set or extended it. Until the period closes a record counts on its other facts; after it, a record counts only with a written notice that reached the claimant within the period.
- **A late notice.** 'Jos määritelmän mukainen jäsen ilmoittautuu ryhmään asetetun määräajan jälkeen, mutta ennen kuin täsmennetty haastehakemus on toimitettu tuomioistuimelle, kantaja voi erityisestä syystä hyväksyä hänet ryhmän jäseneksi' (8 § 2 mom). The export states the court's period, so the validator does not count such a member (section 8).
- **The form.** A written notice to the claimant. Since 1103/2022 it need not be signed: the government bill struck the signature because it 'ei ole nyky-yhteiskunnassa toimiva menettelytapa' (HE 111/2022 vp, p. 83).
- **The fee.** 'Jos kanteen on nostanut oikeutetuksi yksiköksi nimetty järjestö, kantaja voi edellyttää ryhmäkanteeseen osallistuvalta kohtuullisen ilmoittautumismaksun suorittamista' (8 § 1 mom). The Kuluttaja-asiamies charges none.
- **The notice to members.** 'Kantajan on viipymättä ilmoitettava tiedossa oleville ryhmän jäsenille asian vireilletulosta. Ilmoitus on toimitettava postitse tai sähköisesti' (6 § 2 mom), with 'tieto siitä, miten ryhmään ilmoittaudutaan ja ilmoittautumiselle asetetusta määräajasta sekä mahdollisesta ilmoittautumismaksusta' (7 § 1 mom 4 kohta).
- **Withdrawal, to the court.** 'Ryhmän jäsen voi ennen asian siirtämistä pääkäsittelyyn irrottautua ryhmästä ilmoittamalla siitä kirjallisesti tuomioistuimelle tai sen kansliaan' (15 § 1 mom); after the transfer only with the defendant's consent, and 'Kun asia on jätetty päätettäväksi, ryhmästä ei voi enää irrottautua' (15 § 2 mom).
- **Who holds the list.** The claimant takes the notices and files the list in the refined summons (9 §). The court holds the refined summons, the withdrawals and the judgment's list of the members bound. No court registry or state portal takes notices.

## 3. When the register is tested

| Stage | What it asks of the register | Source |
|---|---|---|
| Filing | The group, the known claims, why group treatment fits, and the facts the claimant knows that matter only for some members. No names | 5 § 1 mom |
| Notice and period | The court tells the parties and sets the period for joining; the claimant notifies the known members by post or electronically, with how to join, the deadline and any fee | 6 § 1, 2 mom; 7 § 1 mom |
| Joining | A written notice to the claimant inside the period, from a person within the definition, with any fee the claimant requires paid | 8 § 1 mom |
| Refined summons | Each member's name, address and individualised claim, within one month of the period's end. The summons issues only after it | 9 §; 10 § 1 mom |
| Preparation | Before the refined summons, a claim the claimant drops ends; after it, the member may go on alone. Withdrawals reach the court | 13 §; 15 § 1 mom |
| Main hearing | A member withdraws only with the defendant's consent, and not at all once the case is submitted for decision | 15 § 2 mom |
| Judgment | Binds the members the court names in it, each with an award; the claimant tells the members | 16 §; 15 a § 1 mom |
| Settlement | Binds the members once the court confirms it | HE 111/2022 vp, p. 32 |

**Reference dates.** The last day of the period, with the list the refined summons files within a month after it (9 §). After that the list only shrinks (13 §, 15 §) or grows by a wider definition during preparation (12 § 1 mom). No ryhmäkanne had been filed by 19 October 2026: the Kilpailu- ja kuluttajavirasto wrote in 2021 that 'yhtään ryhmäkannetta ei tuomioistuimessa ole vielä koskaan nostettu', and no later filing was found.

## 4. Required items

A register that claims a level in a Finnish action meets every item below. The first table holds what Finnish law requires. The second holds what this standard requires beyond the law, with the reason.

### What the law requires

| # | Item | Core | Source |
|---|---|---|---|
| FI-1 | Each record holds the facts that place the person within the group the summons defines | 4.2, 4.3, 6.1 | 8 § 1 mom: 'Määritelmän mukainen ryhmän jäsen'; 2 § 3 kohta: 'ryhmä on riittävän täsmällisesti määritelty' |
| FI-2 | Each record holds its opt-in: the day the person's written notice reached the claimant, through the channel `qe`, within the period the court set. A sign-up taken before the court set the period, such as a pre-registration, is not that notice | 4.1 (8), 4.6, 5.3 | 8 § 1 mom: 'joka asetetussa määräajassa on toimittanut kantajalle kirjallisen ilmoituksen halukkuudestaan osallistua ryhmäkanteeseen, kuuluu ryhmään'; 6 § 1 mom: 'Lisäksi tuomioistuimen on asetettava määräaika ryhmään ilmoittautumiselle.' |
| FI-3 | A notice that reached the claimant after the period holds the claimant's decision on it: admitted for a special reason before the refined summons was filed, with the reason, or refused and recorded `excluded` | 4.1 (1), 4.6 | 8 § 2 mom: 'mutta ennen kuin täsmennetty haastehakemus on toimitettu tuomioistuimelle, kantaja voi erityisestä syystä hyväksyä hänet ryhmän jäseneksi' |
| FI-4 | Where the claimant requires a sign-up fee, the amount, the day it was paid, and the notice that announced it. A person who did not pay a fee the claimant required is recorded `excluded` | 4.1 (1), 9 | 8 § 1 mom: 'kantaja voi edellyttää ryhmäkanteeseen osallistuvalta kohtuullisen ilmoittautumismaksun suorittamista'; 7 § 1 mom 4 kohta |
| FI-5 | Each member's name, address and individualised claim, exportable as the list of the refined summons within one month of the period's end | 4.2, 6.5 | 9 §: 'Kantajan on laadittava täsmennetty haastehakemus, joka sisältää jäsenten nimet ja osoitteet sekä yksilöidyt vaatimukset ja, jos se on tarpeellista, täsmennetyt perusteet. Haastehakemus on toimitettava tuomioistuimelle kuukauden kuluessa ryhmään ilmoittautumiselle asetetusta määräajasta.' |
| FI-6 | A record that the claimant notified the known members by post or electronically, with the notice's content, and any notice in a newspaper or by other means | 5.1 | 6 § 2 mom: 'Ilmoitus on toimitettava postitse tai sähköisesti. Jos ilmoitusta ei mainituin tavoin voida toimittaa kaikille määritelmän mukaisille ryhmän jäsenille, ryhmäkanteesta voidaan ilmoittaa yhdessä tai useammassa sanomalehdessä taikka muulla asianmukaisella tavalla.'; 7 § 1 mom |
| FI-7 | A withdrawal is recorded `withdrawn` with the day the member gave written notice to the court, taken from the court's record, and after the transfer to the main hearing the defendant's consent | 4.1 (1), 5.3 | 15 § 1 mom: 'ilmoittamalla siitä kirjallisesti tuomioistuimelle tai sen kansliaan'; 15 § 2 mom: 'ryhmän jäsen voi vain vastaajan suostumuksella 1 momentissa säädetyllä tavalla irrottautua ryhmästä' |
| FI-8 | A claim the claimant drops is recorded `excluded` with its day: before the refined summons it ends; after it, the record holds whether the member went on alone | 4.1 (1) | 13 § 1 mom: 'tuomioistuimen on tältä osin jätettävä kanne sillensä'; 13 § 2 mom |
| FI-9 | The members the judgment names, each with the award stated for them, and a contact channel through which the claimant tells them of it | 4.1 (7), 5.3 | 16 §; 15 a § 1 mom: 'Kantaja ilmoittaa ryhmän jäsenille annetusta tuomiosta ja muista tuomioistuimen ratkaisuista.' |

### What this standard requires

| # | Item | Core | Reason |
|---|---|---|---|
| FI-10 | Each notice states why the person is a member, the claim, the facts behind it and any evidence | 4.3, 6.5 | The act asks only for a written notice, but the government bill expects more: 'Ryhmään liityttäessä olisi ilmoitettava, millä perusteella ilmoittautuja katsoo olevansa ryhmän jäsen.' The claimant accepts a notice on the information it gives, and 'Puutteelliset tai epäselvät ilmoittautumiset johtaisivat ryhmän ulkopuolelle jättämiseen' (HE 154/2006 vp, on 8 §). The refined summons needs each claim individualised (9 §) |

## 5. Recommended items

- **The evidence behind each claim and its amount.** The judgment states what each member receives, and 'Viime kädessä tuomioistuin ratkaisisi ryhmän jäsenyyttä koskevan kysymyksen' (HE 154/2006 vp, on 8 §).
- **For an electronic notice, the sender's identity and the document's integrity.** Where the Kuluttaja-asiamies is the claimant, an electronic notice to it meets the written form without a signature if it identifies the sender and its origin and integrity are not in doubt (HE 111/2022 vp, p. 83).
- **Pre-registration kept apart from joining.** The Kuluttaja-asiamies ran a pre-registration in 2019 to see whether the group would be large enough, before any action was filed. Such support shows in the cross-section (6.3), and each person still joins within the court's period (FI-2).
- **An enforcement mandate, and payee details.** Each member enforces their own award (HE 154/2006 vp, on 16 §), so where the claimant is to collect for members it needs a mandate, and a settlement paid through the claimant needs each member's account.
- **A funding file ready for a 2 a § request.**
- **An operator receiving notices for the claimant.** Each written notice is addressed to the claimant by name, at a channel the claimant publishes as its own; the operator receives it as the claimant's processor under a written mandate to receive; the opt-in's day is the day the claimant had it, and the register keeps the day the operator received it. A notice falls within the court's period only where the claimant had it in time (8 § 1 mom). This lowers the risk of the question section 8 leaves open; it does not settle it.

## 6. Recognised identification

- **Identity, grade A**: the Citizen Certificate on the Finnish identity card, notified under eIDAS at assurance level high (the European Commission's overview of notified schemes: C/2025/2448), and so covered by `eidas`. No other Finnish scheme is notified, and `fi.json` names no further one.
- **Outside sources, grade B**: none named. No Finnish court has yet examined a list of members.

## 7. The level a typical action needs

A recommendation, not a court's rule.

- **Level 3, Verified, for the refined summons in a damages action.** The judgment names each member and states each award (16 §), the claimant accepts each notice and the court decides membership in the end (HE 154/2006 vp, on 8 §), and the defendant can contest each member once served.
- **Level 2, Identified, is the floor** the refined summons sets: each member's name, address and individualised claim (9 §).

## 8. Unsettled

- No ryhmäkanne has been filed, so no court has set a period, read a refined summons or ruled on a member.
- Two kinds of lawful member are undercounted, because the export states the court's period alone: a member the claimant admits late for a special reason under 8 § 2 mom, and a new member a definition widened during preparation brings in under 12 § 1 mom. The validator grades both D (`not_opted_in`); the register shows them apart, and the auditor reports them.
- Whether a notice that reached the claimant after the action was filed but before the court set the period counts. FI-2 reads 8 § 1 mom as asking for a notice within the period.
- Whether a third party may receive notices for the claimant: 8 § sends them to the claimant, and no source read addresses an agent.
- Whether members' names and addresses in the refined summons are public in the court's file.

## Sources

1. Ryhmäkannelaki 444/2007, consolidated text, Finlex, Oikeusministeriö: https://www.finlex.fi/fi/lainsaadanto/2007/444
2. Laki ryhmäkannelain muuttamisesta 1103/2022, with its transitional rule, Suomen säädöskokoelma, Finlex: https://www.finlex.fi/fi/lainsaadanto/saadoskokoelma/2022/1103
3. HE 154/2006 vp, the government bill for the ryhmäkannelaki, Finlex: https://www.finlex.fi/fi/hallituksen-esitykset/2006/154
4. HE 111/2022 vp, the government bill transposing Directive (EU) 2020/1828, Finlex: https://www.finlex.fi/fi/hallituksen-esitykset/2022/111
5. Pikaluottojen ryhmäkanne: kuluttaja-asiamiehen neuvottelut päättyivät hyvitysten maksamiseen, 17 March 2021, Kilpailu- ja kuluttajavirasto: https://www.kkv.fi/ajankohtaista/tiedotteet/pikaluottojen-ryhmakanne-kuluttaja-asiamiehen-neuvottelut-j-w-yhtioiden-ja-weststarin-kanssa-paattyivat-hyvitysten-maksamiseen/
6. Kuluttaja-asiamies puuttuu pikaluottojen kohtuuttomiin kustannuksiin, ennakkoilmoittautuminen ryhmäkanteeseen alkaa, 23 October 2019, Kilpailu- ja kuluttajavirasto: https://www.kkv.fi/ajankohtaista/tiedotteet/kuluttaja-asiamies-puuttuu-pikaluottojen-kohtuuttomiin-kustannuksiin-ennakkoilmoittautuminen-ryhmakanteeseen-alkaa/
7. Cross-border qualified entities, Finland, European Commission: https://justice-collaboration-platform.ec.europa.eu/cross-border-qualified-entities
8. Overview of pre-notified and notified eID schemes under eIDAS, European Commission: https://ec.europa.eu/digital-building-blocks/sites/display/EIDCOMMUNITY/Overview+of+pre-notified+and+notified+eID+schemes+under+eIDAS

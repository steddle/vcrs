# Conformance statement

VCRS 0.1.0-beta.6, core and Annex <XX>. One page, no personal data. The same content as JSON follows `schema/conformance.schema.json`.

| | |
|---|---|
| Representative | <name, registration number> |
| Action | <title>, against <defendants>, <court and case number>, <under the forum's transposition of Directive (EU) 2020/1828, or not> |
| Operator | <name> |
| Level claimed | <Registered, Identified or Verified> |
| Reference date | <YYYY-MM-DD> |
| Denominator | <low> to <high>, from <source>, as of <date> |

## Records at the reference date

| Grade | Records | Coverage |
|---|---:|---:|
| A or better | | |
| B or better | | |
| C or better | | |
| C, membership not established | | |
| D, active | | |
| D, not active | | |

Each row from A to C counts the active records at that grade or better (core 6.2). A record that is not active is grade D (core 4.1 rule 1) and counts in the last row alone, so C or better and the two rows at D add up to the records in the snapshot. The row C, membership not established counts the records at grade C whose evidence does not establish that the person is in the class (core 4.3); they are part of C or better.

These figures describe the representative's register. They do not establish whom the law or the court treats as represented or bound: that follows from the applicable law and the court's orders (the annex, section 2).

## Coverage per subgroup and per part

Where the class has subgroups (core 6.4) or the claim is split into parts (core 4.6), the coverage of each against a denominator of its own. A record in both parts counts in each.

| Subgroup or part | Denominator | A or better | B or better | C or better |
|---|---|---:|---:|---:|
| <name> | <low> to <high>, from <source>, as of <date> | | | |

## The snapshot

| | |
|---|---|
| Records in the snapshot | |
| Snapshot root | sha256:<64 hex> |
| Manifest | sha256:<64 hex> |
| Anchored by | <notary, qualified timestamp or OpenTimestamps>, <reference>, <date> |

## The independent check

| | |
|---|---|
| Auditor | <firm> |
| Standard | <ISRS 4400 or Standaard 4400N for agreed-upon procedures, ISAE 3000 or its national equivalent for assurance> |
| Engagement | <agreed-upon procedures, which report what the auditor found and give no assurance, or an assurance engagement, which ends in the auditor's conclusion> |
| Check | <sample tracing, full recomputation or reproduction test> |
| Report dated | <YYYY-MM-DD> |

The board of <representative> approved the class definition, every version of the sign-up flow and this statement on <date>.

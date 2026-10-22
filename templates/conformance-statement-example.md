# Conformance statement: an example

VCRS 0.1.0-beta.4, core and Annex NL. The [conformance statement](conformance-statement.md) filled in for the example register in [register.json](register.json) and [records.csv](records.csv). The representative, the defendant, the operator and the auditor are fictional. The figures are the example register's: eight records against a class of 21 000 to 26 000, so its coverage is a fraction of a percent.

| | |
|---|---|
| Representative | Stichting Voorbeeldclaim, KvK 00000000 |
| Action | Software that was sold and never delivered, against Example Motors B.V., not yet filed, under the forum's transposition of Directive (EU) 2020/1828 |
| Operator | Stichting Voorbeeldclaim |
| Level claimed | Verified |
| Reference date | 2026-10-12 |
| Denominator | 21 000 to 26 000, from RDW open data, registrations of the models concerned, times the take rate of package X in the defendant's annual report, as of 2026-09-01 |

## Records at the reference date

| Grade | Records | Coverage |
|---|---:|---:|
| A or better | 1 | 0.0038% to 0.0048% |
| B or better | 3 | 0.0115% to 0.0143% |
| C or better | 5 | 0.0192% to 0.0238% |
| D, not counted | 2 | |
| Not active | 1 | |

## The snapshot

| | |
|---|---|
| Records in the snapshot | 8 |
| Snapshot root | sha256:bd16f0dd9c9205fe559998e18a1424442e40f79e0d2f2696c5e9ce986da80cf2 |
| Anchored by | OpenTimestamps, snapshots/2026-10-12.ots, 2026-10-12 |

## The independent check

| | |
|---|---|
| Auditor | Voorbeeld Accountants |
| Standard | Standaard 4400N |
| Check | Reproduction test |
| Report dated | 2026-10-14 |

The board of Stichting Voorbeeldclaim approved the class definition, every version of the sign-up flow and this statement on 15 October 2026.

## As JSON

The same statement, as [`schema/conformance.schema.json`](../schema/conformance.schema.json) sets it out:

```json
{
    "vcrs": "0.1.0-beta.4",
    "annex": "nl",
    "level": "verified",
    "representative": "Stichting Voorbeeldclaim",
    "action": {
        "title": "Software that was sold and never delivered",
        "defendants": [
            "Example Motors B.V."
        ],
        "court_reference": null,
        "directive": true
    },
    "operator": "Stichting Voorbeeldclaim",
    "reference_date": "2026-10-12",
    "denominator": {
        "low": 21000,
        "high": 26000,
        "source": "RDW open data, registrations of the models concerned, times the take rate of package X in the defendant's annual report",
        "as_of": "2026-09-01"
    },
    "claims": {
        "low": 31500000,
        "high": 39000000,
        "currency": "EUR",
        "method": "The price of package X, €1 500 per car, times the denominator"
    },
    "counts": {
        "A": 1,
        "B": 2,
        "C": 2,
        "D": 2,
        "inactive": 1
    },
    "coverage": {
        "A": {
            "records": 1,
            "low": 0.0038,
            "high": 0.0048
        },
        "B": {
            "records": 3,
            "low": 0.0115,
            "high": 0.0143
        },
        "C": {
            "records": 5,
            "low": 0.0192,
            "high": 0.0238
        }
    },
    "snapshot": {
        "root": "sha256:bd16f0dd9c9205fe559998e18a1424442e40f79e0d2f2696c5e9ce986da80cf2",
        "records": 8,
        "anchor": {
            "method": "opentimestamps",
            "reference": "snapshots/2026-10-12.ots",
            "on": "2026-10-12"
        }
    },
    "auditor": {
        "firm": "Voorbeeld Accountants",
        "standard": "Standaard 4400N",
        "report_date": "2026-10-14",
        "check": "reproduction_test"
    },
    "issued_on": "2026-10-15"
}
```

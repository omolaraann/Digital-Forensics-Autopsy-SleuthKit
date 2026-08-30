# Digital Forensics Case Handling, Autopsy and Sleuth Kit Analysis

**Course:** SBT-DF202 — Computer and Digital Forensics
**Practical Lab:** Lab 1
**Platform:** Local Forensic Workstation / Kali Linux or Ubuntu VM + Autopsy
**Evidence Image:** `Ch01InChap01.dd`

---

## 1. Practical Overview

This practical laboratory demonstrates the application of digital forensic investigation procedures using **Autopsy** and **The Sleuth Kit**.

The investigation involves the examination of the authorised forensic disk image `Ch01InChap01.dd`. The objective is to preserve evidence integrity, identify deleted files, recover relevant files, perform keyword searches, analyse file metadata and data units, verify recovered evidence using cryptographic hashes, and document the investigation in a repeatable forensic report.

The original forensic image was preserved and was not modified during the examination.

---

## 2. Objectives

The practical objectives are to:

* Preserve and verify the integrity of the forensic disk image.
* Calculate and document MD5 and SHA-256 hashes.
* Maintain a mini chain of custody/evidence worksheet.
* Create and configure a forensic case in Autopsy.
* Examine the forensic image using Autopsy.
* Identify deleted files.
* Perform keyword searches.
* Tag and recover relevant evidence.
* Analyse the image using The Sleuth Kit command-line tools.
* Identify the metadata address of `INCOME.XLS`.
* Examine file metadata using `istat`.
* Recover `INCOME.XLS` using `icat`.
* Perform block-level recovery using `blkcat` where applicable.
* Perform additional file recovery using `tsk_recover`.
* Compare cryptographic hashes of recovered copies.
* Examine the recovered spreadsheet locally.
* Produce a professional forensic report supported by screenshots and evidence.

---

## 3. Evidence Information

| Item                         | Details                            |
| ---------------------------- | ---------------------------------- |
| Evidence filename            | `Ch01InChap01.dd`                  |
| Evidence type                | Forensic disk image                |
| Evidence source              | Authorised ICDFA training evidence |
| Original location            | To be documented                   |
| File size                    | To be documented                   |
| MD5                          | To be calculated                   |
| SHA-256                      | To be calculated                   |
| Acquisition/examination date | 30 August 2026                     |
| Original image modified      | No                                 |

---

## 4. Tools Used

The following forensic tools and utilities were used during the examination:

* Autopsy
* The Sleuth Kit
* `img_stat`
* `mmls`
* `fsstat`
* `fls`
* `istat`
* `icat`
* `blkcat`
* `blkls`
* `tsk_recover`
* `md5sum`
* `sha256sum`

---

## 5. Investigation Methodology

The investigation was conducted using a structured forensic workflow:

1. Evidence identification and preservation
2. Evidence hashing and integrity verification
3. Chain-of-custody documentation
4. Autopsy case creation
5. Evidence source configuration
6. Deleted-file examination
7. Keyword searching
8. Evidence tagging and recovery
9. Sleuth Kit command-line examination
10. Metadata and data-unit analysis
11. Recovery of `INCOME.XLS`
12. Hash verification and comparison
13. Local examination of recovered evidence
14. Documentation and reporting

---

## 6. Evidence Integrity

Cryptographic hashes were calculated for the original forensic image before analysis.

### Original Evidence Hashes

**MD5:**
`To be documented`

**SHA-256:**
`To be documented`

The original forensic image was preserved throughout the investigation. Recovery, analysis, screenshots and reports were stored separately from the source image.

---

## 7. Autopsy Analysis

Autopsy was used to create and analyse the forensic case.

The following activities were performed:

* Created a forensic case.
* Added `Ch01InChap01.dd` as the evidence source.
* Examined the file system.
* Identified deleted files.
* Performed keyword searches.
* Identified relevant evidence.
* Tagged relevant files.
* Recovered relevant evidence.
* Generated an Autopsy report.

### Autopsy Evidence

Screenshots documenting the Autopsy investigation are stored in:

`/screenshots/autopsy/`

Supporting Autopsy outputs are stored in:

`/autopsy/`

---

## 8. Sleuth Kit Analysis

The forensic image was examined using The Sleuth Kit command-line utilities.

The analysis included:

```text
img_stat
mmls
fsstat
fls
istat
icat
blkcat
blkls
tsk_recover
```

Command outputs and supporting screenshots are stored in:

`/sleuthkit/`

---

## 9. Deleted File Analysis

Deleted files were identified using forensic file-system analysis techniques.

A recursive deleted-file listing was performed using `fls`.

The investigation documented:

* Deleted file names
* File metadata addresses
* File system information
* Relevant data units
* Recovery attempts
* Recovered evidence

Supporting evidence is stored in:

`/sleuthkit/`

---

## 10. INCOME.XLS Recovery

The investigation specifically examined the deleted file:

`INCOME.XLS`

The file was:

1. Located within the forensic image.
2. Identified using Sleuth Kit analysis.
3. Associated with its metadata address.
4. Examined using `istat`.
5. Recovered using `icat`.
6. Subjected to `blkcat` recovery where applicable.
7. Recovered using `tsk_recover`.
8. Compared using cryptographic hashes.
9. Examined locally to confirm successful recovery.

Recovered files are stored in:

`/recovered_files/`

---

## 11. Hash Verification

Cryptographic hashes were calculated for recovered copies of `INCOME.XLS`.

The recovered files were compared to determine whether the recovery methods produced identical evidence.

### Recovered File Hashes

| Recovery Method | MD5              | SHA-256          |
| --------------- | ---------------- | ---------------- |
| `icat`          | To be documented | To be documented |
| `blkcat`        | To be documented | To be documented |
| `tsk_recover`   | To be documented | To be documented |

Final hash results will be updated after completion of the practical.

---

## 12. Chain of Custody

A mini chain-of-custody/evidence worksheet was maintained throughout the examination.

The worksheet records:

* Evidence identification
* Evidence source
* Date/time of handling
* Examiner
* Evidence location
* Integrity verification
* Examination activities
* Evidence storage

Supporting documentation is stored in:

`/chain_of_custody/`

---

## 13. Screenshots and Supporting Evidence

Screenshots are provided to demonstrate the major stages of the investigation.

They include evidence of:

* Evidence image information
* Hash calculation
* Chain of custody
* Autopsy case creation
* Evidence source configuration
* Deleted-file analysis
* Keyword searches
* Tagged/recovered evidence
* Autopsy reporting
* Sleuth Kit commands
* `INCOME.XLS` identification
* Metadata analysis
* File recovery
* Hash comparison
* Local examination of the recovered spreadsheet

Screenshots are stored in:

`/screenshots/`

---

## 14. Repository Structure

```text
Lab1-Digital-Forensics-Autopsy-SleuthKit/
│
├── README.md
├── screenshots/
│   ├── autopsy/
│   └── sleuthkit/
├── evidence/
├── autopsy/
├── sleuthkit/
├── recovered_files/
├── hashes/
├── chain_of_custody/
└── report/
```

---

## 15. Forensic Handling Statement

The authorised training forensic image was treated as original evidence and was not intentionally modified during the investigation.

All forensic analysis, file recovery, screenshots, command outputs and reports were conducted and stored separately from the original evidence image.

Cryptographic hashing was used to support evidence integrity and to verify recovered files.

---

## 16. Final Findings

This section will be completed after the practical investigation.

The final findings will summarise:

* Deleted files identified
* Relevant evidence recovered
* Keyword-search results
* `INCOME.XLS` metadata and recovery results
* Hash comparison results
* Integrity verification
* Significant observations
* Any errors and corrective actions

---

## 17. Final Report

The completed professional forensic report will be provided in the `report/` directory.

The report will contain the investigation methodology, evidence details, forensic analysis, screenshots, findings, hash results, conclusions and supporting documentation.

---

**Note:** The original `Ch01InChap01.dd` forensic image is intentionally excluded from this repository to preserve the original evidence and comply with the laboratory submission requirements.

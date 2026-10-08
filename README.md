# ICD Coding Query — Offline Edition

**Home page: https://<your-account>.github.io/<repo-name>/** (replace after publishing)

A self-contained, fully offline retrieval tool for clinical coding. It integrates four coding
systems and tolerates *disordered*, *fragmentary* queries — the way coders actually remember
disease and procedure names.

* One HTML page plus a data folder. Double-click to run. **No install, no network, no server, no GPU.**
* Three exact tiers plus one fallback tier: exact substring → two-character fragments →
  order-free single characters → **partial-coverage fallback (v8.4)**.
* The fallback tier fires only when no exact hit exists; it returns at most the 10 closest
  candidates and marks them as fuzzy, for reference only. It never displaces an exact match.
* Cross-references the Chinese national clinical version 2.0 against the medical insurance
  version 2.0 and flags mismatches ("grey codes") automatically.
* No training, no annotation, no external model — all matching is deterministic string logic
  over local tables.

## Download

| File | Notes |
|---|---|
| [`ICD_Coding_Query_v8.4.zip`](ICD_Coding_Query_v8.4.zip) | Complete software, about 8 MB (unpacks to about 60 MB) |

Unzip anywhere (local disk or USB stick) and open `ICD编码查询-离线版/index.html` in
Chrome 60+ or Edge 79+, or double-click `启动工具.bat`. An English interface
(`index_en.html`) is included.

## Requirements

| | |
|---|---|
| Operating system | Windows 7 / 10 / 11 (32- or 64-bit) |
| Browser | Chrome 60+ or Edge 79+ (any Chromium-based browser). No plug-ins. |
| Memory / disk | 2 GB RAM; about 60 MB disk space (or a USB stick) |
| Network | None required — runs with the network adapter disabled |
| Privileges | No administrator rights needed |

## Data

282,015 coded entries across ICD-10 (national clinical version 2.0), ICD-9-CM-3, ICD-11 and
ICD-O / morphology. The classification codes and their titles are public classification
standards; this repository redistributes them only as processed electronic indexes.

## License

[CC BY-NC 4.0](LICENSE.txt) — free for personal, educational, research and non-commercial
clinical use, with attribution. Commercial use requires written permission from the
corresponding author. The software is provided "as is", without warranty of any kind.
Retrieval results are for reference only; the final coding decision must be made by a
qualified coder according to the coding rules in force.

## How to cite

> Duan J. *Development and evaluation of an offline disorder-tolerant fragment matching
> system for clinical coding retrieval.* Manuscript submitted to *BMC Medical Informatics
> and Decision Making* (Software article).

The DOI will be added here once the article is published.

## Contact

Jun Duan (段俊), Department of Medical Records and Statistics, Peking University Shenzhen
Hospital, Shenzhen, Guangdong, China — Duanjunywq@163.com

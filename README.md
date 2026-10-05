# Whole-Home Wi-Fi Expansion: Option Analysis

A printable decision report for one network: an ASUS RT-BE92U on stock Asuswrt, with AdGuard DNS over DoT, a USB SSD Samba share and a 6 GHz-only SSID carrying a Ryzen AI Max+ 395 mini-PC. Fifteen ways to extend coverage are scored against stated requirements, from a matched AiMesh node to third-party mesh kits, Ubiquiti UniFi and GL.iNet Flint routers.

Revision 1.6.0 — 2026-10-03.

**Verdict.** Buy a second RT-BE92U and add it as an AiMesh node on Ethernet backhaul: 10G where the primary's 10G port is free and the run is Cat6A, otherwise 2.5G. MoCA over coax where no Ethernet run exists, wireless MLO backhaul only where neither does.

## Files

| File | What It Is |
| --- | --- |
| `wifi-expansion-report-v1.6.pdf` | The report: 13 pages, US Letter, black-and-white safe |
| `README.md` | This file |
| `CHANGELOG.md` | Release history, newest first |
| `LICENSE` | MIT license covering the report and these documents |

**PDF checksum.** 799,817 B, SHA-256 `313fb571b1c13529807a3cd3767f9bce9860f6c00f790fff48d867f75331c7af`.

## What Is Inside

Thirteen sections and an appendix: the verdict, the baseline network, requirements R1 to R6, the AiMesh and non-AiMesh candidates, backhaul engineering against the host's 2,882 Mb/s ceiling, a decision matrix over fifteen options, the target topology, the deployment plan P0 to P8, the field checks V1 to V8, the risks U1 to U14, and a printable worksheet. Nine figures carry the path choice, port plan, ceilings, airtime, headroom, ranking, prices and topology.

## How to Verify

```fish
sha256sum wifi-expansion-report-v1.6.pdf
qpdf --check wifi-expansion-report-v1.6.pdf
pdfinfo wifi-expansion-report-v1.6.pdf | grep -E '^(Pages|Title|Subject):'
pdffonts wifi-expansion-report-v1.6.pdf
```

Expect a clean report, 13 pages and seven embedded DejaVu faces.

## Printing and Scope

US Letter, portrait. Every PASS, PART and FAIL cell repeats its label inside the shading, so the matrix survives a monochrome printer; page 13 is the worksheet, meant to be printed alone. Facts about the network are as stated by its owner and were not re-measured; vendor figures are as listed, and prices are snapshots taken between 2026-10-01 and 2026-10-03. Inferences are labeled where they appear.

## License and Versioning

MIT, in `LICENSE`. Release `X.Y.0` carries report edition `vX.Y`, as shown on the cover and in the PDF metadata; `CHANGELOG.md` follows the kernel.org style, newest block first, blocks never renumbered.

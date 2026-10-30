# Signal-Integrity Analyses

Short studies done alongside the board designs to build intuition for crosstalk, channel loss, and equalization.
Reports are written in Indonesian.

| Report | Tool | Summary |
|---|---|---|
| [01 – Crosstalk between PCB traces](01-Crosstalk-PCB-Analysis.pdf) | MATLAB (`traceLine`, `pcbComponent`) | EM current distribution and coupling between two adjacent traces over a ground plane at 1 GHz, swept over trace spacing |
| [02 – Crosstalk with Serial Link Designer](02-Crosstalk-Serial-Link-Designer.pdf) | MATLAB Serial Link Designer | Design-space sweep of trace length (0.75–1.5 in) and aggressor clearance (10/15/20 mil); ICR and ICN margins show 10 mil fails and 20 mil passes |
| [03 – Backplane with line cards](03-Backplane-Line-Card-Analysis.pdf) | MATLAB Serial Link Designer | 100 Ω differential stripline model (100.27 Ω from 2-D field solver), Touchstone connector import, end-to-end backplane channel analysis |
| [04 – LPF, CS amplifier & CTLE](04-SPICE-CTLE.pdf) | SPICE | RC low-pass filter, common-source MOSFET amplifier, and continuous-time linear equalizer frequency responses |

[`crosstalk-data.xlsx`](crosstalk-data.xlsx) contains the raw crosstalk sweep data.

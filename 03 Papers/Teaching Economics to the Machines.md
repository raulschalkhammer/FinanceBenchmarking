---
title: "Teaching Economics to the Machines"
created: 2026-07-06
tags: [paper, cluster-d, hoch]
---
# Teaching Economics to the Machines

## Metadata
Autoren: Hui Chen, Yuhan Cheng, Yanchu Liu, Ke Tang · Jahr: 2026 (Januar) · Institution: [[MIT Sloan]] / Shandong Univ. / Sun Yat-sen Univ. / Tsinghua (NBER WP 34713, nicht peer-reviewed) · Relevanz: Hoch · Link: https://www.nber.org/papers/w34713

## Research Question
Verbessert die Kombination aus ökonomischer Struktur (Theorie) und ML die Prognose/Bewertung – ohne die Schwächen beider Ansätze (schlechter Fit bei Strukturmodellen, Overfitting bei reinem ML)?

## Data
Optionsdaten (Anwendungsbeispiel); Struktur-„Quelldomäne" aus synthetischen, vom Strukturmodell erzeugten Daten.

## Methodology
**Theory-Guided Transfer Learning**: Ein neuronales Netz wird zuerst auf synthetischen Daten eines ökonomischen Strukturmodells vortrainiert (die Theorie als „Quelldomäne"), dann auf echten Empiriedaten fine-getunt. Die (evtl. fehlspezifizierten) Strukturrestriktionen werden nicht als harte Nebenbedingungen erzwungen, sondern **regularisieren** das Lernen – d. h. Theorie als weiche Leitplanke statt als Zwangskorsett.

## Main Findings
Der Hybrid **schlägt sowohl strukturelle als auch rein datengetriebene Benchmarks** – besonders stark in **kleinen Stichproben, unter instabilen Marktbedingungen und bei fehlspezifizierten Modellen** (genau die Situationen, in denen reines ML versagt). Liefert zusätzlich eine neue Modellvergleichs-Metrik auf Basis der „Daten-Modell-Komplementarität".

## Contributions
Paradigma „Theorie als Regularisierung" – gemeinsame Linie mit [[Deep Learning in Asset Pricing]]; direkt übertragbar auf DCF ([[Distress-Kosten im DCF – strukturell plus ML]]) und auf theoriegeleitete Kapitalkosten-Schätzung ([[ML Cost of Capital Literature Map]]). Der Transfer-Learning-Trick (auf Theorie-Synthetik vortrainieren, auf Realdaten fine-tunen) ist ein konkretes Rezept, das die WU auf Bewertungsprobleme mit dünnen Daten (z. B. private KMU) anwenden könnte.

## Limitations
Kein Peer-Review; Anwendung nur auf Optionspreise gezeigt (nicht auf Cashflow-/Bewertungsprognose); Erfolg hängt an der Qualität des zugrundeliegenden Strukturmodells.

## Related
Streams: [[Corporate Valuation]], [[Asset Pricing]] · Map: [[ML Cost of Capital Literature Map]] · [[AI Valuation Research Program]]

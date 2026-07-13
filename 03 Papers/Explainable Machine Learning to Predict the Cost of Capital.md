---
title: "Explainable Machine Learning to Predict the Cost of Capital"
created: 2026-07-06
tags: [paper, cost-of-capital, xai, esg, sehr-hoch]
---
# Explainable Machine Learning to Predict the Cost of Capital

## Metadata
Autoren: (auf gelesenen Seiten nicht namentlich genannt; wahrscheinlich Mariani/Pizzutilo et al. laut Selbstzitation) · Jahr: ~2022 · Typ: SSRN-Working-Paper · Relevanz: **Sehr hoch** (WU-Fokus WACC/Kapitalkosten × ML × Interpretierbarkeit) · Link: https://ssrn.com/abstract=4173890

## Research Question
Welche finanziellen **und nicht-finanziellen** Faktoren treiben die ex-ante (implizite) Kapitalkosten eines Unternehmens – und lässt sich das mit einem interpretierbaren ML-Modell zeigen?

## Data
Über 1.400 börsennotierte multinationale Unternehmen weltweit; Zielgröße: **implizite (ex-ante) Cost of Capital** = die vom Investor wahrgenommene Riskiness der Firma. Firmen-, Markt- und Länderfaktoren (inkl. World-Bank-Governance-Indikatoren und ESG-Variablen).

## Methodology
[[XGBoost]] ([[Gradient Boosting]]) zur Vorhersage der Kapitalkosten, geöffnet durch **zwei Explainable-AI-Werkzeuge**: SHAP-Werte (Shapley) und Lorenz-Zonoide ([[Interpretable Machine Learning]]). Feature-Ranking + Diebold-Mariano-Test zur Modellvereinfachung.

## Main Findings
Die vier wichtigsten Prädiktoren (ein sparsames 4-Variablen-Modell ist statistisch so gut wie das 11-Variablen-Modell, Diebold-Mariano p = 0,999): **Firmengröße (SIZE), Eigenkapitalrendite (ROE), Aktienkurs-Volatilität und die institutionelle Qualität des Landes (World-Bank „Voice")**. SIZE allein erklärt ~11 % der Prognosegüte, +ROE ~2 %, +Volatilität ~2 %, +Länderqualität ~1 %. **ESG zählt:** Hohe Emissionsintensität → **höhere** Kapitalkosten (der Markt „bestraft" Umweltsünder); gute Governance / gute institutionelle Qualität → **niedrigere** Kapitalkosten. Zusammenhänge sind **nichtlinear** – lineare Standardmodelle würden sie verfehlen.

## Contributions
Erste Arbeit, die **Explainable AI auf die Kapitalkosten-Schätzung** anwendet und damit die „Black Box" öffnet – zeigt, welche Treiber wie wirken, ohne vorab Linearität anzunehmen. Liefert empirische Evidenz, dass **nicht-finanzielle (ESG/Länder-)Faktoren** eigenständige Prädiktoren der Kapitalkosten sind.

## Limitations
Kein Peer-Review; nur große, gelistete Multis (Übertragbarkeit auf KMU/private Firmen offen); Querschnitt, keine Zeitdynamik/Regime; Autorennamen auf den gelesenen Seiten nicht eindeutig; ESG-Datenqualität als bekannte Schwachstelle.

## Research Opportunities
**Direkte Anschlussstelle an den WU-Auditing-/Explainability-Fokus:** interpretierbare Kapitalkosten-Modelle sind für Prüfung und Regulierung ideal. Erweiterung auf europäische/österreichische Firmen und auf **private KMU** (wo Kapitalkosten am schwersten zu schätzen sind). Verbindung mit [[Distress-adjustierter Diskontsatz]]: ESG-/Governance-Treiber neben ML-Ausfallwahrscheinlichkeit in einen firmenspezifischen Diskontsatz.

## Related Concepts
[[Implied Cost of Capital]] · [[Equity Risk Premium]] · [[Market Implied Discount Rate]]

## Related Papers
[[Earnings Forecast Accuracy and Implied Cost of Capital]] · [[The Implied Cost of Capital – A Machine Learning Approach]] · [[Interpretable Machine Learning for Earnings Forecasts]]

## Related Methods
[[XGBoost]] · [[Gradient Boosting]] · [[Interpretable Machine Learning]]

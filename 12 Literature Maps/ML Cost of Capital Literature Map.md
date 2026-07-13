---
title: "ML Cost of Capital Literature Map"
created: 2026-07-06
tags: [map, cost-of-capital, wacc, fokus]
---
# ML & AI für Cost of Capital / WACC — Fokus-Map

**Zweck dieser Gruppe:** Bündelt gezielt die Schnittmenge **Asset Pricing ∩ Machine Learning/AI ∩ Kapitalkosten (WACC / Cost of Equity / Cost of Debt / Diskontsatz)**. Der „Nenner" der Bewertung — wo ML/AI den Diskontsatz schätzt, statt nur Cashflows zu prognostizieren. Querschnitt über die Streams [[Cost of Capital]], [[Discount Rate Estimation]] und [[Asset Pricing]].

```mermaid
graph TD
  subgraph EK["Eigenkapitalkosten / ICC"]
    LW["Lee/Wang 2024<br>ICC ↑ (optimistisch)"]
    BARK["Barkfeldt 2022<br>ICC ernüchternd"]
    HT["Houston/Toronto 2023<br>ICC international"]
    LW --- BARK
    HT --> LW
  end
  subgraph XAI["Interpretierbare Kapitalkosten (WU-Winkel)"]
    ECC["Explainable ML for Cost of Capital<br>XGBoost + SHAP, ESG zählt"]
  end
  subgraph FK["Fremdkapitalkosten"]
    BOND["Bianchi et al. 2021<br>Bond Risk Premiums ML"]
  end
  subgraph MKT["Marktimplizite Sätze"]
    MIDR["CFA 2026 MIDR"]
    DAMO["Damodaran ERP 2026"]
    DAMO --> MIDR
  end
  subgraph THEORIE["AP-Theorie: SDF = Diskontfaktor"]
    DLAP["Chen/Pelger/Zhu 2023<br>Deep Learning in AP (SDF)"]
    AIPM["Kelly et al. 2025-26<br>AI Asset Pricing (Transformer-SDF)"]
    NNSDF["Wang et al. 2025<br>NewsNet-SDF (News→SDF)"]
    TEM["Chen et al. 2026<br>Teaching Economics (Theorie+ML)"]
    DLAP --> AIPM
    DLAP --> NNSDF
    DLAP -.Methode.-> TEM
  end
  EK --> WACC["WACC / firmenspezifischer Diskontsatz"]
  FK --> WACC
  XAI --> WACC
  MKT --> WACC
  THEORIE -.liefert Risikofaktoren.-> WACC
  WACC --> IDEE["WU-Ideen: Distress-adjustierter Diskontsatz,<br>ERP-Nowcasting, Textbasierte Risk Factors"]
```

## Lesart
- **Eigenkapitalseite (ICC):** Kernspannung [[Earnings Forecast Accuracy and Implied Cost of Capital]] (bessere Prognose → besserer Diskontsatz) vs. [[The Implied Cost of Capital – A Machine Learning Approach]] (Gegenbefund); international geprüft in [[ML Earnings Forecasting und ICC International]].
- **Interpretierbarkeit (WU-Heimvorteil):** [[Explainable Machine Learning to Predict the Cost of Capital]] öffnet die Black Box (XGBoost + SHAP) und zeigt, dass sogar ESG/Governance eigenständig auf die Kapitalkosten wirken — ideal für den Auditing-/Regulierungskontext.
- **Fremdkapitalseite:** [[Bond Risk Premiums with Machine Learning]] deckt die Debt-Seite des WACC.
- **Marktimplizite Zielgrößen:** [[What the Market Knows That WACC Doesn't (MIDR)]] und [[Equity Risk Premiums 2026 und Cost of Capital by Industry]] liefern beobachtbare Sätze zum Kalibrieren/Testen.
- **AP-Theorie (der Diskontfaktor selbst):** [[Deep Learning in Asset Pricing]] → [[Artificial Intelligence Asset Pricing Models]] / [[NewsNet-SDF]]; methodisch flankiert von [[Teaching Economics to the Machines]] (Theorie + ML).

## Offene Frage / Forschungsfenster
Der ungelöste Lee/Wang-vs-Barkfeldt-Widerspruch sitzt genau hier → [[Gaps – Valuation und Diskontsatz]].

## WU-Anknüpfung
Ideen: [[Distress-adjustierter Diskontsatz]] · [[ERP-Nowcasting mit ML]] · [[Textbasierte Latent Risk Factors für Kapitalkosten]] · [[LLM-basierte ICC-Schätzung]]

→ [[AI Valuation Research Program]]

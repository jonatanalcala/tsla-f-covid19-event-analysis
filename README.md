# **TSLA vs F During the COVID-19 Pandemic: Volatility, Risk-Adjusted Returns, and Event-Driven Behavior (2020–2022)**

## **1. Introduction**

This report analyzes the stock performance of **Tesla (TSLA)** and **Ford (F)** during the COVID-19 pandemic, focusing on:

1. **Volatility and risk-adjusted returns** (2020–2022)  
2. **Short-term market reactions** around major COVID-19 events  
3. **Event-study comparisons** of how TSLA and F responded to identical macro shocks  

A benchmark index (S&P 500) is included, and all analysis uses daily adjusted close prices.

---

## **2. Data & Methods Overview**

- **Data Source:** Yahoo Finance (`yfinance`)  
- **Period:** January 2020 – December 2022  
- **Assets:** TSLA, F, S&P 500  
- **Features Computed:**  
  - Daily returns  
  - 30-day rolling volatility  
  - Annualized Sharpe ratios  
  - Event-study windows (±10 trading days)

Three major COVID-related events were studied:

1. **WHO pandemic declaration** — March 11, 2020  
2. **CARES Act stimulus signed** — March 27, 2020  
3. **Pfizer/BioNTech vaccine effectiveness news** — November 9, 2020  

---

## **3. Descriptive Statistics (2020–2022)**

| Asset | Mean Daily Return | Std Dev Daily Return | Sharpe Ratio |
|-------|-------------------|-----------------------|--------------|
| TSLA  | 0.0030 | 0.0455 | **1.0236** |
| F     | 0.0008 | 0.0312 | **0.4074** |
| S&P 500 | 0.0003 | 0.0160 | 0.3115 |

### **Insights**

- Tesla produced **almost 4×** the mean daily return of Ford.  
- Tesla was **more volatile**, but still delivered a stronger risk-adjusted return.  
- Ford was more correlated with the S&P 500 (0.62) compared to TSLA (0.51).  
- TSLA’s lower correlation suggests more “growth stock” behavior, while Ford follows cyclical/market trends.

---

## **4. Visualization Analysis**

---

### **4.1 Normalized Price Performance (2020–2022)**  
![](figures/normalized_price_path_vs_sp500.png)

#### **Insights**

- Tesla massively outperformed both Ford and the S&P 500 during the pandemic.  
- TSLA increased more than **12×** from its starting price before declining in 2022.  
- Ford saw moderate appreciation (~2× at peak), consistent with a traditional automaker.  
- Both fell in 2022, but Tesla remained the stronger performer.

---

### **4.2 Rolling 30-Day Volatility (TSLA vs F)**  
![](figures/30_day_rolling_volatility_tsla_f.png)

#### **Insights**

- TSLA exhibited consistently higher volatility than Ford across the full period.  
- Large volatility spikes appeared around:
  - The March 2020 crash  
  - 2020–2021 EV/sentiment rallies  
- Ford’s volatility was lower and more stable, representing cyclical manufacturing behavior.  

---

### **4.3 Risk-Adjusted Performance (Sharpe Ratios)**  
![](figures/annualized_sharpe_ratios_tsla_f.png)

#### **Insights**

- Tesla had an annualized Sharpe ratio of **1.02**, more than double Ford’s **0.41**.  
- Despite Tesla’s higher volatility, returns were strong enough to justify the risk.  
- Ford offered lower returns without meaningfully lower volatility.

---

## **5. Event-Driven Market Shock Analysis**

To isolate major pandemic shocks and avoid noise from a 3-year window, event-study windows of **±10 trading days** were used.

---

## **5.1 WHO Pandemic Declaration — March 11, 2020**
![](figures/event_study_WHO_pandemic_annoucement.png)

### **Cumulative Returns (Event → +10 days)**
- **TSLA:** –14.98%  
- **F:** –8.64%

### **Volatility Change**
| Asset | Pre-Event Vol | Post-Event Vol |
|-------|----------------|----------------|
| TSLA | 0.0785 | **0.1158** |
| F    | 0.0529 | **0.0574** |

### **Interpretation**
- Both stocks dropped sharply immediately after the WHO announcement.  
- TSLA declined almost **twice as much** as Ford, showing higher sensitivity to systemic risk.  
- TSLA’s volatility exploded post-event, while Ford’s rose only modestly.

---

## **5.2 CARES Act Stimulus — March 27, 2020**
![](figures/event_study_CARES_act_signed.png)

### **Cumulative Returns (Event → +10 days)**
- **TSLA:** +26.56%  
- **F:** –0.5

### **Volatility Change**
| Asset | Pre-Event Vol | Post-Event Vol |
|-------|----------------|----------------|
| TSLA | 0.1112 | **0.0601** |
| F    | 0.1066 | **0.0471** |

### **Interpretation**
- TSLA soared following the stimulus bill, signaling rapid investor optimism.  
- Ford barely reacted in the short window.  
- Both experienced sharply lower volatility after the announcement, indicating market stabilization.  
- TSLA’s price response was exceptionally strong compared to Ford.

---

## **5.3 Pfizer Vaccine Announcement — November 9, 2020**
![](figures/event_study_pfizer_vaccine_news.png)

### **Cumulative Returns (Event → +10 days)**
- **TSLA:** +23.88%  
- **F:** +8.05%

### **Volatility Change**
| Asset | Pre-Event Vol | Post-Event Vol |
|-------|----------------|----------------|
| TSLA | 0.0428 | **0.0456** |
| F    | 0.0303 | **0.0233** |

### **Interpretation**
- Both stocks rallied due to economic reopening optimism, but TSLA’s rally was larger.  
- Ford saw falling volatility (increased stability).  
- TSLA volatility ticked up slightly, reflecting renewed speculative interest.

---

## **6. Answers to Research Questions**

---

## **RQ1: Volatility and Risk-Adjusted Return Analysis**

### **How did TSLA and F differ in volatility?**
- TSLA was consistently more volatile across all years.  
- Volatility spikes for TSLA were significantly higher during extreme market events.

### **Which stock had better risk-adjusted returns?**
**Tesla.**  
- Sharpe Ratio: **1.02**  
- Ford: **0.41**  
- TSLA delivered far better returns per unit of risk.

### **Conclusion (RQ1)**  
> **Tesla outperformed Ford on both absolute and risk-adjusted bases, despite much higher volatility.**

---

## **RQ2: Event-Driven Volatility Comparison (Market Shock Analysis)**

### **1. WHO Pandemic Announcement**
- Both stocks fell, but TSLA dropped more sharply.
- TSLA volatility jumped dramatically; Ford only modestly.

### **2. CARES Act Stimulus**
- TSLA surged +26%, Ford remained flat.
- Volatility decreased for both afterward as markets stabilized.

### **3. Pfizer Vaccine Announcement**
- Both rallied, but TSLA again outperformed.
- Ford volatility fell; TSLA volatility increased slightly.

### **Did TSLA and F react differently to major COVID events?**  
**Yes. Significantly.**

| Event | Tesla Reaction | Ford Reaction |
|-------|----------------|---------------|
| WHO Declaration | Large crash | Moderate drop |
| CARES Act | Huge rally | Flat |
| Pfizer Vaccine | Strong rally | Positive but smaller |

### **Conclusion (RQ2)**  
> **Tesla reacts more aggressively to macro shocks—both negatively and positively—while Ford’s responses are milder and more aligned with traditional cyclical patterns.**

---

## **7. Final Conclusions**

- Tesla showed **higher volatility**, **higher returns**, and **higher risk-adjusted performance**.  
- Tesla's extreme sensitivity to news reflects its growth-stock nature.  
- Ford behaved like a traditional cyclical automaker—less volatile, more correlated with the market.  
- COVID events magnified the difference between a speculative growth company and an established manufacturer.

Overall:

> **Tesla outperformed Ford in every major dimension—returns, risk-adjusted returns, post-event rebounds, and responsiveness to macroeconomic shocks.**

---

<div align="center">

# 📈 Yield Curve Modelling & Bond Analytics Suite

### Fixed Income Analytics • Interest Rate Risk • Yield Curve Engineering

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white">
  <img src="https://img.shields.io/badge/SciPy-Optimization-blue?style=for-the-badge">
  <img src="https://img.shields.io/badge/FRED-Market_Data-success?style=for-the-badge">
  <img src="https://img.shields.io/badge/Nelson--Siegel--Svensson-Yield_Curve-orange?style=for-the-badge">
</p>

<p align="center">
  <b>Yield Curves</b> • <b>Bond Pricing</b> • <b>Duration</b> • <b>Interest Rate Risk</b>
</p>

</div>

---

## Overview

Interest rates drive the valuation of almost every financial asset.

This project builds an institutional-grade fixed income analytics platform that models the entire yield curve, prices bonds, measures interest rate sensitivity, and stress-tests portfolios under changing market conditions.

The framework replicates workflows commonly used by fixed-income traders, bond portfolio managers, treasury teams, and central banks.

---

## Fixed Income Analytics Framework

<div align="center">

```text
          Market Yields
                │
                ▼

       Yield Curve Fitting

                │
                ▼

 Nelson-Siegel-Svensson

                │
                ▼

        Spot Curve

                │

      ┌─────────┼─────────┐

      ▼                   ▼

 Bond Pricing      Risk Analytics

      │                   │

      └─────────┬─────────┘

                ▼

      Portfolio Analysis
```

</div>

---

## Yield Curve Engine

<div align="center">

```text
      Treasury Yields

             │

             ▼

     Curve Calibration

             │

             ▼

      NSS Parameters

             │

             ▼

      Smooth Curve

             │

             ▼

 Yield Estimates
```

</div>

---

## Nelson-Siegel-Svensson Model

### Curve Components

<div align="center">

```text
 Yield Curve

      │

      ▼

 Level Factor

      │

      ▼

 Slope Factor

      │

      ▼

 Curvature Factor

      │

      ▼

 Long-Term Structure
```

</div>

The NSS framework captures the level, slope, and curvature dynamics of interest rate markets while producing smooth, arbitrage-consistent yield curves.

---

## Yield Curve Construction

<div align="center">

```text
 Market Data

      │

      ▼

 Treasury Rates

      │

      ▼

 NSS Calibration

      │

      ▼

 Spot Curve

      │

      ▼

 Forward Curve
```

</div>

---

## Bond Pricing Engine

<div align="center">

```text
 Cash Flows

      │

      ▼

 Discount Factors

      │

      ▼

 Present Value

      │

      ▼

 Bond Price
```

</div>

### Supported Instruments

| Instrument | Analytics |
|------------|------------|
| Treasury Bonds | Pricing & Risk |
| Corporate Bonds | Yield Analysis |
| Zero-Coupon Bonds | Discounting |
| Fixed Coupon Bonds | Duration Analysis |

---

## Interest Rate Risk Framework

<div align="center">

```text
 Interest Rates

         │

         ▼

 Yield Curve Shift

         │

         ▼

 Bond Repricing

         │

         ▼

 Portfolio Impact
```

</div>

---

## Duration Analytics

### Modified Duration

Measures first-order sensitivity to interest rate movements.

<div align="center">

```text
 Rate Change

      │

      ▼

 Price Change

      │

      ▼

 Duration
```

</div>

---

## Convexity Analysis

### Second-Order Risk

<div align="center">

```text
 Interest Rate Move

          │

          ▼

 Price Sensitivity

          │

          ▼

 Convexity Effect
```

</div>

Convexity improves the approximation of bond price changes for larger yield movements.

---

## DV01 Engine

### Dollar Value of a Basis Point

<div align="center">

```text
 +1 bp Move

      │

      ▼

 Price Impact

      │

      ▼

 DV01
```

</div>

Used extensively by trading desks to manage interest rate exposure.

---

## Key Rate Duration Analysis

<div align="center">

```text
 Yield Curve

      │

      ▼

 2Y   5Y   10Y   30Y

 │    │     │     │

 ▼    ▼     ▼     ▼

 KRD  KRD   KRD   KRD

      │

      ▼

 Risk Decomposition
```

</div>

Identifies sensitivity to movements at specific points along the yield curve.

---

## Yield Curve Stress Testing

### Parallel Shift

```text
      /
     /
    /
   /
  /
```

Entire curve moves uniformly.

---

### Twist Shift

```text
 \
  \
   \
   /
  /
 /
```

Short and long rates move differently.

---

### Butterfly Shift

```text
 \      /
  \    /
   \  /
    \/
```

Changes concentrated around the middle of the curve.

---

## Scenario Analysis Workflow

<div align="center">

```text
 Current Curve

       │

       ▼

 Stress Scenario

       │

       ▼

 Reprice Bonds

       │

       ▼

 Portfolio Impact

       │

       ▼

 Risk Report
```

</div>

---

## System Architecture

<div align="center">

```text
┌──────────────────────────┐
│ FRED Yield Data          │
└─────────────┬────────────┘
              │
              ▼

┌──────────────────────────┐
│ Yield Curve Engine       │
├──────────────────────────┤
│ NSS Calibration          │
│ Spot Curve Generation    │
│ Forward Curves           │
└─────────────┬────────────┘
              │
              ▼

┌──────────────────────────┐
│ Bond Analytics Layer     │
├──────────────────────────┤
│ Pricing                  │
│ Duration                 │
│ Convexity                │
│ DV01                     │
│ Key Rate Durations       │
└─────────────┬────────────┘
              │
              ▼

┌──────────────────────────┐
│ Scenario Analysis        │
└──────────────────────────┘
```

</div>

---

## Dashboard Components

| Module | Purpose |
|----------|---------|
| Yield Curve Dashboard | Curve Visualization |
| NSS Calibration | Model Fitting |
| Bond Pricing Engine | Valuation |
| Duration Analytics | Interest Rate Risk |
| DV01 Monitor | Risk Sensitivity |
| Key Rate Dashboard | Curve Exposure |
| Scenario Analysis | Stress Testing |

---

## Quantitative Foundation

<div align="center">

```text
      Fixed Income Markets

               │

               ▼

        Yield Curves

               │

               ▼

 Nelson-Siegel-Svensson

               │

               ▼

 Bond Valuation

               │

               ▼

 Interest Rate Risk
```

</div>

---

## Example Research Workflow

<div align="center">

```text
 FRED Data

     │

     ▼

 NSS Calibration

     │

     ▼

 Yield Curve

     │

     ▼

 Bond Pricing

     │

     ▼

 Risk Measures

     │

     ▼

 Stress Testing
```

</div>

---

## Technology Stack

```text
Python
│
├── NumPy
├── SciPy
├── Plotly
├── FRED API
└── Fixed Income Models
```

---

## Real-World Applications

### Fixed Income Desks

- Bond Valuation
- Risk Management
- Relative Value Trading

### Central Banks

- Yield Curve Monitoring
- Monetary Policy Analysis
- Economic Forecasting

### Treasury Departments

- Asset-Liability Management
- Interest Rate Exposure
- Capital Planning

### Bond Fund Managers

- Portfolio Construction
- Duration Management
- Scenario Analysis

---

## Skills Demonstrated

✅ Fixed Income Analytics

✅ Yield Curve Modelling

✅ Nelson-Siegel-Svensson

✅ Bond Pricing

✅ Duration Analysis

✅ Convexity Modelling

✅ DV01 & Key Rate Durations

✅ Interest Rate Risk

✅ Financial Engineering

✅ Quantitative Research

---

## Repository Structure

```text
yield-curve-modelling-bond-analytics-suite/
│
├── data/
│
├── yield_curve/
│   ├── nss_model.py
│   ├── calibration.py
│
├── bond_pricing/
│   ├── bond_engine.py
│
├── risk/
│   ├── duration.py
│   ├── convexity.py
│   ├── dv01.py
│   └── key_rate_duration.py
│
├── scenarios/
│
├── dashboards/
│
├── notebooks/
│
└── README.md
```

---

<div align="center">

### 📈 Model The Curve. Measure The Risk. Price The Market.

*"Every bond price begins with a yield curve."*

</div>

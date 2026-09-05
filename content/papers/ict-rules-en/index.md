---
title: "Rule-Based Evaluation of PO3-Inspired ICT Strategies: A Reproducible Analysis of Weekly Profile and Daily Swing Framework"
date: 2026-05-03
lastmod: 2026-06-12
tags: ["FX", "ICT", "PO3", "backtesting", "reproducibility", "negative-results"]
author: ["David Vossebürger"]
description: "Reproducible, rule-based evaluation of PO3-inspired ICT strategies on weekly profile and daily swing timeframes — six instruments, 18 years of M30 data."
summary: "Reproducible, rule-based evaluation of PO3-inspired ICT strategies using weekly-profile and daily-swing frameworks on six instruments across 18 years of M30 data. Negative-result study."
editPost:
    URL: "https://papers.ssrn.com/sol3/papers.cfm?abstract_id=6700099"
    Text: "SSRN 6700099"

---

<a class="repo-card" href="https://github.com/DavidVossebuerger/po3-ict-backtesting" target="_blank" rel="noopener">
  <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 16 16" width="20" height="20" fill="currentColor"><path d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0 0 16 8c0-4.42-3.58-8-8-8z"/></svg>
  <div class="repo-meta">
    <span class="repo-name">DavidVossebuerger/po3-ict-backtesting</span>
    <span class="repo-action">View source code on GitHub →</span>
  </div>
</a>

---

##### Abstract

This paper evaluates two rule-based ICT trading strategies — the Daily Swing Framework and a Composite signal aggregator — within a reproducible backtesting framework. The empirical basis is a multi-asset run across six instruments (EURUSD, GBPUSD, USDJPY, XAUUSD, USA500IDXUSD, USATECHIDXUSD) on M30 bid data from 2007 to 2025 (Dukascopy), with calibration, out-of-sample (OOS), and forward phases examined separately per instrument.

Neither strategy shows robust outperformance in its current parameterization. The daily-swing framework produced annualised Sharpe ratios between −3.89 and −0.35 across the six instruments, with maximum drawdowns of 100–227 %. Composite delivered Sharpe ratios of −1.24 to −0.53 with drawdowns of 47–81 %. A cost-attribution analysis reveals that under idealized (frictionless) execution the daily-swing framework achieves a Sharpe of +0.81 on EURUSD, but retail-level spread and slippage fully erase this edge.

Initial drafting was assisted by large language models; all quantitative analysis and interpretations were verified by the author.

---


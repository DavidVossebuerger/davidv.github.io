---
title: "Regime-Preserving Bootstrap for FX Fair-Value Models"
date: 2026-06-17
tags: ["FX", "bootstrap", "fair-value", "BEER", "FEER", "PPP", "regime-detection"]
author: ["David Vossebürger"]
description: "A bootstrap methodology that preserves exchange-rate regime structure when evaluating fair-value models of FX."
summary: "Two regime-aware bootstrap resamplers (Regime-Uniform and Regime-Markov) for FX fair-value strategies (BEER, FEER, PPP), validated against naive baselines on three currency pairs with B = 1999 replicates."
editPost:
    URL: "https://papers.ssrn.com/sol3/papers.cfm?abstract_id=6890880"
    Text: "SSRN 6890880"

---

<a class="repo-card" href="https://github.com/DavidVossebuerger/MC-Regime" target="_blank" rel="noopener">
  <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 16 16" width="20" height="20" fill="currentColor"><path d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0 0 16 8c0-4.42-3.58-8-8-8z"/></svg>
  <div class="repo-meta">
    <span class="repo-name">DavidVossebuerger/MC-Regime</span>
    <span class="repo-action">View source code on GitHub →</span>
  </div>
</a>

---

##### Abstract

This paper documents a regime-preserving bootstrap procedure for validating the out-of-sample robustness of FX fair-value strategies (BEER, FEER, PPP). The central idea is that standard bootstrap methods (IID, Moving Block, Stationary Block) destroy the economic regime structure of macro-FX data and thereby systematically bias Sharpe ratio inference.

We propose two regime-aware resamplers — Regime-Uniform (block resampling within macro-regimes) and Regime-Markov (block resampling with calibrated Markov transition matrix) — and validate them using five structure metrics, a Sharpe loss metric, an arrangement distance, a stationarity gate per Section 11.7, and Wilcoxon paired tests with Benjamini-Hochberg FDR.

Applied to a BEER pricer for three currency pairs (EURUSD, GBPUSD, USDJPY) with B = 1999 bootstrap replicates, the key finding is: **Regime-Markov reduces the bootstrap Sharpe loss by a factor of 1.3× compared to Regime-Uniform and by a factor of 4.6× compared to the naive IID benchmark.** The Markov transition structure provides the additional gain over pure block resampling.

The calibrated transition matrix passes the Section 11.7 stationarity gate (TV drift = 0.10), validating forward projections over short horizons of ∼3–5 Markov steps. The paper documents the complete metric definitions, the implementation, and the honest limits of cross-pair generalization.

---


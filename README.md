# A Synergistic Hybrid Architecture with Residual Attention and Mixture-of-Experts for Robust Hour-Ahead Forex Forecasting

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Conference: ICCKE 2025](https://img.shields.io/badge/Conference-ICCKE%202025-orange.svg)](https://iccke.um.ac.ir/)
[![Python 3.9+](https://img.shields.io/badge/Python-3.9+-teal.svg)](https://www.python.org/)

Official research codebase for the paper:
> **A Synergistic Hybrid Architecture with Residual Attention and Mixture-of-Experts for Robust Hour-Ahead Forex Forecasting**  
> *Author: Alireza Abbaszadeh*

This repository contains the implementation of a **synergistic hybrid deep learning architecture** that leverages **Residual Attention** and a **Mixture-of-Experts (MoE)** framework for robust hour-ahead forecasting of foreign exchange (Forex) rates.

---

## Table of Contents

- [Overview](#overview)
- [Key Features](#key-features)
- [Architecture](#architecture)
- [Installation](#installation)
- [Dataset Format](#dataset-format)
- [Contributing](#contributing)
- [License](#license)
- [Citation](#citation)

---

## Overview

Accurate and robust forecasting of Forex rates is vital for financial institutions and algorithmic trading systems. This project proposes a hybrid model combining residual attention mechanisms with a mixture-of-experts ensemble to improve hour-ahead exchange rate predictions. The architecture synergizes deep representation learning for multi-scale feature extraction and expert gating for robust predictive aggregation.

## Key Features

- **Residual Attention Mechanisms:** Enhance feature learning and dynamically focus on critical temporal patterns.
- **Mixture-of-Experts (MoE):** Specialized neural subnetworks coordinated by a gating network for diverse regime modeling.
- **Time-Series Sequence Modeling:** Tailored for high-frequency financial sequence data (Forex OHLCV).
- **Clean Python Pipeline:** Fully modularized and reproducible.

## Architecture

- **Input:** Historical Forex data (OHLCV sequences and technical indicators).
- **Feature Extraction:** Deep residual blocks with multi-head attention layers.
- **Expert Subnetworks:** Multiple specialized predictor networks.
- **Gating Mechanism:** Dynamically weights and combines experts based on the current regime.
- **Output:** Next-hour exchange rate return and level forecasts.

## Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/alirezaabbaszadeh/iccke25-forex-hybrid.git
   cd iccke25-forex-hybrid
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

## Dataset Format

The pipeline operates on standard time-series Forex data with OHLCV features:
```csv
Timestamp,Open,High,Low,Close,Volume
2024-01-01 00:00,1.1234,1.1250,1.1220,1.1240,1000
```

## Contributing

Contributions, feedback, and issue reports are welcome! Please open an issue or submit a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Citation

If you use this code or architecture in your research, please cite:

```bibtex
@inproceedings{abbaszadeh2025synergistic,
  title={A Synergistic Hybrid Architecture with Residual Attention and Mixture-of-Experts for Robust Hour-Ahead Forex Forecasting},
  author={Abbaszadeh, Alireza},
  booktitle={Proceedings of the 15th International Conference on Computer and Knowledge Engineering (ICCKE 2025)},
  year={2025}
}
```

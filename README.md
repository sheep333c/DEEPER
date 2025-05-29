# DEEPER: Directed Persona Refinement for Dynamic Persona Modeling

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen)
![Version](https://img.shields.io/badge/version-1.0-yellow)

**Official Implementation of the paper:  
"DEEPER: Insight into User-Directed Persona Refinement for Dynamic Persona Modeling"**  
By Aili Chen, Chengyu Du, Jiangjie Chen, et al.  
[[Paper]](https://arxiv.org/abs/2502.11078) | [[Project Page]](https://github.com/sheep333c/DEEPER.git)

---

## 🔍 Overview

DEEPER proposes a new *refinement-based paradigm* for **dynamic persona modeling**, addressing the limitations of traditional regeneration and extension methods.

Instead of blindly updating user personas, DEEPER leverages **prediction-behavior discrepancies** to guide update **directions**, enabling:
- ✨ Continual persona optimization  
- 🔄 Iterative refinement via RL  
- 🎯 Improved user behavior prediction across domains

---

## 🚀 Features

- A novel **three-goal objective**:  
  - ✅ Previous Preservation  
  - ✅ Current Reflection  
  - ✅ Future Advancement  

- Two-stage **iterative RL training** with DPO (Direct Preference Optimization)

- Evaluated on 4 datasets across **10 domains**, supporting both seen/unseen domain generalization

---

## 🛠 Installation

We recommend using Python 3.8 and Conda:

```bash
conda create -n deeper python=3.10
conda activate deeper
pip install -r requirements.txt
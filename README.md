# DEEPER: Directed Persona Refinement for Dynamic Persona Modeling

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen)
![Version](https://img.shields.io/badge/version-1.0-yellow)

## 🧠 Model & Data

- 🤖 **Model (DEEPER-llama-8B)**: [https://huggingface.co/deeper-team/DEEPER-llama-8B](https://huggingface.co/deeper-team/DEEPER-llama-8B)  
- 📂 **Dataset Hub**: [https://huggingface.co/deeper-team](https://huggingface.co/deeper-team)

---

**Official implementation of the paper**  
**"DEEPER: Insight into User-Directed Persona Refinement for Dynamic Persona Modeling"**  
by  
[**Aili Chen**](mailto:alchen20@fudan.edu.cn), [**Chengyu Du**](mailto:cydu24@m.fudan.edu.cn), [**Jiangjie Chen**](mailto:jiangjiec@bytedance.com),  
[**Jinghan Xu**](mailto:jhxu21@m.fudan.edu.cn), [**Yikai Zhang**](mailto:ykzhang22@m.fudan.edu.cn), [**Siyu Yuan**](mailto:syyuan21@m.fudan.edu.cn), et al.  
<br>
**Fudan University**

[[📄 Paper (arXiv)]](https://arxiv.org/abs/2502.11078) | [[💻 Project Page]](https://github.com/sheep333c/DEEPER.git)

---

## 🔍 Overview

**DEEPER** introduces a refinement-based paradigm for **dynamic persona modeling**, addressing the shortcomings of prior regeneration and extension approaches.

Instead of repeatedly replacing or appending to user personas, DEEPER uses **prediction-behavior discrepancies** to direct persona updates more effectively.

Key benefits:
- ✨ Continual persona optimization  
- 🔄 Iterative RL-based refinement  
- 🎯 Enhanced behavior prediction across diverse domains

---

## 🚀 Features

- ✅ **Three-Goal Optimization Framework**:
  - **Previous Preservation**
  - **Current Reflection**
  - **Future Advancement**

- 🔁 **Two-stage reinforcement learning** training strategy
- 📉 **Improves Mean Absolute Error (MAE)** across 10 domains
- 📦 Compatible with HuggingFace Transformers

---

## 🛠 Installation

We recommend using Python 3.10 and Conda:

```bash
conda create -n deeper python=3.10
conda activate deeper
git clone https://github.com/hiyouga/LLaMA-Factory.git
cd LLaMA-Factory
pip install -e ".[torch,metrics]" --no-build-isolation
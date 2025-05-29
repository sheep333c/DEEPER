# DEEPER: Directed Persona Refinement for Dynamic Persona Modeling

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen)
![Version](https://img.shields.io/badge/version-1.0-yellow)

By [<sup>1</sup>**Aili Chen**](https://scholar.google.com/citations?user=FAJzMAQAAAAJ&hl=zh-CN), [<sup>2</sup>**Chengyu Du**](https://scholar.google.com.hk/citations?user=tfwhN2gAAAAJ&hl=zh-CN), [<sup>3</sup>**Jiangjie Chen**](https://jiangjiechen.github.io/),  [<sup>4</sup>**Jinghan Xu**](mailto:jhxu21@m.fudan.edu.cn), [<sup>5</sup>**Yikai Zhang**](https://ykzhang721.github.io/), [<sup>6</sup>**Siyu Yuan**](https://siyuyuan.github.io/), et al.  

<sup>1</sup>Fudan University

[[📄 Paper]](https://arxiv.org/abs/2502.11078) | [[💻 Project Page]](https://github.com/sheep333c/DEEPER.git) | [[🤖 Model: DEEPER-llama-8B]](https://huggingface.co/deeper-team/DEEPER-llama-8B) | [[📂 Dataset Hub]](https://huggingface.co/deeper-team)


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

We recommend using Python 3.10 and Conda.  
You’ll also need to install [LLaMA-Factory](https://github.com/hiyouga/LLaMA-Factory):

```bash
conda create -n deeper python=3.10
conda activate deeper
git clone https://github.com/hiyouga/LLaMA-Factory.git
cd LLaMA-Factory
pip install -e ".[torch,metrics]" --no-build-isolation
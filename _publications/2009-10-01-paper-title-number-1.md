---
title: "Diffusion Blend: Inference-Time Multi-Preference Alignment for Diffusion Models"
collection: publications
category: manuscripts
permalink: /publication/2025-05-24-diffusion-blend
excerpt: "This paper proposes a method for inference-time alignment of diffusion models to multiple, possibly conflicting, user-specified preferences (rewards) without additional fine-tuning."
date: 2025-05-24
venue: "arXiv (pre-print)"
paperurl: "https://arxiv.org/abs/2505.18547"
citation: "Min Cheng, Fatemeh Doudi, Dileep Kalathil, Mohammad Ghavamzadeh, Panganamala R. Kumar. (2025). \"Diffusion Blend: Inference-Time Multi-Preference Alignment for Diffusion Models.\" arXiv:2505.18547."
---

Diffusion Blend introduces an inference-time approach for **multi-preference alignment** in diffusion models, enabling users to balance multiple reward functions (e.g., text-image consistency, aesthetics) without retraining. Unlike traditional reinforcement learning–based fine-tuning, which aligns a model to a single objective, Diffusion Blend blends backward diffusion processes from multiple fine-tuned models to accommodate new user-defined combinations of preferences dynamically.

The authors propose two key methods:

- **DB-MPA (Multi-Preference Alignment):** Combines fine-tuned models for distinct rewards to synthesize arbitrary linear reward combinations during inference.  
- **DB-KLA (KL-Regularization Alignment):** Enables inference-time control over KL regularization strength, managing the trade-off between fidelity to the base model and adherence to specific rewards.

Experiments on Stable Diffusion demonstrate that Diffusion Blend surpasses baseline methods in reward trade-offs and generates outputs matching or exceeding individually fine-tuned models, validating both its theoretical underpinnings and practical flexibility.

**Key contributions:**
- A theoretical formulation linking diffusion model alignment with control-based blending of backward SDEs.  
- Inference-time flexibility for both multi-objective alignment and regularization control.  
- Empirical results showing superior reward trade-offs and sample quality without additional fine-tuning.

**Limitations and future directions:**
- Requires initial fine-tuning for each base reward.  
- Linear blending may degrade with extreme reward combinations.  
- Potential exploration: nonlinear preference composition, more efficient fine-tuning, and scaling to larger models.

---

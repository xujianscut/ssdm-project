# Stochastic Schrodinger Diffusion Models

Project page for the preprint:

**Stochastic Schrodinger Diffusion Models for Pure-State Ensemble Generation**

Jian Xu, Wei Chen, Chao Li, Jingyuan Zheng, Delu Zeng, John Paisley, Qibin Zhao

## Overview

Stochastic Schrodinger Diffusion Models (SSDMs) study score-based generative modeling directly on the quantum pure-state manifold. The model treats pure states as points on complex projective space and defines both the forward noising process and the reverse-time sampler intrinsically with respect to Fubini-Study geometry.

The project page includes the preprint PDF, a method illustration, the main training-stability figure, Algorithm 1, and the complete main quantitative table.

## Links

- Project page: https://xujianscut.github.io/ssdm-project/
- Direct PDF: https://xujianscut.github.io/ssdm-project/assets/ssdm_preprint.pdf

## Method Summary

SSDM combines three ingredients:

- An intrinsic diffusion process on the complex projective manifold of normalized quantum states modulo global phase.
- A reverse-time generative process driven by a learned Riemannian score.
- A local-time analytic teacher score in Fubini-Study normal coordinates for stable score matching.

The core reverse-time model learns

```text
s_theta(psi, t) ~= grad_FS log p_t(psi),
```

and samples by integrating the corresponding reverse stochastic dynamics on the pure-state manifold.

## Citation

```bibtex
@misc{xu2026ssdm,
  title={Stochastic Schr{\"o}dinger Diffusion Models for Pure-State Ensemble Generation},
  author={Xu, Jian and Chen, Wei and Li, Chao and Zheng, Jingyuan and Zeng, Delu and Paisley, John and Zhao, Qibin},
  year={2026},
  note={Preprint manuscript. Project page: \url{https://xujianscut.github.io/ssdm-project/}. PDF: \url{https://xujianscut.github.io/ssdm-project/assets/ssdm_preprint.pdf}}
}
```

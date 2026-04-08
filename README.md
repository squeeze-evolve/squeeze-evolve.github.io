# Squeeze Evolve — Documentation Website

Documentation site for **Squeeze Evolve**, a verifier-free evolutionary test-time scaling framework with multi-model orchestration.

## About the Paper

Test-time scaling lets language models produce many candidate answers and iteratively refine them through selection and recombination. When paired with an external verifier this evolutionary approach has produced breakthroughs in code generation and scientific discovery — but in many domains (plasma simulation, wet-lab experiments) verification is too expensive, too slow, or simply unavailable.

**Squeeze Evolve** addresses *verifier-free evolution*: achieving a given capability target under tight budget constraints without ground-truth feedback. The key contributions are:

- **Unified evolutionary framework.** Majority voting, self-refinement, RSA, and AlphaEvolve are all shown to be instances of a single evolutionary operator — differing only in their choice of selection, recombination, and fitness signal.
- **Confidence-based multi-model routing.** Model-intrinsic confidence (e.g., token log-probabilities) is used to route hard groups to expensive models and easy groups to cheaper ones, solving both *diversity collapse* and *cost explosion*.
- **Strong empirical results across 8 benchmarks.** 1.4–3.3× cost savings and 4–10× throughput gains on math (AIME 2025, HMMT 2025, GPQA-Diamond), coding (LiveCodeBench V6), vision (MMMU-Pro, BabyVision), visual reasoning (ARC-AGI-V2 — 97.5% at $5.93/task), and scientific discovery (circle packing).

### Citation

```bibtex
@article{maheswaran2026squeezeevolve,
  title={Squeeze Evolve: Unified Multi-Model Orchestration Framework for Verifier-Free Evolution},
  author={Maheswaran, Monishwaran and Lakhani, Leon and Zhou, Zhongzhu and Yang, Shijia and Wang, Junxiong and Hooper, Coleman and Hu, Yuezhou and Tiwari, Rishabh and Wang, Jue and Singh, Harman and Wu, Qingyang and Jian, Yuqing and Zhang, Ce and Keutzer, Kurt and Dao, Tri and Wu, Xiaoxia and Athiwaratkun, Ben and Zou, James and Xu, Chenfeng},
  year={2026}
}
```
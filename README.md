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
@misc{maheswaran2026squeezeevolveunifiedmultimodel,
      title={Squeeze Evolve: Unified Multi-Model Orchestration for Verifier-Free Evolution}, 
      author={Monishwaran Maheswaran and Leon Lakhani and Zhongzhu Zhou and Shijia Yang and Junxiong Wang and Coleman Hooper and Yuezhou Hu and Rishabh Tiwari and Jue Wang and Harman Singh and Qingyang Wu and Yuqing Jian and Ce Zhang and Kurt Keutzer and Tri Dao and Xiaoxia Wu and Ben Athiwaratkun and James Zou and Chenfeng Xu},
      year={2026},
      eprint={2604.07725},
      archivePrefix={arXiv},
      primaryClass={cs.AI},
      url={https://arxiv.org/abs/2604.07725}, 
}
```
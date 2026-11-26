# VISTA-RL Roadmap

**Status:** Planned project (not yet implemented).

## Milestones

1. **Environment & Baseline Harness**
   - Pin Python, PyTorch, and Gymnasium/Atari or DMControl dependencies in `requirements.txt`.
   - Implement a deterministic seeding and logging wrapper (episode return, evaluation seed tracking).
2. **Visual Encoder & PPO Baseline**
   - Build a lightweight convolutional encoder + PPO agent.
   - Establish reproducible baseline learning curves across at least 3 random seeds on a starter visual benchmark.
3. **Representation & Ablation Study**
   - Compare frame-stacking vs. recurrent/temporal encoders and measure sample efficiency on held-out seeds.
4. **Evaluation & Reproducibility Suite**
   - Add automated unit tests for observation preprocessing, rollout buffer shapes, and checkpoint loading.
   - Save evaluation tables and training curves under `results/`.
5. **Documentation & Release**
   - Document exact hardware, hyperparameters, verified metrics, and failure modes in `README.md`.

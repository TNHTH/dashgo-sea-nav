# Provenance

Date: 2026-10-12

- Upstream repository: https://github.com/11chens/SEA-Nav-Code
- Upstream commit: `fbce672c22d432e0ba8c9ef1b1e822f8fbd3ec96`
- Canonical branch: `main`, fast-forwarded to the former `test` tip `ae073ad596a3b2d2c10172dee36134a0795fab5b`
- Local remote to keep: `git remote add upstream https://github.com/11chens/SEA-Nav-Code.git`

Every path in that upstream commit is still present. Fifteen upstream paths differ, including `training/rsl_rl/rsl_rl/algorithms/ppo.py`, the CBF modules, and `training/legged_gym/legged_gym/envs/base/legged_robot.py`. The DashGo adaptation adds `training/sea_nav_diffdrive_isaaclab/`, `packages/sea_nav_core/`, and `tools/sea_*_dashgo.py`.

Fidelity: F2. Observation, the 2D DashGo actor, the unicycle CBF, and the reward path are modified, as already recorded in `docs/dashgo-sea/adaptation-ledger.md`. This is not a byte-identical paper baseline. Hardware and Isaac execution were not rerun for this governance commit, so verification stays V0.

`stable` matched the pre-move `main` and had no unique commits. `issue/1-sea-dashgo-milestone-a` is an ancestor of `ae073ad596a3` and has the same tree.

# smolvm documentation

The flat pages here (`branching.md`, `smolfile.md`, `security-model.md` and the rest) are the
reference for each feature. A skill packet is a tested procedure for one task and links the
reference page it builds on. Each folder below is one: a `README.md` with the facts and why they
hold, and a `SKILL.md` an agent can follow, with its own `scripts/` and `references/`.
Each packet's `SKILL.md` opens with the release and platforms it last ran on. No CI runs the packet
scripts; call them by path from a working directory of your own, since they write to the current
directory.

`llms.txt` lists every packet's `SKILL.md` for agents that read the tree directly.

## Skill packets

| Packet | What it covers | Procedure |
|---|---|---|
| [branch-and-checkpoint](branch-and-checkpoint/README.md) | scheduled checkpoints with history, restores, pause and resume, and branches with their branch point kept | [SKILL.md](branch-and-checkpoint/SKILL.md) |
| [dev-env](dev-env/README.md) | a machine you come back to, and what survives a stop and start | [SKILL.md](dev-env/SKILL.md) |
| [docker-in-machine](docker-in-machine/README.md) | a Docker daemon inside a machine, for tools that call Docker themselves | [SKILL.md](docker-in-machine/SKILL.md) |
| [gpu-cuda](gpu-cuda/README.md) | CUDA Driver API calls remoted to the host NVIDIA GPU | [SKILL.md](gpu-cuda/SKILL.md) |
| [install](install/README.md) | installing smolvm and proving the host can boot a microVM | [SKILL.md](install/SKILL.md) |
| [local-api](local-api/README.md) | driving the machine lifecycle over the local HTTP API | [SKILL.md](local-api/SKILL.md) |
| [pack](pack/README.md) | packing an image or a machine into a portable artifact | [SKILL.md](pack/SKILL.md) |
| [teardown](teardown/README.md) | what state exists, where it lives, and how to leave nothing running | [SKILL.md](teardown/SKILL.md) |
| [throwaway-machine](throwaway-machine/README.md) | running untrusted code in a throwaway machine, with egress granted one host at a time | [SKILL.md](throwaway-machine/SKILL.md) |

---
sidebar_position: 3
description: An overview of the dice manager
tags:
  - Board
  - Character
  - Movement
  - Turn
---

# Dice Manager

```mermaid
  stateDiagram-v2
    [*] --> SpawnDice
    SpawnDice --> Rolling: Next
    Rolling --> RollResult: RollingDone
    RollResult --> RollResult: Next
    RollResult --> [*]: Reset
```
---
title: Transformer from Scratch
layout: page
description: Implementation of a transformer architecture in PyTorch
image: /assets/img/transformer.png
github: https://github.com/Manya009/transformer
---

## Overview

This project implements a **Transformer architecture from scratch** using PyTorch.

Goal: understand attention mechanisms and training dynamics.

---

## Architecture

![Transformer architecture](/assets/img/transformer.png)

Key components:

- Multi-head attention
- Positional encoding
- Feedforward layers
- Layer normalization

---

## Results

| Metric | Value |
|------|------|
Training Loss | 1.32 |
Validation Loss | 1.41 |

---

## Learnings

- Attention layers dominate compute
- Training stability depends heavily on initialization

---

## Links

GitHub: [View Code]({{ page.github }})
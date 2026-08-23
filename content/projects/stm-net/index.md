---
title: "STM-Net: Reconstructing Molecular Orbitals from STM Images"
date: 2024-01-01
summary: >-
  Physics-driven STM image restoration with PSNR above 37 dB using 10% of the
  training data and above 43 dB on the full dataset.
tags:
  - Scanning tunneling microscopy
  - DFT
  - U-Net
  - Computer vision
  - AI for Science
links:
  - type: code
    url: https://github.com/ZeHeru/STM_net/tree/main
  - type: custom
    label: JACS Au paper
    url: https://doi.org/10.1021/jacsau.5c00310
featured: true
aliases:
  - /portfolio/stm-net/
---

In a nutshell: **Are orbitals observable?**

This project reconstructs pristine molecular-orbital information from
high-resolution scanning tunneling microscopy images. STM images are simulated
at the density-functional-theory level using Bardeen's approximation, and
STM-Net separates s-wave molecular-orbital signals from p-wave contributions
introduced by CO-functionalized tips.

<!--more-->

The approach connects Tersoff-Hamann theory and Chen's derivative rule with
physics-informed image restoration. Experiments included DAE, U-Net, and
Mask2Former-based models.

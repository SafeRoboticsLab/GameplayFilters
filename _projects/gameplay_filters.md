---
layout: project
permalink: /
title: "Gameplay Filters: Safe Robot Walking through Adversarial Imagination"
authors:
    - Duy Phuong Nguyen
    - Kai-Chieh Hsu
    - Jaime Fernandez Fisac
figure: src/test-front-figures.png
video: 
abstract: "This paper presents gameplay filter, a general approach that leverages offline game-theoretic reinforcement learning to synthesize a highly robust safety filter for high-order nonlinear dynamics that maintains runtime safety by continually simulating adversarial futures and precluding task-driven actions that would cause it to lose future games (and thereby violate safety)."
---

# Offline gameplay learning
We employ a game-theoretic reach–avoid reinforcement learning scheme that iteratively pits the robot’s controller against a simulated adversarial environment. The algorithm updates a safety value network (critic) and keeps a leaderboard of the most effective player policies (actors). The video below shows the co-training process:

<center>
    <iframe src="https://drive.google.com/file/d/1JmuKZqwurjL5H6yPznkAIQcJmQMAMC50/preview" style="width: 40vw; max-width: 960px; height: 22.5vw; max-height: 540px;" allow="autoplay"></iframe>
</center>

<br><br>

# Online gameplay safety filter
![gameplay filter operation](src/gameplay-filter-operation.png)

<br><br>

# Experiments
![table 1](src/table-1-result.png)
Gameplay rollout - bumpy terrain experiment
<center>
    <iframe src="https://drive.google.com/file/d/1nZOw_vl-cDAMg493mTEDMP46lUL9NEN4/preview" style="width: 60vw; max-width: 960px; height: 33.75vw; max-height: 540px;" allow="autoplay"></iframe>
</center>

Gameplay rollout - tugging experiment
<center>
    <iframe src="https://drive.google.com/file/d/1QudR9QxSfyiUrffoESTVea6O9B0vgpf7/preview" style="width: 60vw; max-width: 960px; height: 33.75vw; max-height: 540px;" allow="autoplay"></iframe>
</center>

Value shielding and task policy
<center>
    <iframe src="https://drive.google.com/file/d/16u33ukdTPIq3G_h9c8DYXb808u9zwrHW/preview" style="width: 60vw; max-width: 960px; height: 33.75vw; max-height: 540px;" allow="autoplay"></iframe>
</center>

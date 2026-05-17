# quadrotor-mamba

This repository contains the materials and supplements of "**Vision-Driven State-Space Imitation Learning for Quadrotor
Navigation in Infrastructure Inspection**".

**ABSTRACT**: With the rapid development of intelligent civil infrastructure and smart cities, quadrotors are increasingly deployed for inspection, monitoring, and emergency response in infrastructure environments, such as power transmission corridors, transportation greenbelts, and urban green infrastructure. Reliable quadrotor navigation in such environments requires robust perception-driven decision making to safely avoid obstacles while maintaining operational efficiency. However, existing quadrotor navigation approaches often rely on handcrafted heuristics, task-specific planning, or reinforcement learning methods with high training cost and limited stability, which restrict their applicability in safety-critical infrastructure scenarios. To address these challenges, this paper proposes a vision-driven imitation learning framework with state-space models for quadrotor navigation in infrastructure inspection environments. The approach leverages a privileged expert to generate large-scale demonstration data in simulation, from which a vision-based navigation policy is trained via imitation learning. Depth-based visual observations and proprioceptive states are encoded into compact representations and processed by a selective state-space model to capture long-horizon temporal dependencies and motion continuity. The learned policy outputs high-level navigation commands, which are executed through a geometric control module, facilitating stable and physically consistent deployment. Extensive simulation experiments in representative infrastructure navigation scenarios demonstrate that the proposed method reduces collision occurrences and energy consumption, while producing smoother and more temporally consistent trajectories than state-of-the-art baselines, even at high flight speeds. The results indicate that the proposed framework provides a robust, computer-aided solution for safe quadrotor navigation in civil infrastructure inspection environments.

This work has been accepted by [Computer-Aided Civil and Infrastructure Engineering](https://www.sciencedirect.com/journal/computer-aided-civil-and-infrastructure-engineering), to cite this work:

```bib
@article{TAO2026100030,
title = {Vision-driven state-space imitation learning for quadrotor navigation in infrastructure inspection},
journal = {Computer-Aided Civil and Infrastructure Engineering},
pages = {100030},
year = {2026},
issn = {1093-9687},
doi = {https://doi.org/10.1016/j.cacaie.2026.100030},
url = {https://www.sciencedirect.com/science/article/pii/S1093968726030045},
author = {Xiaowen Tao and Yinuo Wang and Bing Zhu and Jiayi Han and Peixing Zhang and Pengxiang Meng and Jinzhao Zhou and Chin-Teng Lin},
}
```

# Architecture
<img src="https://github.com/user-attachments/assets/439e244b-4519-42fb-83e2-9c2de73815e1"
     width="600"
     style="border: 3px solid #333; border-radius: 8px;"
/>

# Experiments Results of Our Model

| Desired vel | Unseen Tree Secenario| Sphere Scenario          |
|------|-----------------------------|--------------------------|
| 3m/s |![tree3](media/tree3.gif)|![sphere3](media/sphere3.gif)|
| 5m/s |![tree3](media/tree5.gif)|![sphere5](media/sphere5.gif)|
| 7m/s |![tree3](media/tree7.gif)|![sphere7](media/sphere7.gif)|

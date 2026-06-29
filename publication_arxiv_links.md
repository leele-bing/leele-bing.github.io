# arXiv Links for Publications

This file records arXiv versions found for the publications currently listed in `_bibliography/papers.bib`.

## Confirmed arXiv Links Added to Publications

| BibTeX key             | Title                                                                                                       | arXiv ID     | URL                              | Notes                                                                                          |
| ---------------------- | ----------------------------------------------------------------------------------------------------------- | ------------ | -------------------------------- | ---------------------------------------------------------------------------------------------- |
| `ma2025robust`         | Robust Second-Order LiDAR Bundle Adjustment Algorithm Using Mean Squared Group Metric                       | `2409.01856` | https://arxiv.org/abs/2409.01856 | Matched by title. The arXiv author list may differ from the published/current BibTeX metadata. |
| `sun2025namr`          | NAMR-RRT: Neural Adaptive Motion Planning for Mobile Robots in Dynamic Environments                         | `2411.00440` | https://arxiv.org/abs/2411.00440 | Confirmed title and author list include Bingyi Xia.                                            |
| `xie2025autonomous`    | Autonomous Multiple-Trolley Collection System with Nonholonomic Robots: Design, Control, and Implementation | `2401.08433` | https://arxiv.org/abs/2401.08433 | Confirmed title and author list include Bingyi Xia.                                            |
| `xi2024disturbance`    | Disturbance Rejection Control for Autonomous Trolley Collection Robots with Prescribed Performance          | `2309.12660` | https://arxiv.org/abs/2309.12660 | Matched by title. The arXiv author list may differ from the published/current BibTeX metadata. |
| `xia2023collaborative` | Collaborative Trolley Transportation System with Autonomous Nonholonomic Robots                             | `2303.06624` | https://arxiv.org/abs/2303.06624 | Confirmed title and author list include Bingyi Xia.                                            |

## No arXiv Version Found in This Pass

| BibTeX key             | Title                                                                                                                                        |
| ---------------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| `xia2024smart`         | Smart Mobility With Agent-Based Foundation Models: Towards Interactive and Collaborative Intelligent Vehicles                                |
| `gao2023divide`        | A Divide-and-Conquer Control Strategy with Decentralized Control Barrier Function for Luggage Trolley Transportation by Collaborative Robots |
| `tang2022relationship` | Relationship Oriented Semantic Scene Understanding for Daily Manipulation Tasks                                                              |
| `xia2021motion`        | Motion Planning for Hexapod Robots in Dynamic Rough Terrain Environments                                                                     |
| `liu2021etextile`      | E-Textile Batteryless Displacement and Strain Sensor for Human Activities Tracking                                                           |
| `liu2020embroidered`   | Embroidered Inductive Strain Sensor for Wearable Applications                                                                                |
| `liu2020fabrics`       | Fabrics-Based Embroidered Passive Displacement Sensors for On-Body Applications                                                              |

## Implementation Note

`al-folio` renders an arXiv button from the BibTeX field:

```bibtex
arxiv = {2303.06624}
```

The earlier `eprint` / `eprinttype` fields are not used by the current publication template for button rendering, so confirmed arXiv links were converted to `arxiv`.

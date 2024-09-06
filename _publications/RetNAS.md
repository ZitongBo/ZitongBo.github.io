---
title: "Designing Real-Time Neural Networks by Efficient Neural Architecture Search"
collection: publications
category: conferences
permalink: /publication/RetNAS
excerpt: 'Authors: **Zitong Bo**, Yilin Li, Ying Qiao, Chang Leng and Hongan Wang'
date: 2024-08-08
venue: '2024 International Conference on Intelligent Computing (ICIC)'
paperurl: 'http://zitongbo.github.io/files/RetNAS.pdf'
citation: 'BO, Zitong, et al. Designing Real-Time Neural Networks by Efficient Neural Architecture Search. In: International Conference on Intelligent Computing. Singapore: Springer Nature Singapore, 2024. p. 62-73.'
---

Convolutional Neural Networks (CNNs) are extensively used in cyber-physical systems for tasks like object detection and semantic segmentation. Given the critical nature of these systems, the ability of CNNs to meet stringent timing constraints is as crucial as their accuracy. However, variability in CNN execution times can lead to time constraint violations, affecting system reliability. To address this, we introduce RetNAS, an efficient neural architecture search framework that combines a rapid Worst-Case Execution Time (WCET) estimator and a constraint schedule to ensure timely performance. We utilize extreme value theory to estimate WCET, leveraging a generalized Pareto distribution based on limited execution time samples. Furthermore, RetNAS employs a constraint schedule to accelerate the search efficiency, which pursues a gradual search trajectory. RetNAS significantly enhances search efficiency and achieves a success rate of approximately 99.2% in meeting time constraints, outperforming other methods. Our experiments also show that CNNs designed by RetNAS surpass the accuracy of manually designed CNNs and visual transformers by 0.4% to 5%.

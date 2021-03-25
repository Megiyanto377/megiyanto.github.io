---
title: "Re-identification network"
excerpt: "Re-identification of wild animals based on natural markings.<br/><img src='/images/portfolio/reid/portfolio-reid-manta.jpg'>"
collection: portfolio
---

# Overview

This is the implementation for re-identification system described in the paper ["Robust Re-identification of Manta Rays from Natural Markings by Learning Pose Invariant Embeddings"](https://arxiv.org/pdf/1902.10847.pdf) by Olga Moskvyak, Frederic Maire, Asia Armstrong, Feras Dayoub and Mahsa Baktashmotlagh.

The convolutional neural network (CNN) is trained to learn embeddings for images of natural markings, where the learned distance between embedding points corresponds to similarity between patterns. The network is optimized using the triplet loss function and the online semi-hard triplet mining strategy. The proposed re-identification method is generic and not species specific. We evaluate the proposed system on image databases of manta ray belly patterns, humpback whale flukes and whale sharks.


# Deliverables

* Source code in Keras/Tensorflow [reid-manta](https://github.com/olgamoskvyak/reid-manta)
* Updated source code in PyTorch and integration with WildMe/WildBook in [wbia-plugin-reid](https://github.com/olgamoskvyak/wbia-plugin-pie-v2)
* [Paper](https://arxiv.org/pdf/1902.10847.pdf)


# Qualitative results

First image in each row is a query image. The next five images are the top-5 retrieved mathces from the test set.

<span style="color:green">A green border</span> - correct match, <span style="color:red">a red border</span> border - incorrect match.

Whale Sharks:

![Example of whale sharks](/images/portfolio/reid/portfolio-reid-whale-shark-example-1.jpg)
![Example of whale sharks](/images/portfolio/reid/portfolio-reid-whale-shark-example-2.jpg)
![Example of whale sharks](/images/portfolio/reid/portfolio-reid-whale-shark-example-3.jpg)
![Example of whale sharks](/images/portfolio/reid/portfolio-reid-whale-shark-example-4.jpg)
Image credit: [WildMe/WildBook](https://www.wildme.org)

Manta rays:

![Example of manta rays](/images/portfolio/reid/portfolio-reid-manta-example-2.png)
![Example of manta rays](/images/portfolio/reid/portfolio-reid-manta-example-3.png)
![Example of manta rays](/images/portfolio/reid/portfolio-reid-manta-example-4.png)
![Example of manta rays](/images/portfolio/reid/portfolio-reid-manta-example-5.png)

Image credit: Amelia Armstrong and Asia Armstrong

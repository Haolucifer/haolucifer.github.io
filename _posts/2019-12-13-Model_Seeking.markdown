---
layout:     post
title:      "Model Seeking读书笔记"
author:     "JiG"
header-img: "img/post-bg-kuaidi.jpg"
tags: 

  - GAN
  - CVPR2019_paper
---

 

# Model Seeking Generative Adversarial Networks for Diverse Image Synthesis  

[论文地址](http://openaccess.thecvf.com/content_CVPR_2019/html/Mao_Mode_Seeking_Generative_Adversarial_Networks_for_Diverse_Image_Synthesis_CVPR_2019_paper.html)

## Abstract

Most conditional generation tasks expect diverse outputs given a single conditional context. However, conditional generative adversarial networks (cGANs) often focus on the prior conditional information and ignore the input noise vectors, which contribute to the output variations. Recent attempts to resolve the mode collapse issue for cGANs are usually task-specific and computationally expensive. In this work, we propose a simple yet effective regularization term to address the mode collapse issue for cGANs. The proposed method explicitly maximizes the ratio of the distance between generated images with respect to the corresponding latent codes, thus encouraging the generators to explore more minor modes during training. This mode seeking regularization term is readily applicable to various conditional generation tasks without imposing training overhead or modifying the original network structures. We validate the proposed algorithm on three conditional image synthesis tasks including categorical generation, image-to-image translation, and text-to-image synthesis with different baseline models. Both qualitative and quantitative results demonstrate the effectiveness of the proposed regularization method for improving diversity without loss of quality.  



## 摘要

大多数条件生成任务希望给一个单一条件信息能够生成多样的输出。然而，条件生成对抗网络经常专注于先前的条件信息同时忽略输入的噪声向量，这是多样输出的关键贡献。最近人们为条件生成对抗网络重新解决模式崩塌的问题大多还是在任务驱动的具体应用中并且附带了高昂的计算消耗。在本文的工作中，我们提出了一个目前为止简洁有效的正则化项去为条件生成对抗网络解决模式崩塌的问题。该方法显式地使生成的图像与对应的潜码之间的距离比值达到最大，从而鼓励生成器在训练过程中探索更多的次要模式。这种寻求正则化项的模式很容易适用于各种条件生成任务，而不需要增加训练开销或修改原有的网络结构。我们验证了该算法在三个条件图像合成任务上的有效性，包括分类生成、图像-图像转换和文本-图像合成。定性和定量的结果都证明了所提出的正则化方法在不损失质量的情况下提高多样性的有效性。


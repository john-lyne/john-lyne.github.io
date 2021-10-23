---
title: "3D Channel Flow Super-Resolution"
excerpt: "Three dimensional fluid velocity super-resolution. 1<br/><img src='/images/srres2.png'>"
collection: portfolio
---

Super-resolution is a technique used to turn low-resolution images into high-resolution images. The idea is that we provide a network with high resolution images and the corresponding low-resolution representation of those images, and the network learns a mapping from low to high resolutions. The goal is to get a model that can take a blurry image and turn it into a nice crisp high definition image. This technique is used in photo restoration and remote sensing (i.e satellite imagery).

My project involved applying super-resolution to three dimensional volumes of fluid flow. The motivation behind this is that DNS simulations require a lot of memory. So, it would be benificial to compress these databases into a lower resolution so that we can more easily share this data among acamademic researchers in this area. The idea is that we could toss around these low dimensional datasets, and recover the original high dimensional representation with a super-resolution model. I spent a decent amount of time on this project, testing out different networks.
The first network I tested was the SRResnet, where I modified the standard 2 dimensional architechture to support 3D super-resolution instead (this essentially just involved changing from 2D to 3D convolutions with a few tweaks here and there). Then I tried the improved version, the Enhanced Deep Residual Network (EDSR). Finally, I explored adding a discriminator to the mix - creating a EDSR-GAN network. The motivation around adding discriminators to these networks is that while the networks alone perform quite well, they can struggle to get the fine details.
Adding a discriminator introduces a critic that can essentially take a magnifying glass to the fine scales and tell the super-resolution network to work on these areas that it would have otherwise glossed over. For some more insight on GANs and the role of a discriminator, you can check out my post [here](https://john-lyne.github.io/posts/2021-10-GANs/). Qualitative results of this project can be seen below.

<img src='/images/srres.png'>

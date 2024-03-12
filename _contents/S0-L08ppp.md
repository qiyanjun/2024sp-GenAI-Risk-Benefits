---
layout: post
title: FM copyright infrigement 
lecture: W5-FM-copyright-infrigement 
lectureVersion: current
extraContent: 
notes: team-5
video: team-6
tags:
- Mitigate
- Evaluate
---

In this session, our readings cover: 

## Required Readings: 


### Foundation Models and Fair Use
+ Peter Henderson, Xuechen Li, Dan Jurafsky, Tatsunori Hashimoto, Mark A. Lemley, Percy Liang
+ [URL](https://arxiv.org/abs/2303.15715)
+ Existing foundation models are trained on copyrighted material. Deploying these models can pose both legal and ethical risks when data creators fail to receive appropriate attribution or compensation. In the United States and several other countries, copyrighted content may be used to build foundation models without incurring liability due to the fair use doctrine. However, there is a caveat: If the model produces output that is similar to copyrighted data, particularly in scenarios that affect the market of that data, fair use may no longer apply to the output of the model. In this work, we emphasize that fair use is not guaranteed, and additional work may be necessary to keep model development and deployment squarely in the realm of fair use. First, we survey the potential risks of developing and deploying foundation models based on copyrighted content. We review relevant U.S. case law, drawing parallels to existing and potential applications for generating text, source code, and visual art. Experiments confirm that popular foundation models can generate content considerably similar to copyrighted material. Second, we discuss technical mitigations that can help foundation models stay in line with fair use. We argue that more research is needed to align mitigation strategies with the current state of the law. Lastly, we suggest that the law and technical mitigations should co-evolve. For example, coupled with other policy mechanisms, the law could more explicitly consider safe harbors when strong technical tools are used to mitigate infringement harms. This co-evolution may help strike a balance between intellectual property and innovation, which speaks to the original goal of fair use. But we emphasize that the strategies we describe here are not a panacea and more work is needed to develop policies that address the potential harms of foundation models.

### Extracting Training Data from Diffusion Models

+ Nicholas Carlini, Jamie Hayes, Milad Nasr, Matthew Jagielski, Vikash Sehwag, Florian Tramèr, Borja Balle, Daphne Ippolito, Eric Wallace
+ Image diffusion models such as DALL-E 2, Imagen, and Stable Diffusion have attracted significant attention due to their ability to generate high-quality synthetic images. In this work, we show that diffusion models memorize individual images from their training data and emit them at generation time. With a generate-and-filter pipeline, we extract over a thousand training examples from state-of-the-art models, ranging from photographs of individual people to trademarked company logos. We also train hundreds of diffusion models in various settings to analyze how different modeling and data decisions affect privacy. Overall, our results show that diffusion models are much less private than prior generative models such as GANs, and that mitigating these vulnerabilities may require new advances in privacy-preserving training.



### A Comprehensive Survey of AI-Generated Content (AIGC): A History of Generative AI from GAN to ChatGPT
  + https://arxiv.org/abs/2303.04226
  + Recently, ChatGPT, along with DALL-E-2 and Codex,has been gaining significant attention from society. As a result, many individuals have become interested in related resources and are seeking to uncover the background and secrets behind its impressive performance. In fact, ChatGPT and other Generative AI (GAI) techniques belong to the category of Artificial Intelligence Generated Content (AIGC), which involves the creation of digital content, such as images, music, and natural language, through AI models. The goal of AIGC is to make the content creation process more efficient and accessible, allowing for the production of high-quality content at a faster pace. AIGC is achieved by extracting and understanding intent information from instructions provided by human, and generating the content according to its knowledge and the intent information. In recent years, large-scale models have become increasingly important in AIGC as they provide better intent extraction and thus, improved generation results. With the growth of data and the size of the models, the distribution that the model can learn becomes more comprehensive and closer to reality, leading to more realistic and high-quality content generation. This survey provides a comprehensive review on the history of generative models, and basic components, recent advances in AIGC from unimodal interaction and multimodal interaction. From the perspective of unimodality, we introduce the generation tasks and relative models of text and image. From the perspective of multimodality, we introduce the cross-application between the modalities mentioned above. Finally, we discuss the existing open problems and future challenges in AIGC.

## More Readings: 


### Audio Deepfake Detection: A Survey
+ https://arxiv.org/abs/2308.14970
+ Audio deepfake detection is an emerging active topic. A growing number of literatures have aimed to study deepfake detection algorithms and achieved effective performance, the problem of which is far from being solved. Although there are some review literatures, there has been no comprehensive survey that provides researchers with a systematic overview of these developments with a unified evaluation. Accordingly, in this survey paper, we first highlight the key differences across various types of deepfake audio, then outline and analyse competitions, datasets, features, classifications, and evaluation of state-of-the-art approaches. For each aspect, the basic techniques, advanced developments and major challenges are discussed. In addition, we perform a unified comparison of representative features and classifiers on ASVspoof 2021, ADD 2023 and In-the-Wild datasets for audio deepfake detection, respectively. The survey shows that future research should address the lack of large scale datasets in the wild, poor generalization of existing detection methods to unknown fake attacks, as well as interpretability of detection results.




###  Copyright Plug-in Market for The Text-to-Image Copyright Protection
+ https://openreview.net/forum?id=pSf8rrn49H 
+ The images generated by text-to-image models could be accused of the copyright infringement, which has aroused heated debate among AI developers, content creators, legislation department and judicature department. Especially, the state-of-the-art text-to-image models are capable of generating extremely high-quality works while at the same time lack the ability to attribute credits to the original creators, which brings anxiety to the artists' community. In this paper, we propose a conceptual framework -- copyright Plug-in Market -- to address the tension between the users, the content creators and the generative models. We introduce three operations in the \copyright Plug-in Market: addition, extraction and combination to facilitate proper credit attribution in the text-to-image procedure and enable the digital copyright protection. For the addition operation, we train a \copyright plug-in for a specific copyrighted concept and add it to the generative model and then we are able to generate new images with the copyrighted concept, which abstract existing solutions of portable LoRAs. We further introduce the extraction operation to enable content creators to claim copyrighted concept from infringing generative models and the combination operation to enable users to combine different \copyright plug-ins to generate images with multiple copyrighted concepts. We believe these basic operations give good incentives to each participant in the market, and enable enough flexibility to thrive the market. Technically, we innovate an inverse LoRA'' approach to instantiate the extraction operation and propose a data-ignorant layer-wise distillation'' approach to combine the multiple extractions or additions easily. To showcase the diverse capabilities of copyright plug-ins, we conducted experiments in two domains: style transfer and cartoon IP recreation. The results demonstrate that copyright plug-ins can effectively accomplish copyright extraction and combination, providing a valuable copyright protection solution for the era of generative AIs.


### Membership Inference Attacks against Language Models via Neighbourhood Comparison
https://aclanthology.org/2023.findings-acl.719/ 


### Deepfake Taylor Swift event: 
+ https://www.cbsnews.com/news/taylor-swift-artificial-intellignence-ai-4chan/


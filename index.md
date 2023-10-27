---
layout: project_page
permalink: /

title: Learn to Optimize Denoising Scores - A Unified and Improved Diffusion Prior for 3D Generation
authors:
    .
affiliations:
    .
paper: https://huggingface.co/docs/datasets
video: https://huggingface.co/docs/datasets
code: https://huggingface.co/docs/datasets
data: https://huggingface.co/docs/datasets
---

<div class="columns is-centered has-text-centered">
    <div class="column is-four-fifths">
        <h2>Abstract</h2>
        <div class="content has-text-justified">
We present a unified framework aimed at improving the diffusion priors on 3D generation problems guided by diffusion models. Despite the significance of these tasks, current methods often struggle to produce high-quality results. In this paper, we consolidate the 3D generation problems as an optimization problem given a groundtruth score function, and propose an iterative optimization algorithm to facilitate effective learning. Based on the learnable parameters, our approach offers multiple configurations, affording various trade-offs between performance, implementation complexity, and efficiency. We show in experiments that our method largely improves the baseline methods and achieves new state-of-the-art results in the field of 3D generation. Remarkably, we find that while our primary focus lies in addressing 3D problems, our method demonstrates versatility in its applicability to 2D space, facilitating the generation and manipulation of 2D images. Furthermore, our framework provides valuable insights into recently proposed score distillation methods, such as the VSD loss and DDS loss.
        </div>
    </div>
</div>



![Demo](/static/image/demo.PNG)

*Figure 1: Potential use cases of our proposed diffusion prior. Although we mainly target 3D generation, our method can be used on a wide range of applications, including 2D generation and editing, 3D image-guided generation and 3D text-guided generation.*

## Table: Performance on T3Bench

|     Dataset      | Dreamfusion | Magic3D | LatentNeRF | Fantasia3D | SJC  | ProlificDreamer | LODS (Embedding) | LODS (LoRA) |
|:----------------:|:-----------:|:-------:|------------|------------|------|-----------------|------------------|-------------|
|  Single Object   |    24.4     |  37.0   | 33.1       | 26.4       | 24.7 | 49.4            | **52.3**         |             |
|   Surroundings   |    24.6     |  35.4   | 30.6       | 27.0       | 19.8 | 44.8            | **49.8**         |             |
| Multiple Objects |    16.1     |  25.7   | 20.6       | 18.5       | 11.7 | 35.8            | **39.7**         |             |
|     Average      |    21.7     |  32.7   | 28.1       | 24.0       | 18.7 | 43.3            | **47.3**         |             |

We achieve state-of-the-art performance on T3Bench.

## Generation Results


![](/static/image/demo_gif1.gif)

*A red and white lighthouse on a cliff*

![](/static/image/demo_gif2.gif)

*An intricately-carved wooden chess set*

![](/static/image/demo_gif3.gif)

*A cactus with pink flowers*

![](/static/image/demo_gif4.gif)

*A vintage porcelain doll with a frilly dress*
## Citation
```
@article{yang2023lods,
  title={Learn to Optimize Denoising Scores - A Unified and Improved Diffusion Prior for 3D Generation},
  author={Xiaofeng Yang, Yiwen Chen, Cheng Chen, Fayao Liu and Guosheng Lin},
  journal={Arxiv},
  year={2023}
}
```

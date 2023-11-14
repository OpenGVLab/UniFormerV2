# UniFormerV2

This repo is the official implementation of ["UniFormerV2: Spatiotemporal Learning by Arming Image ViTs with Video UniFormer"](https://arxiv.org/abs/2211.09552).
By [Kunchang Li](https://scholar.google.com/citations?user=D4tLSbsAAAAJ), [Yali Wang](https://scholar.google.com/citations?user=hD948dkAAAAJ), [Yinan He](https://dblp.org/pid/93/7763.html), [Yizhuo Li](https://scholar.google.com/citations?user=pyBSGjgAAAAJ), [Yi Wang](https://scholar.google.com.hk/citations?hl=zh-CN&user=Xm2M8UwAAAAJ), [Limin Wang](https://scholar.google.com/citations?user=HEuN8PcAAAAJ) and [Yu Qiao](https://scholar.google.com/citations?user=gFtI-8QAAAAJ&hl).

## Update

***11/14/2023***

Thanks for Innat'help [@innat](https://github.com/innat). Now our models also support [Keras](https://github.com/innat/UniFormerV2)! 😄

***07/14/2023***

UniFormerV2 has been accepted by ICCV2023! 🎉

***02/13/2023***

UniFormerV2 has been integrated into [MMAction2](https://github.com/open-mmlab/mmaction2/tree/dev-1.x/configs/recognition/uniformerv2). Training code will be provided soon! 😄

***11/20/2022***

We give a video demo in [hugging face](https://huggingface.co/spaces/Andy1621/uniformerv2_demo). Have a try! 😄

***11/19/2022***

We give a blog in Chinese [Zhihu](https://zhuanlan.zhihu.com/p/584669411).

***11/18/2022***

All the code, models and configs are provided. Don't hesitate to open an issue if you have any problem! 🙋🏻 

## Introduction

In UniFormerV2, we propose a generic paradigm to build a powerful family of video networks, by arming the pre-trained [ViTs](https://github.com/rwightman/pytorch-image-models/blob/main/timm/models/vision_transformer.py) with efficient [UniFormer](https://github.com/Sense-X/UniFormer) designs. It inherits the concise style of the UniFormer block. But it contains brand- new local and global relation aggregators, which allow for preferable accuracy-computation balance by seamlessly integrating advantages from both ViTs and UniFormer.
![teaser](img/framework.png)
It gets the state-of-the-art recognition performance on 8 popular video benchmarks, including scene-related Kinetics-400/600/700 and Moments in Time, temporal-related Something-Something V1/V2, untrimmed ActivityNet and HACS. In particular, **it is the first model to achieve 90% top-1 accuracy on Kinetics-400**.

[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/uniformerv2-spatiotemporal-learning-by-arming/action-classification-on-kinetics-400)](https://paperswithcode.com/sota/action-classification-on-kinetics-400?p=uniformerv2-spatiotemporal-learning-by-arming)
[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/uniformerv2-spatiotemporal-learning-by-arming/action-classification-on-kinetics-600)](https://paperswithcode.com/sota/action-classification-on-kinetics-600?p=uniformerv2-spatiotemporal-learning-by-arming)
[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/uniformerv2-spatiotemporal-learning-by-arming/action-classification-on-kinetics-700)](https://paperswithcode.com/sota/action-classification-on-kinetics-700?p=uniformerv2-spatiotemporal-learning-by-arming)
[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/uniformerv2-spatiotemporal-learning-by-arming/action-classification-on-moments-in-time)](https://paperswithcode.com/sota/action-classification-on-moments-in-time?p=uniformerv2-spatiotemporal-learning-by-arming)
[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/uniformerv2-spatiotemporal-learning-by-arming/action-classification-on-activitynet)](https://paperswithcode.com/sota/action-classification-on-activitynet?p=uniformerv2-spatiotemporal-learning-by-arming)
[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/uniformerv2-spatiotemporal-learning-by-arming/action-recognition-on-hacs)](https://paperswithcode.com/sota/action-recognition-on-hacs?p=uniformerv2-spatiotemporal-learning-by-arming)
[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/uniformerv2-spatiotemporal-learning-by-arming/action-recognition-in-videos-on-something-1)](https://paperswithcode.com/sota/action-recognition-in-videos-on-something-1?p=uniformerv2-spatiotemporal-learning-by-arming)
[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/uniformerv2-spatiotemporal-learning-by-arming/action-recognition-in-videos-on-something)](https://paperswithcode.com/sota/action-recognition-in-videos-on-something?p=uniformerv2-spatiotemporal-learning-by-arming)

## Model Zoo

All the models can be found in [MODEL_ZOO](MODEL_ZOO.md).

## Instructions

See [INSTRUCTIONS](INSTRUCTIONS.md) for more details about:
- Environment installation
- Dataset preparation
- Training and validation


##  Cite Uniformer

If you find this repository useful, please use the following BibTeX entry for citation.

```latex
@misc{li2022uniformerv2,
      title={UniFormerV2: Spatiotemporal Learning by Arming Image ViTs with Video UniFormer}, 
      author={Kunchang Li and Yali Wang and Yinan He and Yizhuo Li and Yi Wang and Limin Wang and Yu Qiao},
      year={2022},
      eprint={2211.09552},
      archivePrefix={arXiv},
      primaryClass={cs.CV}
}
```

## License

This project is released under the MIT license. Please see the [LICENSE](LICENSE) file for more information.

## Acknowledgement

This repository is built based on [UniFormer](https://github.com/Sense-X/UniFormer) and [SlowFast](https://github.com/facebookresearch/SlowFast) repository.

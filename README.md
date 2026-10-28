<!-- SVENKUNKKA-README-NAV:BEGIN -->
[English overview](#project-overview-en) · [中文项目说明](#project-overview-zh) · [Maintainer on X / 维护者 X](https://x.com/Svenu1s5)
<!-- SVENKUNKKA-README-NAV:END -->

# Hi3DGen: High-fidelity 3D Geometry Generation from Images via Normal Bridging

<div class="is-size-5 publication-authors">
  <span class="author-block"><a href="https://github.com/hugoycj">Chongjie Ye</a><sup>1,2*</sup>,</span>
  <span class="author-block"><a href="https://yushuang-wu.github.io">Yushuang Wu</a><sup>2*</sup>,</span>
  <span class="author-block"><a href="" onclick="return false;">Ziteng Lu</a><sup>1</sup>,</span>
  <span class="author-block"><a href="https://scholar.google.com/citations?hl=en&user=HA5zLp4AAAAJ">Jiahao Chang</a><sup>1</sup>,</span>
  <span class="author-block"><a href="" onclick="return false;">Xiaoyang Guo</a><sup>2</sup>,</span>
  <span class="author-block"><a href="https://scholar.google.com/citations?hl=en&user=qn61WqgAAAAJ">Jiaqing Zhou</a><sup>2</sup>,</span>
  <span class="author-block"><a href="https://sites.google.com/view/fromandto">Hao Zhao</a><sup>3</sup>,</span>
  <span class="author-block"><a href="https://gaplab.cuhk.edu.cn">Xiaoguang Han</a><sup>1#</sup></span>
</div>


<div class="is-size-5 publication-authors">
  <span class="author-block"><sup>1</sup>The Chinese University of Hong Kong, Shenzhen,&nbsp;&nbsp;</span>
  <span class="author-block"><sup>2</sup>ByteDance,&nbsp;&nbsp;</span>
  <span class="author-block"><sup>3</sup>AIR, Tsinghua University</span>
</div>

![teaser-1](assets/teaser.gif)

<div align="center">

[![Website](https://raw.githubusercontent.com/prs-eth/Marigold/main/doc/badges/badge-website.svg)](https://stable-x.github.io/Hi3DGen/) 
[![Paper](https://img.shields.io/badge/arXiv-PDF-b31b1b)](https://arxiv.org/abs/2503.22236) 
[![Online Demo](https://img.shields.io/badge/🤗%20Hugging%20Face%20-Space-yellow)](https://huggingface.co/spaces/Stable-X/Hi3DGen) 
[![Hugging Face Model](https://img.shields.io/badge/🤗%20Hugging%20Face%20-Model-green)](https://huggingface.co/Stable-X/trellis-normal-v0-1) 
 </div>

Hi3DGen target at generating high-fidelity 3D geometry from images using normal maps as an intermediate representation. The framework addresses limitations in existing methods that struggle to reproduce fine-grained geometric details from 2D inputs.

## Installation
Clone the repo:
```bash
git clone --recursive https://github.com/Stable-X/Hi3DGen.git
cd Hi3DGen
```

Create a conda environment (optional):
```bash
conda create -n stablex python=3.10
conda activate stablex
```

Install dependencies:
```bash
# pytorch (select correct CUDA version)
pip install torch==2.4.0 torchvision==0.19.0 --index-url https://download.pytorch.org/whl/{your-cuda-version}
pip install spconv-cu{your-cuda-version}==2.3.6 xformers==0.0.27.post2
# other dependencies
pip install -r requirements.txt
```

## Local Demo 🤗
Run by:
```bash
python app.py
```

<!-- License -->
## License
The model and code of Hi3DGen are adapted from [**Trellis**](https://github.com/microsoft/TRELLIS), which are licensed under the [MIT License](LICENSE). While the original Trellis is MIT licensed, we have specifically removed its dependencies on certain NVIDIA libraries (kaolin, nvdiffrast, flexicube) to ensure this adapted version can be used commercially. Hi3DGen itself is distributed under the [MIT License](LICENSE).

## Citation
If you find this work helpful, please consider citing our paper:
```
@article{ye2025hi3dgen,
  title={Hi3DGen: High-fidelity 3D Geometry Generation from Images via Normal Bridging},
  author={Ye, Chongjie and Wu, Yushuang and Lu, Ziteng and Chang, Jiahao and Guo, Xiaoyang and Zhou, Jiaqing and Zhao, Hao and Han, Xiaoguang},
  journal={arXiv preprint arXiv:2503.22236}, 
  year={2025}
}
```


---

<!-- SVENKUNKKA-PROJECT-INFO:BEGIN -->

<a id="project-overview-zh"></a>
## 中文项目说明

Hi3DGen 图像到三维几何生成研究项目的 Fork，通过法线图作为中间表示，探索细节几何重建。GitHub 上游为 [Stable-X/Stable3DGen](https://github.com/Stable-X/Stable3DGen)，本仓库保留 Hi3DGen 论文与作者信息。

**使用入口：** 按原 README 配置 Python、匹配 CUDA 的 PyTorch 及依赖后，运行 `python app.py` 启动本地演示；在线演示、论文与模型链接见原 README。

**范围说明：** 代码与模型基于 TRELLIS 适配；环境与模型依赖需按原说明配置，论文作者和上游许可证保持原归属。

<a id="project-overview-en"></a>
## English project overview

A fork of the Hi3DGen image-to-3D geometry research project, using normal maps as an intermediate representation for detailed reconstruction. The GitHub parent is [Stable-X/Stable3DGen](https://github.com/Stable-X/Stable3DGen); this snapshot retains Hi3DGen paper and author information.

**Getting started:** Configure Python, CUDA-matched PyTorch, and dependencies as documented, then run `python app.py` for the local demo. Online demo, paper, and model links are provided in the original README.

**Scope:** Code and models are adapted from TRELLIS. Follow the documented environment and model requirements; research authorship and upstream licensing remain credited.

**本 Fork 的维护者 / Maintainer of this fork:** [SvenKunkka](https://github.com/SvenKunkka) · [X / Twitter](https://x.com/Svenu1s5)

**上游项目 / Upstream:** [Stable-X/Stable3DGen](https://github.com/Stable-X/Stable3DGen)。保留原作者署名与原许可证 / Original authorship and license notices are retained.

<!-- SVENKUNKKA-PROJECT-INFO:END -->

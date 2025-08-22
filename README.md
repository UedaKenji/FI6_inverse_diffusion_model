# IF6 Inverse Diffusion Model

このプロジェクトは、逆拡散モデル（Inverse Diffusion Model）の実装例を提供します。確率微分方程式（SDE）を用いた生成モデルの学習と推論について、Jupyter Notebook形式で解説しています。

## 概要

本リポジトリでは、以下の2つの主要なSDEアプローチを実装しています：

- **VE-SDE (Variance Exploding SDE)**: 分散発散型確率微分方程式
- **VP-SDE (Variance Preserving SDE)**: 分散保存型確率微分方程式

これらのアプローチは、ノイズから高品質な画像やデータを生成するための最先端の生成モデル技術です。

## Notebooks

### VE-SDE Example
分散爆発型SDEの実装例とデモンストレーション

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/UedaKenji/FI6_inverse_diffusion_model/blob/main/VE-SDE_example.ipynb)

### VP-SDE Example  
分散保存型SDEの実装例とデモンストレーション

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/UedaKenji/FI6_inverse_diffusion_model/blob/main/VP-SDE_example.ipynb)

## 使い方

### Google Colabで実行する場合
上記のバッジをクリックして、Google Colab環境で直接ノートブックを開いて実行できます。

### ローカル環境で実行する場合
```bash
git clone https://github.com/UedaKenji/FI6_inverse_diffusion_model.git
cd FI6_inverse_diffusion_model
jupyter notebook
```


## 技術的詳細

これらのノートブックでは、以下のトピックについて紹介しています。

- 確率微分方程式（SDE）に対応するノイズスケジュール
- ニューラルネットワークを用いたスコア関数の学習
- 逆拡散過程によるサンプリングアルゴリズム
- 観測尤度ガイダンス付き拡散モデル(ベイジアン拡散モデル)

## 参考文献

- Song, Y., Sohl-Dickstein, J., Kingma, D. P., Kumar, A., Ermon, S., & Poole, B. (2021). Score-Based Generative Modeling through Stochastic Differential Equations. *International Conference on Learning Representations (ICLR)*. Available at: https://arxiv.org/abs/2011.13456
- Karras, T., Aittala, M., Aila, T., & Laine, S. (2022). Elucidating the Design Space of Diffusion-Based Generative Models. *Advances in Neural Information Processing Systems (NeurIPS)*, 35. Available at: https://arxiv.org/abs/2206.00364
- Chung, H., Kim, J., Mccann, M. T., Klasky, M. L., & Ye, J. C. (2023). Diffusion Posterior Sampling for General Noisy Inverse Problems. *International Conference on Learning Representations (ICLR)*. Available at: https://arxiv.org/abs/2209.14687
- Daras, G., Chung, H., Lai, C.-H., Mitsufuji, Y., Ye, J. C., Milanfar, P., Dimakis, A. G., & Delbracio, M. (2024). A Survey on Diffusion Models for Inverse Problems. *arXiv preprint arXiv:2410.00083*. Available at: https://arxiv.org/abs/2410.00083


## ライセンス

このプロジェクトはMITライセンスの下で公開されています。
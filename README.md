# ok-ap-x-anylabeling-asset

《蓝色星原：旅谣》（Azur Promilia）ok-ap 的模板源文件仓库（submodule）。

本仓库存放 `ok_templates/` 的模板源文件：使用 [x-anylabeling](https://github.com/CVHub520/X-AnyLabeling) 标注的模板图片与标注文件，供 ok-ap 主仓库通过 submodule 引用。

## 目录结构

```
├── .github/workflows/   CI（下载量统计）
├── assets/              生成的下载量统计 SVG
├── scripts/             工具脚本
└── *.png / *.json       模板图片与标注文件（x-anylabeling 格式）
```

## 使用方式

主仓库通过 git submodule 引用本仓库：

```bash
git clone --recurse-submodules https://github.com/AliceJump/ok-ap.git
```

## 维护

- 模板图片与标注文件由 [x-anylabeling](https://github.com/CVHub520/X-AnyLabeling) 生成，标注后提交到本仓库根目录。
- 下载量统计由 GitHub Actions 每日自动更新 `assets/downloads.svg`。

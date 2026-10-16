# QTMS_Meshmodels

Meshy 生成的 3D 模型归档，由 **leewensong** 维护。

## 本次同步

| 内容 | 数量 |
| --- | ---: |
| GLB 模型 | 40 |
| 模型预览图 | 40 |
| 成功任务 | 40 |
| 失败任务记录（不含模型） | 1 |

模型和预览图合计 **620,190,053 字节（591.46 MiB）**。归档校验时间：2026-10-17T05:01:18+08:00。

![全部模型缩略图](contact_sheet.jpg)

## 目录结构

每个 `名称__完整任务ID/` 目录包含：

- `model.glb`：3D 模型（由 Git LFS 管理）。
- `preview.png`：模型生成后的预览图，**不是原始输入参考图**。
- `metadata.json`：任务 ID、状态、时间、模型统计与文件 SHA-256。

根目录文件：

- `index.html`：下载后可在浏览器中打开的模型浏览页。
- `manifest.json` / `manifest.csv`：完整模型与任务清单。
- `SHA256SUMS`：已发布文件的 SHA-256 校验清单。

已有归档不会因为云端历史任务不再列出而删减。失败任务的目录仅含状态记录。

## 克隆和下载完整模型

请先安装 Git LFS，再运行：

```bash
git lfs install
git clone https://github.com/leewensong/QTMS_Meshmodels.git
cd QTMS_Meshmodels
git lfs pull
```

如果 GLB 文件只有约一百字节，并显示 `version https://git-lfs.github.com/spec/v1`，说明拿到的是 LFS 指针，需要执行 `git lfs pull`。

## 后续同步

将经过校验的新模型、预览图及对应清单放入本仓库工作目录后：

```bash
git add .
git commit -m "Update model archive"
git push origin main
```

新增模型会按 `.gitattributes` 中的规则交给 Git LFS 管理。

## 安全与范围

- 仅归档已有模型、预览图和脱敏任务清单，没有提交新的 Meshy 生成任务。
- 不包含 API token、授权请求头、临时签名下载地址、原项目源码或本机绝对路径。
- 原始本地模型目录保持不变。
- 模型的使用和分发权限须遵循原始素材及生成服务的相应条款；本仓库未额外授予许可。

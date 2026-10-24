# QTMS_Meshmodels

Meshy 生成的 3D 模型归档，由 **FXGVR** 组织维护。

## 当前内容

- 任务记录：**43**
- 含模型的任务：**43**
- GLB 模型文件：**43**
- 模型预览图：**43**
- 模型与预览图大小：**1,045,510,963 bytes (997.08 MiB)**

![模型缩略图总览](contact_sheet.jpg)

## 目录结构

每个任务目录 `名称__任务ID/` 包含 GLB 模型、可用时的 `preview.png` 和 `metadata.json`。

根目录包含 `index.html`、`manifest.json`、`manifest.csv`、`SHA256SUMS`、多 KEY 同步记录和清理记录。

## 克隆并下载模型

```bash
git lfs install
git clone https://github.com/FXGVR/QTMS_Meshmodels.git
cd QTMS_Meshmodels
git lfs pull
```

## 最近清理

已移除芭蕾舞演员相关模型、没有预览图的 Rig/Animation 输出，以及失败任务记录。旧 Git 提交历史可能仍保留历史文件。

## 安全范围

未提交 Meshy API KEY、授权头、临时签名 URL 或本机绝对路径；本次只清理和整理已有文件，没有发起新的生成请求。

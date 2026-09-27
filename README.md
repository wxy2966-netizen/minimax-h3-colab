# MiniMax-H3 Colab A100 Deployment Hub

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/wxy2966-netizen/minimax-h3-colab/blob/main/minimax_h3_comfyui_a100.ipynb)

MiniMax-H3（海螺3）在 Google Colab A100 (80GB SXM4) 上的极速部署环境，集成了 **SageAttention** 加速、**ComfyUI** 节点生态、**Google Drive** 权重挂载持久化以及 **Cloudflare Tunnel** 公网穿透。

## 🚀 极速启动 (2 步)

1. 点击上方的 **`Open In Colab`** 徽标进入 Google Colab。
2. 在 Colab 菜单栏选择 **`Runtime` -> `Change runtime type`**，硬件加速器选择 **GPU: A100**。
3. 点击 **`Runtime` -> `Run all` (快捷键 Ctrl+F9)**。
4. 运行完成后，控制台底部会输出 Cloudflare 穿透链接（如 `https://xxxx.trycloudflare.com`）。

## 📡 本地 Antigravity 自动化调度

在本地知识库终端中运行配套客户端，即可自动派发任务并下载渲染视频：

```bash
python scripts/colab_h3_client.py --url "https://xxxx.trycloudflare.com" --prompt "东方仙子，淡青色汉服，竹林回眸微笑"
```

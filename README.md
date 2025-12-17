# SoulStudio


## 第三方 Docker 镜像
```bash
# 参考文档 https://github.com/YanWenKun/ComfyUI-Docker/blob/main/README.zh.adoc
docker pull yanwk/comfyui-boot:cu128-slim
docker pull yanwk/comfyui-boot:cu128-megapak
```

## 引入第三方库

### ComfyUI-Docker
🐳Dockerfile for 🎨ComfyUI. | 容器镜像与启动脚本
```bash
# 引入 ComfyUI-Docker 库, 版本为 main, 并将其添加到 third_party/ComfyUI-Docker 目录
git remote add -f ComfyUI-Docker https://github.com/YanWenKun/ComfyUI-Docker.git
git subtree add --prefix=third_party/ComfyUI-Docker ComfyUI-Docker main --squash

# 更新 ComfyUI-Docker 库
git fetch ComfyUI-Docker main
git subtree pull --prefix=third_party/ComfyUI-Docker ComfyUI-Docker main --squash
```
### ComfyUI
The most powerful and modular diffusion model GUI, api and backend with a graph/nodes interface.
```bash
# 引入 ComfyUI 库, 版本为 v0.4.0, 并将其添加到 third_party/ComfyUI 目录
git remote add -f ComfyUI https://github.com/comfyanonymous/ComfyUI.git
git subtree add --prefix=third_party/ComfyUI ComfyUI v0.4.0 --squash

# 更新 ComfyUI 库
git fetch ComfyUI v0.4.0
git subtree pull --prefix=third_party/ComfyUI ComfyUI v0.4.0 --squash

# 切换到 master 分支
git fetch ComfyUI master
git subtree pull --prefix=third_party/ComfyUI ComfyUI master --squash
```

### Pixelle-MCP
An Open-Source Multimodal AIGC Solution based on ComfyUI + MCP + LLM https://pixelle.ai
```bash
# 引入 Pixelle-MCP 库, 版本为 main, 并将其添加到 third_party/Pixelle-MCP 目录
git remote add -f Pixelle-MCP https://github.com/AIDC-AI/Pixelle-MCP.git
git subtree add --prefix=third_party/Pixelle-MCP Pixelle-MCP main --squash

# 更新 Pixelle-MCP 库
git fetch Pixelle-MCP main
git subtree pull --prefix=third_party/Pixelle-MCP Pixelle-MCP main --squash
```

### Pixelle-Video
🚀 AI 全自动短视频引擎 | AI Fully Automated Short Video Engine
```bash
# 引入 Pixelle-Video 库, 版本为 main, 并将其添加到 third_party/Pixelle-Video 目录
git remote add -f Pixelle-Video https://github.com/AIDC-AI/Pixelle-Video.git
git subtree add --prefix=third_party/Pixelle-Video Pixelle-Video main --squash

# 更新 Pixelle-Video 库
git fetch Pixelle-Video main
git subtree pull --prefix=third_party/Pixelle-Video Pixelle-Video main --squash
```
## ComfyUI 自定义节点
### IndexTTS2
```bash
# 引入 IndexTTS2 库, 版本为 main, 并将其添加到 third_party/custom_nodes/IndexTTS2 目录
git remote add -f IndexTTS2 https://github.com/snicolast/ComfyUI-IndexTTS2.git
git subtree add --prefix=third_party/custom_nodes/IndexTTS2 IndexTTS2 main --squash

# 更新 IndexTTS2 库
git fetch IndexTTS2 main
git subtree pull --prefix=third_party/custom_nodes/IndexTTS2 IndexTTS2 main --squash
```

# CT500 Engineer Updates

本仓库仅用于托管 **CT500 气体质量流量控制器（工程师版）** 的客户端自动更新文件。

- 检查清单：仓库 `main` 根目录的 [`latest.json`](./latest.json)
- 安装包：通过 [Releases](../../releases) 附件发布（不要把大体积 `.exe` 直接 commit 进 git）

客户端固定检查地址：

```text
https://raw.githubusercontent.com/darkteethxu/CT500-Engineer-Updates/main/latest.json
```

## 发版步骤

1. 在源码项目执行：`python build_mfc.py x.y.z --installer`
2. 本仓库创建 Release，Tag 填 `vx.y.z`，上传 Setup.exe
3. 用生成的 `installer/latest.json` 覆盖本仓库根目录的 `latest.json` 并推送到 `main`

仓库需保持 **Public**。

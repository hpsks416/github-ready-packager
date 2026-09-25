# github-ready-packager

把一个已有本地项目收敛成独立、干净、可直接 `git push` 或交给 GitHub 的项目。默认只准备“独立目录 + zip”，不擅自提交。

## 环境依赖

- 操作系统：Windows
- 运行时：Python 3（标准库）
- 第三方软件：无（仅依赖系统自带的 PowerShell / 标准库）

## 目录结构

    github-ready-packager/
    ├── SKILL.md    技能入口与工作流
    ├── evals.yaml
    ├── agents\openai.yaml
    ├── scripts\package_for_github.py

## 安装

    # GitHub
    git clone https://github.com/hpsks416/github-ready-packager.git "$env:USERPROFILE\.dsh\skills\github-ready-packager"
    # 或 Gitee（国内直连）
    git clone https://gitee.com/hpsks416/github-ready-packager.git "$env:USERPROFILE\.dsh\skills\github-ready-packager"

克隆后 DSH 自动重新发现，无需构建。

## License

MIT License. See [LICENSE](LICENSE).

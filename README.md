# github-ready-packager

把一个已有本地项目收敛成独立、干净、可直接 `git push` 或交给 GitHub 的项目。默认只准备“独立目录 + zip”，不擅自提交。

## 适用对象

- DeepSeek Harness（DSH）用户：一个可由 AI agent 按需自动加载的 skill，克隆即用、无需构建。
- 想把本地项目整理成可直接提交 GitHub 仓库的人

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

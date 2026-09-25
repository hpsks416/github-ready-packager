# github-ready-packager

将本地项目整理为可直接提交 GitHub 的独立项目：补齐 .gitignore/README/依赖清单与启动脚本，排除密钥和大文件，校验后打成 zip（可选初始化 git 仓库）。适用于“打包/整理成 GitHub 项目、提交 GitHub”类请求，不用于普通代码编辑或提交后的 Git 操作。

## 这是什么

DSH（DeepSeek Harness）skill —— 一个可由 AI agent 按需自动加载的能力单元。克隆到 skill 目录后，DSH 会依据上方描述自动发现并触发它，无需构建。

## 安装

最简单：用 [dsh-config](https://github.com/hpsks416/dsh-config) 的一键脚本 `install.ps1` 批量安装全部 skill。单个安装：

    # GitHub
    git clone https://github.com/hpsks416/github-ready-packager.git "$env:USERPROFILE\.dsh\skills\github-ready-packager"
    # 或 Gitee（国内直连更快）
    git clone https://gitee.com/hpsks416/github-ready-packager.git "$env:USERPROFILE\.dsh\skills\github-ready-packager"

克隆后 DSH 会自动重新发现，无需重启。更新用：

    git -C "$env:USERPROFILE\.dsh\skills\github-ready-packager" pull

## 目录结构

    github-ready-packager/
    ├── SKILL.md    技能入口与工作流
    ├── agents\openai.yaml
    ├── evals.yaml
    ├── scripts\package_for_github.py

## 依赖

脚本以 Python 3 标准库为主，无第三方依赖（个别脚本如需额外依赖，见文件头注释）。

## License

MIT License. See [LICENSE](LICENSE).

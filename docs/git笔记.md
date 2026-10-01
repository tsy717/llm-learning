# Git 学习笔记

## 三大区域
1. **工作区（Working Directory）**：本地文件夹，VS Code编辑文件的地方
2. **暂存区（Stage/Index）**：git add 后存放改动的临时区域
3. **版本库（Repository）**：.git目录，git commit 后保存版本快照

## 核心命令
```bash
git init                    # 初始化本地仓库
git config --global user.name "用户名"   # 配置用户名
git config --global user.email "邮箱"    # 配置邮箱
git status                  # 查看仓库状态
git diff <file>             # 查看文件具体改动
git add <file>              # 工作区 → 暂存区
git commit -m "说明"        # 暂存区 → 版本库
git log                     # 查看提交历史
git log --oneline           # 精简版历史
git remote add origin <url> # 关联远程仓库
git push -u origin master   # 第一次推送到远程
git push                    # 后续推送
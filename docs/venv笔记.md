# Python venv 虚拟环境笔记

## venv 作用
- **环境隔离**：不同项目的Python包版本互不干扰
- A项目装 requests 2.0，B项目装 requests 3.0，互不影响
- 不会污染系统全局Python

## 常用命令
python -m venv venv          # 创建虚拟环境
source venv/Scripts/activate # 激活（Windows Git Bash）
deactivate                   # 退出虚拟环境
pip install <包名>           # 安装包（激活状态下）
pip list                     # 查看已安装的包

## 注意
- venv 文件夹只存在本地，不要提交到GitHub
- 靠 .gitignore 忽略 venv/ 文件夹
- 别人克隆你的仓库后，自己重新创建venv
# GitHub仓库初始化与后续操作指南

*本指南由樱琳大人亲自整理，看好了别搞错了～*

## 一、创建仓库（CREATE REPOSITORY）入口在哪？
**听好了！** GitHub创建仓库的入口在页面**右上角**，点击那个**"+"号图标**，在弹出的下拉菜单中选择**"New repository"**，这就是CREATE REPOSITORY的入口！

## 二、初始化仓库时添加README的位置
进入创建仓库页面后，填写完**Repository name**（仓库名称，必填）和**Description**（描述，可选）后，往下滚动一点，就能看到一个复选框：

**【Initialize this repository with a README】**

✓ 一定要勾选它！这样GitHub会自动为你创建README.md文件，省得你手动创建～

如果已经创建了仓库但没勾这个选项，往下看补救方法～

## 三、没有README的仓库怎么办？
1. 先把仓库克隆到本地：
   ```bash
   git clone https://github.com/你的用户名/你的仓库名.git
   ```
2. 进入克隆的文件夹：
   ```bash
   cd 你的仓库名
   ```
3. 创建README.md文件：
   - 右键新建文本文件，改名为`README.md`
   - 或用命令：`echo '# 项目名称' > README.md`
4. 添加并提交：
   ```bash
   git add README.md
   git commit -m '添加README文件'
   git push origin main
   ```

## 四、创建仓库的完整步骤
1. 登录GitHub账号，进入主页
2. 点击右上角"+"→"New repository"
3. 填写仓库名称（必填）
4. 填写描述（可选）
5. 选择仓库类型（公开Public/私有Private，默认选Public）
6. 勾选"Initialize this repository with a README"
7. 可选：添加.gitignore和License
8. 点击"Create repository"按钮，完成创建！

## 五、后续基本操作步骤
1. **克隆仓库**（第一次获取代码）：
   ```bash
   git clone https://github.com/你的用户名/你的仓库名.git
   ```

2. **将本地网页文件上传到仓库**：
   ```bash
   # 复制你的网页文件到克隆的仓库文件夹中
   # 查看修改
   git status
   # 添加所有文件
   git add .
   # 提交修改
   git commit -m '上传网页文件'
   # 推送到GitHub
   git push origin main
   ```

3. **从GitHub获取最新代码**（多人协作时）：
   ```bash
   git pull origin main
   ```

*樱琳大人友情提示：命令要在Git Bash里执行，仓库名要和你创建的一致哦～别问本公主为什么知道，因为本公主什么都懂～*
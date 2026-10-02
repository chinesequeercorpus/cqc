# Chinese Queer Corpus (CQC) — website

This repository contains only the public website for CQC. **No corpus data, audio, transcripts, or metadata are stored here.**

Website: https://YOUR-ACCOUNT.github.io/cqc/  ·  Contact: your-cqc-address@outlook.com

---

## 搭建步骤（GitHub Pages）

### 0. 发布前先改三处
1. **邮箱**：用文本编辑器（VS Code 最方便）在全部 `.html` 文件里“查找并替换” `your-cqc-address@outlook.com` → 你们的 Outlook 地址。VS Code：左侧放大镜图标 → 输入旧地址 → 输入新地址 → 点“全部替换”。
2. **TODO**：全局搜索 `TODO`，逐一填写。网页上黄色高亮的 `[TODO: …]` 就是这些位置。全部填完后，搜索结果应为 0。
3. **数字**：`corpus.html` 中 gender identity / trans status 表格要等原始 metadata 核对完再填，并与论文保持一致。

### 1. 注册 / 登录 GitHub
到 https://github.com 注册。建议建一个**组织账号**（右上角头像 → Your organizations → New organization → Free），名字比如 `chinese-queer-corpus`，这样网址不挂在个人名下，多位成员也都能管理。

### 2. 新建仓库
右上角 **+** → **New repository**
- Owner：选上一步的组织（或你自己）
- Repository name：`cqc`（网址会是 `https://<owner>.github.io/cqc/`）
- 选 **Public**（免费账号的 Pages 只能从公开仓库发布）
- 不要勾选 “Add a README”
- 点 **Create repository**

### 3. 上传文件
在新仓库页面点 **uploading an existing file**，把文件夹里的所有文件拖进去：
`index.html`, `corpus.html`, `access.html`, `agreement.html`, `ethics.html`, `about.html`, `zh.html`, `styles.css`, `README.md`, `.nojekyll`

> `.nojekyll` 是隐藏文件（以点开头），Mac 的 Finder 默认不显示。按 `Cmd + Shift + .` 显示隐藏文件后再拖。漏传它网站一般也能正常显示，但传上去更稳妥。

页面底部写一句说明（如 “Initial website”），点 **Commit changes**。

### 4. 打开 GitHub Pages
仓库 → **Settings** → 左栏 **Pages**
- Source：**Deploy from a branch**
- Branch：**main**，文件夹 **/ (root)** → **Save**

等 1–3 分钟，刷新这一页，顶部会出现 “Your site is live at …”。点开检查。

### 5. 检查
- 用手机打开一遍，看导航和表格是否正常。
- 点 “Email an application” 和 “Email a removal request” 按钮，确认会打开邮件并带有模板。
- 每一页都点一遍链接。

### 6. 以后怎么改
- 小改动：在 GitHub 上打开文件 → 右上角铅笔图标 → 修改 → **Commit changes**，1–2 分钟后网站更新。
- 换文件：**Add file → Upload files**，上传同名文件会覆盖旧文件。
- 页脚的 “Last updated” 记得同步更新。

### 7. （可选）自定义域名
如果学校或你们有域名，在 Settings → Pages → Custom domain 填入，并在域名服务商处加一条 CNAME 记录指向 `<owner>.github.io`。

---

## 注意事项
- **双盲评审**：ICPhS 评审期间，论文里不要放这个网址；网站上不要写 “paper under review at ICPhS 2027”。如果担心审稿人搜到作者姓名，可以等到录用结果出来后再在 `about.html` 填写成员姓名。
- **仓库是公开的**：任何人都能看到仓库里的所有文件和修改历史。绝对不要上传音频、转写、TextGrid 或说话人信息，删除后历史记录里仍能找到。
- **小样本**：`corpus.html` 公开了各类别人数（包括 n = 1 的类别）。如果你们决定按 DUA 的小样本规则处理，网站上也应合并或删去这些行。
- **Outlook 申请表单（可选）**：如果想用表单代替邮件，可以用 Microsoft Forms 做一个申请表，把 `access.html` 里 “Email an application” 按钮的链接换成表单链接。

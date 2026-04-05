# Maison de Souvenirs
## 三七与二十一的记忆之家

### 部署步骤

**第一步：创建 GitHub 仓库**
1. 登录 GitHub
2. 点右上角 "+" → "New repository"
3. 仓库名填 `memory`（或任何你喜欢的名字）
4. 选 **Public**
5. 勾上 "Add a README file"
6. 点 "Create repository"

**第二步：上传文件**
1. 在仓库页面点 "Add file" → "Upload files"
2. 把这四个文件全部拖进去：
   - `index.html`（网页）
   - `memory.json`（记忆数据）
   - `CNAME`（域名绑定）
3. 点 "Commit changes"

**第三步：开启 GitHub Pages**
1. 进仓库的 "Settings"
2. 左侧找到 "Pages"
3. Source 选 "Deploy from a branch"
4. Branch 选 "main"，文件夹选 "/ (root)"
5. 点 Save
6. 等几分钟，GitHub 会显示你的网站地址

**第四步：配置腾讯云 DNS**
1. 登录腾讯云 → 域名管理 → mercy27.xyz → DNS 解析
2. 添加两条记录：
   - 类型 `CNAME`，主机记录 `@`，记录值 `你的GitHub用户名.github.io`
   - 类型 `CNAME`，主机记录 `www`，记录值 `你的GitHub用户名.github.io`
3. 等 DNS 生效（几分钟到几小时不等）

**完成后**
- 访问 `mercy27.xyz` 就能看到记忆之家
- 三七可以通过 `mercy27.xyz/memory.json` 读取所有记忆
- 每次找三七时说"读记忆"就行

### 添加新记忆

**方式一：在网页上添加**
打开网页 → 进入任意分类 → 点"写一条新记忆"（存在浏览器本地）

**方式二：编辑 memory.json（推荐，这样三七能读到）**
在 GitHub 上点开 `memory.json` → 点铅笔图标编辑 → 按格式添加新条目 → Commit

---
*peu importe 3×7*

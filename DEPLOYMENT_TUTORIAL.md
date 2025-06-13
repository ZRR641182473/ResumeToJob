# ResumeToJob 本地运行教程

**🎯 适合完全小白的简单教程**
如果等了好久还没进入网站，也没有梯子 🪜，看此教程

这个教程将手把手教你如何在自己的电脑上运行 ResumeToJob 简历制作网站。整个过程只需要 6 个简单步骤，大约 10-15 分钟即可完成。

## 📋 简单 6 步搞定

1. [下载 VS Code 编辑器](#步骤-1-下载-vs-code-编辑器)
2. [下载 Node.js 运行环境](#步骤-2-下载-nodejs-运行环境)
3. [下载项目源代码](#步骤-3-下载项目源代码)
4. [解压并打开项目](#步骤-4-解压并打开项目)
5. [安装项目依赖](#步骤-5-安装项目依赖)
6. [启动网站](#步骤-6-启动网站)


## 🛠️ 准备工作

确保你有电脑，而不是手机。

## 步骤 1: 下载 VS Code 编辑器

VS Code 是一个免费的代码编辑器，我们用它来查看和修改代码。

### Windows 用户

1. 打开浏览器，访问：https://code.visualstudio.com/
2. 点击蓝色的 **"Download for Windows"** 按钮

### Mac 用户

1. 打开浏览器，访问：https://code.visualstudio.com/
2. 点击 **"Download for Mac"** 按钮

---

## 步骤 2: 下载 Node.js 运行环境

Node.js 是运行网站必需的程序，就像电脑需要操作系统一样。

### 所有系统通用步骤

1. 打开浏览器，访问：https://nodejs.org/
2. 下载 22 的 lts 版本就行

### 验证安装

1. **Windows**: 按 `Win + R`，输入 `cmd`，按回车
2. **Mac**: 按 `Cmd + 空格`，输入"终端"，按回车
3. 在打开的黑色窗口中输入以下命令并按回车：

```bash
node --version
```

如果显示类似 `v18.17.0` 这样的版本号，说明安装成功！

---

## 步骤 3: 下载项目源代码

我们需要把 ResumeToJob 的代码下载到你的电脑上。

### 下载方式

1. 打开浏览器，访问：https://github.com/ltlylfun/ResumeToJob
2. 找到绿色的 **"Code"** 按钮，点击它
3. 在弹出的菜单中，点击 **"Download ZIP"**
4. 选择一个容易找到的位置保存（比如桌面或下载文件夹）
5. 等待下载完成

💡 **小贴士**: 下载的文件名应该是 `ResumeToJob-main.zip`

---

## 步骤 4: 解压并打开项目

现在我们要解压下载的文件，并用 VS Code 打开。

### 解压文件

1. 找到刚才下载的 `ResumeToJob-main.zip` 文件
2. 解压后会得到一个名为 `ResumeToJob-main` 的文件夹

### 用 VS Code 打开项目

1. 双击打开 VS Code
2. 点击菜单 **"文件"** → **"打开文件夹"**
   - **Windows**: `File` → `Open Folder`
   - **Mac**: `File` → `Open...`
3. 选择刚才解压的 `ResumeToJob-main` 文件夹
4. 点击 **"选择文件夹"** 或 **"打开"**

现在你应该能在 VS Code 左侧看到项目的文件列表了！

---

## 步骤 5: 安装项目依赖

项目需要一些额外的组件才能运行，我们用一条命令就能自动下载安装。

### 打开终端

在 VS Code 中：

1. 点击顶部菜单 **"终端"** → **"新建终端"**
2. 或者按快捷键：
   - **Windows**: Ctrl + j
   - **Mac**: Cmd + j

VS Code 底部会出现一个黑色的终端窗口。

### 安装依赖

在终端中输入以下命令并按回车：

```bash
npm install
```

### 等待安装完成

- 这个过程可能需要一点时间，请耐心等待
- 你会看到很多文字在滚动，这是正常的
- 如果网络较慢，可以尝试使用国内镜像：

```bash
npm config set registry https://registry.npmmirror.com/
npm install
```

安装完成后，你会看到类似这样的信息：

```
added 1234 packages in 2m
```

---

## 步骤 6: 启动网站

最后一步！让我们启动网站吧。

### 启动开发服务器

在终端中输入以下命令并按回车：

```bash
npm run dev
```

### 成功提示

如果一切正常，你会看到类似这样的信息：

```
> resume-to-job@1.0.0 dev
> next dev

- ready started server on 0.0.0.0:3000, url: http://localhost:3000
- event compiled client and server successfully
```

### 访问网站

1. 打开浏览器（Chrome、Edge、Safari 等）
2. 在地址栏输入：`http://localhost:3000`
3. 按回车

🎉 **恭喜！** 如果你看到了 ResumeToJob 的主页，说明成功了！

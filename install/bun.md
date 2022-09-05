# BUN 安装文档
<p align="center">
  <a href="https://bun.sh"><img src="https://user-images.githubusercontent.com/709451/182802334-d9c42afe-f35d-4a7b-86ea-9985f73f20c3.png" alt="Logo" height=170></a>
</p>

## 安装
1、使用安装命令安装 bun

```
curl https://bun.sh/install | bash
```

2、安装成功
```
bun was installed successfully to ~/.bun/bin/bun

Added "~/.bun/bin" to $PATH in "~/.zshrc"

To get started, run:

 exec /bin/zsh
  bun --help
```
安装成功后，出现如上提示后，使用 `exec` 调用目录即可执行 `bun` 命令

3、使用

```
bun install
```
> 在 Linux 上，bun install 安装包的速度往往比 npm install 快 20 到 100 倍。在 macOS 上，速度快 4x - 80x

```
bun remove react
bun add preact
```
>要从 package.json 添加或删除包：


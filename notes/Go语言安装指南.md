​
1. 引言
Go（又称 Golang）是 Google 推出的一门开源编程语言，以简洁的语法、高效的并发模型和快速的编译速度著称。本文记录我从0学习Go的流程（安装篇）

2. 下载 Go 安装包
访问 Go 官方下载页面，根据操作系统选择对应的安装包：http://go.dev/doc/install
​​​​



Windows：下载 .msi 安装包。
macOS：下载 .pkg 安装包，或通过 Homebrew 安装。
Linux：下载 .tar.gz 压缩包。
3. 安装步骤
Windows 安装


双击运行 .msi 文件，按照向导提示完成安装。



默认安装路径为 C:\Program Files\Go，安装完成后会自动配置环境变量。

4. 配置环境变量
Go 依赖几个关键环境变量来管理开发环境。

GOROOT：Go 安装目录，通常无需手动设置。
GOPATH：工作目录，存放源码、依赖和编译产物。
GOBIN：编译后二进制文件的输出目录。
5. 验证安装
打开终端或命令行，输入 go version 命令验证安装是否成功：



如果输出类似go version go1.27.0 windows/amd64 的信息，说明安装成功。

Go Tools Suite包含几个不同的命令和子命令，输入 go help 即可查看这些命令的列表。



6. 编写第一个 Go 程序
打开工作区软件，我用的VS Code。创建一个名字为goworkspace的文件夹，在里面创建hello.go文件



输入以下代码：

package main

import "fmt"

func main() {
	fmt.Println("Hello World!")
}

在终端Terminal中运行：

go run hello.go
看到输出 Hello, World! 即表示开发环境完全就绪。

​
# 安装与使用

fan 解释器使用 Go 实现。

## 从源码构建

需要先安装 [Go](https://go.dev/dl/)（建议 1.21 或更高版本）。

```bash
git clone git@github.com:china-lan-fan/fan.git
cd fan
go build -o fan ./cmd/fan
```

将生成的 `fan` 可执行文件放到系统 PATH 中，即可使用。

## 运行脚本

编写一个 `hello.fan`：

```fan
打印 "你好，fan"
```

运行：

```bash
fan run hello.fan
```

输出：

```text
你好，fan
```

## 交互式模式（REPL）

```bash
fan repl
```

进入后可以逐行输入表达式：

```text
fan> 1 加 2
3
fan> 变量 名字 = "小明"
fan> 打印 名字
小明
```

输入 `:退出`、`:quit` 或 `:q` 退出 REPL。

## 其他命令

```bash
fan version   # 查看版本
fan help      # 查看帮助
```

## 编辑器支持

官方正在开发编辑器插件：

- JetBrains 插件：[fan-jetbrains-plugin](https://github.com/china-lan-fan/fan-jetbrains-plugin)
- VS Code 插件：[fan-code-plugin](https://github.com/china-lan-fan/fan-code-plugin)

fan 的源文件使用 `.fan` 后缀。

接下来了解 fan 的 [语法风格](./style)。

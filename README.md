# rust-study
学习rust

## 安装

win10

官方文档下载rustup-int.exe*一直点击下一步，可能会由于网速原因导致安装失败，继续安装*

linux 略过

## 快速开始

`cargo new hello-rust`

目录结构
```
hello-rust
    src
        main.rs
    Cargo-toml 类似于npm中的package.json
```

Cargo-toml

```
[package]
name = "hello-rust"
version = "0.1.0"
authors = ["wuhaohao1234 <1611499758@qq.com>"]
edition = "2018"

# See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html

[dependencies]

```

src/main.rs

```
fn main() {
    println!("Hello, world!");
}

```

运行cargo run 

可能会出现的问题是找不到link.exe文件，这个时候需要下载VISUAL STUDIO 2017或者Microsoft Visual C++ Build Tools 2015

https://www.visualstudio.com/downloads

http://go.microsoft.com/fwlink/?LinkId=691126

由于体积过大，是4gb，直接下一步即可

## 入门

### 单文件书写

创建main.rs文件

```
fn main() {
    println!("Hello world");
}
```
编译:

`rustc main.rc`

生成2个文件

main.exe可实行文件
main.pdb调试文件

### cargo

cargo是rust的构建系统，也是包管理器,类似package.json文件

运行cargo创建hello_cargo项目

```
cargo new hello_cargo
```

进入项目

`cd hello_cargo`

编译

`cargo build`

执行

`./target/debug/hello_cargo.exe`

也可以直接运行cargo run 这个时候可以直接编译


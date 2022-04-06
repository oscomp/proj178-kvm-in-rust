# proj178-kvm-in-rust
用Rust语言重写Linux kernel中的KVM

### 项目描述

基于内核的虚拟机 Kernel-based Virtual Machine（KVM）是一种内建于 Linux® 中的开源虚拟化技术。具体而言，KVM 可帮助您将 Linux 转变为虚拟机监控程序，使主机计算机能够运行多个隔离的虚拟环境，即虚拟客户机或虚拟机（VM）。

本项目以Linux Kernel中的KVM为基础，拟采用Rust语言重新设计与实现它。KVM 是 Linux Kernel的一部分。Linux 2.6.20 或更新版本包括 KVM。KVM 于 2006 年首次公布，并在一年后合并到主流 Linux 内核版本中。由于 KVM 属于现有的 Linux 代码，因此它能立即享受每一项新的 Linux 功能、修复和发展，无需进行额外工程。Rust语言与C语言不同，其作为一门现代的系统编程语言，表达能力更强，语义更丰富，所以在用Rust语言参与本项目时，从某种角度上需要我们将一些规则和设计显式地"写"在代码中，这同时也促使了我们去思考。

当前项目实现源码等：

- [kvm in linux](https://github.com/torvalds/linux/search?l=C&q=kvm)
- [kvm社区](https://www.linux-kvm.org/page/Main_Page)

### 所属赛道

2022全国大学生操作系统比赛的“OS功能挑战”赛道

### 参赛要求

- 以小组为单位参赛，最多三人一个小组，且小组成员是来自同一所高校的本科生（2022年春季学期或之后本科毕业的大一~大四的学生）或研究生
- 如学生参加了多个项目，参赛学生选择一个自己参加的项目参与评奖
- 请遵循“20212国大学生操作系统比赛”的章程和技术方案要求

### 项目导师


### 难度

中等 ~ 高等

### 特征

- 符合KVM的语义和它的对外接口
- 使用 Rust 语言实现
- 至少支持一种硬件平台（比如x86, arm, riscv等）
- 支持 QEMU模拟机器上运行
- 支持在物理机器上运行

### 参考实现



### License

- GPL-2 license

## 预期目标

### 注意：下面的内容是建议内容，不要求必须全部完成。选择本项目的同学也可与导师联系，提出自己的新想法，如导师认可，可加入预期目标

**注：为了避免重复造轮子，本项目既可以从头开发，也可以联系导师在其项目基础上进行进一步的开发**

能够在QEMU模拟计算机上运行起来，部分或基本达到kvm的功能，展现出rust写Linux kernel 模块的优缺点。

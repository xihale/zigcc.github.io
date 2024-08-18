---
title: "学习 Zig"
---

{{% blocks/cover title="如何学习 Zig ？" image_anchor="bottom" height="auto" %}}

{{% /blocks/cover %}}

{{% blocks/section color="white" %}}

由于 Zig 目前还处于快速迭代，因此最权威的资料无疑是官方的 [Zig Language Reference](https://ziglang.org/documentation/master/)，遇到语言的细节问题，基本都可以在这里找到答案。 其次是社区的一些高质量教程，例如：

- **[Zig Guide](https://zig.guide/):** 英文资料， [Sobeston](https://github.com/Sobeston) 用户编写
- **[Zig in 30 minutes](https://gist.github.com/ityonemo/769532c2017ed9143f3571e5ac104e50):**
- **[Zig 日报](https://github.com/zigcc/forum/issues):**
- **[学习 Zig](https://learn.ziglang.cc):** 该系列教程最初由 Karl Seguin 编写，该教程行文流畅，讲述的脉络由浅入深，深入浅出，是入门 Zig 非常不错的选择
- **[Zig 语言圣经](https://course.ziglang.cc):** 一份内容全面、深入浅出介绍 Zig 的教程
- **[ziglings/exercises](https://codeberg.org/ziglings/exercises/):** Learn the Zig programming language by fixing tiny broken programs.
- **[Zig Cookbook](https://cookbook.ziglang.cc/):** A collection of simple Zig programs that demonstrate good practices to accomplish common programming tasks
- **[Awesome Zig](https://github.com/zigcc/awesome-zig):** A collection of some awesome public Zig programming language projects.

# 版本管理

推荐使用版本管理工具 [asdf](/post/2023/10/14/zig-version-manager/) 来安装 Zig，具体步骤：

```bash
git clone https://github.com/asdf-vm/asdf.git ~/.asdf --branch v0.14.0
cat <<'EOF' >> $HOME/.bashrc
source "$HOME/.asdf/asdf.sh"
source "$HOME/.asdf/completions/asdf.bash"
EOF

asdf plugin-add zig https://github.com/zigcc/asdf-zig.git

# 安装最新版
asdf install zig latest
asdf global zig latest
zig version
```


{{% /blocks/section %}}
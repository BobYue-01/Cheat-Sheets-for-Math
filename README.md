# 数学速查表  Cheat Sheets for Math

## 关于

本项目是一个使用 $\LaTeX$ 编写数学速查表，包含了数学中常用的公式、定理等，以及一些数学名词的解释。

## 结构

本项目使用 `import` 宏包，以便分章节编译，提升效率。目录结构如下：

```
.
├── main.tex # 主文件
├── preamble # 导言区
│　　├── basic.tex # 基本设置
│　　├── basic # 基本设置
│　　│　　├── math.tex # 数学环境
│　　│　　├── chinese.tex # 中文支持
│　　│　　├── page.tex # 页面设置
│　　│　　└── beauty.tex # 美化
│　　├── pgfplots.tex # 绘图设置
│　　└── tikz.tex # 绘图设置
└── content # 内容
　　　├── titlepage.tex # 封面
　　　├── prolouge.tex # 序言
　　　├── table-of-integrals.tex # 积分表
　　　├── table-of-definitions.tex # 定义表
　　　└── table-of-definitions # 定义表
　　　　　├── abstract-algebra.tex # 抽象代数
　　　　　├── set-theory.tex # 集合论
　　　　　├── topology.tex # 拓扑学
　　　　　└── probability-and-statistics.tex # 概率论与数理统计
```

## 贡献

欢迎大家贡献内容，在此指出一些规范：

### 格式规范

  - 编码、缩进等基本风格请参考本项目已有代码；
  - 请规范使用空格，在中英文之间、符号与文字之间、数学环境与文字之间等处使用空格；
    - ✓ Bob 认为变量 $x$ 为 $0$ `Bob 认为变量 $x$ 为 $0$`  
      ✗ Bob认为变量$x$为$0$`Bob认为变量$x$为$0$`
  - 对于数学公式中的多字母变量，请使用 `\mathrm` 或 `\mathit`；
    - ✓ $\mathrm{difference}$ `\mathrm{difference}`  
      ✓ $\mathit{difference}$ `\mathit{difference}`  
      ✗ $difference$ `difference`

### 编译注意事项

请确保你已安装方正系列字体，并能被 $\LaTeX$ 正常调用。

它们分别是：

  - 方正宋体_GBK
  - 方正小标宋_GBK
  - 方正黑体_GBK
  - 方正楷体_GBK
  - 方正仿宋_GBK

### 提交信息规范

建议以下列分类标识开头：

  - `[doc]` 文档内容的更新
  - `[fix]` 修复编译错误
  - `[fmt]` 格式调整
  - `[chore]` 其他杂项

## 许可

本项目使用 [MIT License](LICENSE) 许可。

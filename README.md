# Open K-12 Math Knowledge Base (开源初中数学全量知识库)

[![License: Apache-2.0](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
[![GitHub Pages](https://img.shields.io/badge/GitHub_Pages-Online-emerald.svg)](https://vivian571.github.io/open-k12-math-kb/)
[![Curriculum: K-12 Math](https://img.shields.io/badge/Curriculum-K--12_Mathematics-cyan.svg)](https://github.com/vivian571/open-k12-math-kb)

本项目是一个面向初中阶段（中考体系）的结构化、可检索、可拓展的开源数学知识库。系统梳理了**七年级数学上册 7 大核心章节、42 个核心考点与拓扑前置依赖树**，并深度收录了**义务教育教科书·数学及最新运算/方程应用强化资料**。

🌐 **在线可视化数学知识库工作台**：[https://vivian571.github.io/open-k12-math-kb/](https://vivian571.github.io/open-k12-math-kb/)

---

## 📚 知识库核心架构

### 1. 中考数学基础考点拓扑图谱 (42 核心考点)
数据文件：[`data/math_topics.json`](data/math_topics.json)

- **第 1 章 有理数的基本概念**：正数负数、有理数分类、数轴三要素、相反数、绝对值非负性、有理数大小比较
- **第 2 章 有理数的运算体系**：加减乘除运算法则与运算律、乘方运算与符号法则（$(-a)^n$ vs $-a^n$）、四则混合运算顺序、科学记数法与有效数字
- **第 3 章 代数式与整式初步**：用字母表示数、代数式的值与整体代入法、单项式与多项式次数与系数
- **第 4 章 整式的加法与减法**：同类项两要素（字母同、指数同）、合并同类项、去括号法则（正不变负全变）、添括号技巧与化简求值
- **第 5 章 一元一次方程的解法**：方程与解的定义、等式的基本性质 1 与 2、移项法则、解方程五部曲（去分母-去括号-移项-合并同类项-系数化为1）
- **第 6 章 一元一次方程与实际问题应用模型**：竞赛积分得分扣分守恒模型、粮仓物资调配模型、工程与协作抽水模型（总量设为1）、行程相遇与追及模型、销售打折与利润率模型
- **第 7 章 基本的几何图形初步**：立体与平面图形展开折叠、两点确定一条直线、两点之间线段最短、角与度分秒换算、角平分线、余角与补角性质

---

### 2. 同步教科书与强化资料库索引
数据文件：[`data/textbooks_catalog.json`](data/textbooks_catalog.json)  
剖析文档：[`docs/textbooks/grade7_math_curriculum.md`](docs/textbooks/grade7_math_curriculum.md)

收录模块：
- **义务教育数学上册教科书**：去手写官方原著，系统梳理数轴、绝对值、去括号法则与标准解方程范例。
- **有理数运算复习巩固卷**：负数乘方符号对比（$(-4)^2$ vs $-4^2$）、科学记数法表示 3000 亿千瓦时大数、交错正负数数列规律探索。
- **一元一次方程解决实际问题精编卷**：科普竞赛抢答得分扣分、甲乙粮仓总量调配守恒、水泵抽水管道检修协作模型。

---

### 3. 点击深入的知识引用与即点即判练习
数据文件：[`data/knowledge_details.json`](data/knowledge_details.json)

每个考点卡片均注入了：
- **📖 课本定义与原篇引用**：溯源自教科书真实定义与定理。
- **📐 核心解题公式与法则**：条理清晰的定理公理及演算步骤。
- **🚨 易错避坑预警**：诊断中考学生高频失误点。
- **✍️ 即点即判随堂练习**：单选题互动自测，实时判断正误并呈现详尽的数学解题推导。

---

## 📂 仓库目录结构

```
open-k12-math-kb/
├── index.html                           # 在线交互式数学知识库平台 (GitHub Pages 部署)
├── README.md                            # 项目说明文档
├── LICENSE                              # Apache-2.0 开源许可协议
├── .gitignore                           # Git 忽略配置
├── data/
│   ├── math_topics.json                 # 7 大章节 42 个核心考点拓扑图谱
│   ├── textbooks_catalog.json           # 教材与强化卷元数据
│   └── knowledge_details.json           # 全量考点引用、解题法则与互动题目库
└── docs/
    ├── CONTRIBUTING.md                  # 贡献规范与验证指南
    └── textbooks/
        └── grade7_math_curriculum.md    # 七上数学教材专题深度剖析
```

---

## 🌐 访问在线工作台

项目已配置 GitHub Pages 自动托管：  
👉 [https://vivian571.github.io/open-k12-math-kb/](https://vivian571.github.io/open-k12-math-kb/)

---

## 📄 开源许可

本项目遵循 [Apache License 2.0](LICENSE) 开源许可协议。

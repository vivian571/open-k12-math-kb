# Math Knowledge Base Contribution Guide (数学知识库贡献规范)

本项目专注于构建高质量、结构化、模块化的初中数学知识库。

## 一、知识库收录范围

1. **数学考点拓扑图谱 (`data/math_topics.json`)**：
   - 覆盖中考数与代数、图形与几何核心考点。
   - 包含考点名称、前置依赖关系（Prerequisites）。

2. **教科书与强化资料元数据 (`data/textbooks_catalog.json`)**：
   - 各年级（初一、初二、初三）教科书章节与专题练习卷。

3. **考点知识引用与做题库 (`data/knowledge_details.json`)**：
   - 每一考点必须包含：课本原句定义引用、核心解题公式/定理、易错避坑预警、针对性即点即判练习题与详尽推导过程。

---

## 二、数据合法性校验

在提交更新前，请确保 JSON 格式合法且无重复 ID：

```bash
python3 -m json.tool data/math_topics.json > /dev/null
python3 -m json.tool data/knowledge_details.json > /dev/null
python3 -m json.tool data/textbooks_catalog.json > /dev/null
```

# 中英双语摘要规范 / CN-EN Abstract Specification

> 核心参考资料：本文件定义中英文摘要的结构规范、对称性审查标准和常见错误。

---

## 一、中文摘要规范（基于 GB 7713-87）

### 1.1 四要素结构

中文摘要必须包含以下四个核心要素，缺一不可：

| 要素 | 定义 | 应回答的问题 | 占摘要比重 |
|------|------|-------------|-----------|
| **目的** | 研究背景、问题陈述、研究目标 | 为什么要做这个研究？要解决什么问题？ | ~10-15% |
| **方法** | 研究设计、数据来源、分析方法 | 怎么做的？用了什么方法？ | ~20-25% |
| **结果** | 主要发现、数据支持、统计结果 | 发现了什么？数据是什么？ | ~35-45% |
| **结论** | 研究发现的意义、理论贡献、实践启示 | 这意味着什么？有什么价值？ | ~15-20% |

### 1.2 常见中文摘要错误

#### 错误类型1：三段式不分要素
```
❌ 不合格示例：
"随着制造业数字化转型的推进，封头制造企业面临信息化水平低的问题。本文
提出了一个面向封头制造的全流程数字化溯源系统。该系统实现了生产过程数据
的全程记录与追溯，对提升产品质量具有重要价值。"

问题分析：
- 缺少"方法"要素：没有说明系统架构、技术方案、开发方法
- 缺少"结果"要素：没有具体数据支撑效果声明
- "结论"过于笼统，缺少量化依据
```

```
✓ 合格示例：
"【目的】封头制造行业存在生产过程数据分散、质量追溯困难的问题，
亟需一套完整的数字化溯源方案。【方法】基于 MES（制造执行系统）架构，
设计了覆盖原材料入库、成型、热处理、无损检测、成品出库五大环节的
全流程数字化溯源系统。系统采用二维码赋码技术实现物料标识，通过
OPC-UA协议与PLC设备通信采集实时工艺参数，数据存储采用时序数据库
InfluxDB。【结果】在河南某封头制造企业部署应用6个月后，质量追溯
响应时间从平均4.2小时缩短至3.2分钟，产品一次合格率从87.3%提升至
93.8%，生产异常定位效率提升76%。【结论】该数字化溯源系统显著提升
了封头制造企业的质量管控能力，为离散制造行业的数字化转型提供了可
参考的方案。"
```

#### 错误类型2：结果数据缺失
```
❌ 不合格："实验结果表明该方法效果显著。"
   → 缺少具体数字：什么指标？从多少提升到多少？显著性水平？

✓ 合格："实验结果表明，改进算法在CIFAR-10数据集上准确率达到94.7%，
   较基准模型ResNet-50提升2.3个百分点（p<0.01）。"
```

#### 错误类型3：评价性语言过多
```
❌ 不合格："本文进行了深入的研究""做出了重要贡献""具有重大意义"
   → 避免主观评价词："深入""重要""重大""显著"（除非有数据支撑）

✓ 合格："本研究通过对比实验验证了..." / "结果表明，该方法使...提升了X%"
   → 客观陈述事实和数据
```

---

## 二、英文 Abstract 规范（IMRAD-based）

### 2.1 五要素结构

英文摘要建议包含五个要素（比中文摘要多一个 Background）：

| Element | Definition | Questions Answered | Proportion |
|---------|-----------|-------------------|------------|
| **Background** | Context and problem gap | What is known? What gap exists? | ~10-15% |
| **Aims/Objectives** | Research purpose and questions | What did this study aim to achieve? | ~10% |
| **Methods** | Design, participants, procedures, analysis | How was the study conducted? | ~20-25% |
| **Results** | Key findings with data | What was found? (with numbers) | ~35-45% |
| **Conclusions** | Interpretation and implications | What do the findings mean? | ~15-20% |

### 2.2 虚构示例

```
This paper addresses the challenge of fragmented production data and
inefficient quality traceability in the head (dished end) manufacturing
industry. We designed and implemented a full-process digital traceability
system based on the MES (Manufacturing Execution System) architecture,
covering five stages: raw material receiving, forming, heat treatment,
non-destructive testing (NDT), and finished product delivery. The system
employs QR-code-based material identification, OPC-UA protocol for
real-time process parameter collection from PLC equipment, and InfluxDB
time-series database for data storage. Deployed at a head manufacturing
enterprise in Henan Province, China, for a six-month trial, the system
reduced quality traceability response time from an average of 4.2 hours
to 3.2 minutes, improved first-pass yield from 87.3% to 93.8%, and
increased production anomaly location efficiency by 76%. These results
demonstrate that the proposed digital traceability system significantly
enhances quality control capabilities in head manufacturing and provides
a replicable approach for digital transformation in discrete manufacturing
industries.
```

---

## 三、中英文摘要对称性审查清单

### 3.1 五项审查指标

| # | 审查项 | 检查方法 | 标准 |
|---|--------|---------|------|
| 1 | **要素对应** | 中文四要素是否在英文中均有体现？英文Background是否在中文译稿中表达？ | 核心要素无遗漏 |
| 2 | **数据一致** | 所有数字（样本量、百分比、统计值）在两种语言中是否一致？ | 完全相同 |
| 3 | **关键词一致** | 中英文关键词在概念上是否一一对应（非逐字翻译）？ | 概念对应，数量一致 |
| 4 | **时态一致** | 英文时态是否规范（Methods/Results→过去时，Conclusions→现在时，Background/Aims→现在时/现在完成时）？ | 时态规范 |
| 5 | **长度比例** | 英文摘要字符数 ÷ 中文摘要字符数 ≤ 1.5:1 | 不超过1.5倍 |

### 3.2 对称性评分

```
5项全通过   ★★★★★ 摘要中英对称性优秀
4项通过     ★★★★☆ 摘要中英对称性良好（有1项需修改）
3项通过     ★★★☆☆ 摘要中英对称性一般（有2项需修改）
≤2项通过    ★★☆☆☆ 摘要中英对称性不足，建议全面修订
```

---

## 四、常见不对称错误

### 4.1 中文有数据，英文没数据

```
中文："实验结果表明准确率从82.1%提升至91.3%"
英文："Experimental results show significant improvement in accuracy."
      → 数据丢失！修正：
      "Experimental results show accuracy improved from 82.1% to 91.3%."
```

### 4.2 英文关键词 ≠ 中文关键词翻译

```
中文关键词：数字化溯源；封头制造；MES系统；质量管控
英文关键词：digital traceability; head manufacturing; MES system; quality control
                     ✓               ✓              ✓              ✓

常见错误：
中文关键词：智能制造；数字化转型
英文关键词：smart manufacturing; Industry 4.0
                     ✓                   ✗（概念不对应！）
```

### 4.3 时态不匹配

```
中文："本文提出了一种新方法"（"提出"暗示动作已完成）
英文："This paper proposes a novel method"
      ✗ 应使用过去时："This paper proposed..." 或现在完成时："This paper has proposed..."
      （注：不同学科惯例不同，CS常用现在时，工程常用过去时）
```

### 4.4 中文有方法描述，英文方法被压缩

```
中文："采用基于有限元分析的数值模拟方法，结合ABAQUS软件建立三维模型"
英文："Using FEM method" 
      → 关键信息被过度压缩
```

---

## 五、中文摘要特有错误

### 5.1 三段式结构，无要素标识

部分中文学术期刊要求使用"【目的】【方法】【结果】【结论】"结构化标识，非结构化摘要也需要各要素内在完整。

### 5.2 背景性内容过多，挤占结果空间

```
❌ 不合格：摘要前60%讲行业背景，只有最后一句提到"研究取得了良好效果"
✓ 合格：背景/目的占15%，方法占25%，结果占45%，结论占15%
```

### 5.3 引用参考文献

摘要应具有独立性和自含性，不应出现引用（如"[1]""（张三，2020）"）。

### 5.4 缩写未在首次出现时展开

```
❌ 不合格："采用CNN和LSTM构建混合模型"
✓ 合格："采用卷积神经网络（Convolutional Neural Network，CNN）
   和长短期记忆网络（Long Short-Term Memory，LSTM）构建混合模型"
```

---

## 六、快速诊断流程

```
1. 中文摘要是否包含四大要素（目的/方法/结果/结论）？
   └─ 缺失 → 补充缺失要素

2. 中文摘要是否有具体数据？
   └─ 无数据 → 补充量化结果

3. 英文摘要是否遗漏了中文摘要中的任何数据？
   └─ 是 → 补充英文数据

4. 中英文关键词是否概念对应？
   └─ 否 → 调整关键词

5. 英文时态是否规范？
   └─ 否 → 修正时态

6. 中英文长度比例是否合理？
   └─ 否 → 调整长度
```

---

*本文件所有示例均使用虚构论文标题和摘要内容。*

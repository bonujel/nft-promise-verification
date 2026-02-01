# 🔍 TRUST NO ONE 画饼粉碎机
![Uploading image.png…]()

> 揭露NFT项目的"画饼"行为，量化项目可信度

[![Python 3.11](https://img.shields.io/badge/Python-3.11-blue.svg)]()
[![License](https://img.shields.io/badge/License-MIT-green.svg)]()
[![Web3](https://img.shields.io/badge/Web3-Ethereum-purple.svg)]()

## 🎯 一句话介绍

**自动化审计工具**：分析NFT项目方在Twitter/官网的承诺，对比链上实际行为，生成"画饼指数"评分（0-100分）。

## ✨ 为什么需要这个工具？

在NFT市场中，项目方常常"画饼"而不兑现承诺。本项目帮你：
- 🔍 **自动收集**项目方的公开承诺
- ⛓️ **链上验证**承诺是否真正兑现  
- 📊 **量化评估**项目可信度
- 🚨 **预警风险**避免投资损失

## 🏆 核心特性

### 🔍 智能承诺提取
- 自动抓取Twitter、官网内容
- 用AI识别"承诺"类信息
- 结构化存储便于跟踪

### 📊 五维审计模型
1. **诚信度** (30%) - 承诺兑现率
2. **公平性** (20%) - 代币分布公平性
3. **开发力** (20%) - 代码更新频率
4. **财务健康** (15%) - 资金流向分析
5. **社区活力** (15%) - 社区互动质量

### ⛓️ 链上验证
- 实时查询EVM链上数据
- 验证承诺执行情况
- 历史行为追踪分析

### 🔒 隐私保护
- 通过ERC-7962实现链上隐私存储
- 保护用户查询隐私
- 零知识证明支持（规划中）

## 🚀 5分钟快速上手

```bash
# 1. 克隆项目
git clone https://github.com/your-org/hackason-project.git
cd hackason-project/nft-promise-verification

# 2. 安装依赖
conda create -n promise-detector python=3.11
conda activate promise-detector
pip install -r requirements.txt

# 3. 配置API密钥
cp config/.env.example config/.env
# 编辑.env文件，填入你的API密钥

# 4. 运行示例
python main.py collect --name "Bored Ape Yacht Club" --twitter "@BoredApeYC"
```
## 📈 输出示例
```
text
项目: Bored Ape Yacht Club
画饼指数: 72/100 🔥

📊 五维评分:
├─ 诚信审计: 65/100 (承诺兑现率65%)
├─ 公平性审计: 80/100 (代币分布较公平)
├─ 开发力审计: 70/100 (开发活跃度中等)
├─ 财务稳定性: 75/100 (资金状况良好)
└─ 社区动能: 70/100 (社区互动正常)

⚠️ 风险提示:
• 有3个未兑现承诺
• Top 5持有者控制35%代币
• 近30天无代码更新
```
## 🛠️ 技术栈

| 组件 | 技术选型 | 用途 |
|------|----------|------|
| **AI框架** | SpoonOS 0.3.6 | Agent编排与管理 |
| **LLM** | Claude 3.5 Sonnet | 语义理解与承诺提取 |
| **区块链** | Web3.py + DDC-SDK | 链上数据交互 |
| **分析** | 自定义评分算法 | 五维审计模型 |
## 📁 项目结构
```
text
nft-promise-verification/
├── agent.py              # 核心Agent
├── main.py               # CLI入口
├── scoring/              # 五维评分算法
├── tools/                # 数据收集工具
├── verification/         # 链上验证逻辑
├── privacy/              # 隐私存储模块
└── config/               # 配置文件
```
## 🤔 使用场景
```
🎨 普通投资者

# 检查你关注的NFT项目
python main.py verify --project "CoolCatsNFT"

📊 数据分析师

# 批量分析Top 100 NFT项目
python main.py batch-analyze --limit 100

🔬 研究机构

# 导出详细审计报告
python main.py report --format pdf --detailed
```
## 📞 联系我们
遇到问题或有建议？

📧 提交Issue: 项目Issue页面

💬 讨论区: 项目Wiki中的讨论页面

🐛 Bug反馈: 提供复现步骤和截图

## 🙌 致谢与引用
基于以下技术构建：

SpoonOS - AI Agent框架

BSN DDC - 区块链隐私存储

Anthropic Claude - AI能力支持

## 📄 许可证
MIT License 


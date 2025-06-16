# 📰 langchain-news-extractor

基于 LangChain 和大语言模型的新闻摘要工具，能够从新闻内容中自动提取 5W 信息（Who、What、When、Where、Why），适用于快速信息抓取、内容分类与知识分析。

---

## 🚀 功能亮点

- 🧠 基于 LangChain 的 LLM 架构
- 🔎 自动提取 5W 要素：谁、做了什么、何时、何地、为何
- 🌐 多语言支持（根据模型能力）
- 🛠 可集成到新闻平台、数据分析流程中

---

## 🔧 安装与依赖

你可以通过以下方式安装本项目依赖：

```bash
git clone https://github.com/yourname/langchain-news-extractor.git
cd langchain-news-extractor
pip install -r requirements.txt
或手动安装主要依赖：
pip install langchain openai pandas

## 使用方法
from news_extractor import extract_5w

text = """
2025年，OpenAI 宣布推出新的 GPT 模型，引起全球 AI 研究者关注。
"""

result = extract_5w(text)
print(result)

##输出示例：
{
  "Who": "OpenAI",
  "What": "推出新的 GPT 模型",
  "When": "2025年",
  "Where": "全球",
  "Why": "引起 AI 研究者关注"
}



## 📂 项目结构
📦 langchain-news-extractor
 ┣ 📜 news_extractor.py         # 主功能模块
 ┣ 📜 prompts.py                # 自定义提示词模板
 ┣ 📜 utils.py                  # 工具函数模块
 ┣ 📄 requirements.txt          # 项目依赖
 ┣ 📄 LICENSE
 ┗ 📄 README.md


## 📄 License
本项目采用 MIT License 开源，欢迎自由使用、修改、再发布。

## 👩‍💻 作者
由 @woshixiyangyang开发与维护。
欢迎提交 Issue 或 PR 改进项目 😊

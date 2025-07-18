---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---
{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}

<span class='anchor' id='about-me'></span>

大家好！我是**于立伟**，目前是本科四年级学生，就读于[新疆大学软件学院](https://ss.xju.edu.cn/)软件工程专业。

我对人工智能充满热情，自入学以来，积极参与各类科研项目和学术竞赛，曾获得中国近现代感恩科学家奖学金（全学院仅1个名额）、ACM-ICPC银牌等多项校内外奖项。在科研方面，我参与并主导了多个项目，包括但不限于**时间序列**、**大语言模型**等领域。

# 🎓 Education Background

- **排名：** GPA排名：**1/819 (0.12%)**、综测排名：**1/819 (0.12%)**  
- **成绩均分：** GPA：4.3/5.0、加权平均分：93/100  
- **语言能力：** 已通过 CET4 和 CET6，《计算机专业英语》成绩为94分，曾独立撰写并投稿全英文学术论文  
- **核心课程：** 高等数学 (100)、线性代数 (94)、概率论与数理统计 (95)、离散数学 (98)、程序设计基础 (95)、Python (97)、Java (96)、Web程序设计 (92)、数据结构与算法分析 (96)、人工智能 (99)、软件工程 (95)、ICS (91)、操作系统 (94)、数据库 (93)、计算机网络 (93)、网络与信息安全 (98)  
- **编程能力：** 熟练掌握 C++ 和 Python，熟悉算法与数据结构，代码能力强，曾获 ACM-ICPC 银牌；熟练掌握 PyTorch、Numpy、Pandas，熟悉各类深度学习模型及其编程实现；长期担任数学建模编程手，曾获“高教社杯”全国大学生数学建模竞赛省级特等奖  
- **开发工具：** VS Code, PyCharm, Jupyter Notebook, LaTeX (Overleaf), Git  
- **在校荣誉：** 曾获第六届中国近现代感恩科学家奖学金（全学院仅1个名额）、新疆大学三好学生

# 🔥 News

# 📈 Research Experience-Time Series

## **💡💡💡 TempoStackNet - A Novel Cryptocurrency Price Prediction Framework**  

- **时间：** 2023.3 - 2024.3  
- **领域：** **时间序列预测**，**AI for Finance**  
- **角色：** 第一作者  
- **研究背景：**  
  1. 相较于传统投资市场，加密货币市场由于其动态性和高波动性，使得相关的价格预测方法效率较低，现有方法无法应对市场的投机性和复杂性。
  2. 当前亟需一种高效的价格预测方法，以更准确地预测加密货币的价格趋势。
- **我们的方法：**  
  1. **引入TempoStackNet框架：** 我们设计了一种新颖的加密货币价格预测框架TempoStackNet，结合了叠加集成学习和跨时间窗口策略，利用时序注意力机制，整合192/96/48个时间窗口间隔的历史数据，有效提高了多步价格预测的准确性。
  2. **多步价格预测策略：** 通过高精度预测未来32天内的加密货币价格趋势，显著提升了预测模型的泛化性和鲁棒性。
- **项目成果：**  
  * 在Global Technology and Cryptocurrency Volatility、S&P 500指数等多个数据集上的实验结果显示，TempoStackNet在准确性、泛化性和鲁棒性方面优于现有的SOTA方法。
  * 相关论文已投稿至中科院2区期刊。

## **💡 Kaggle: Optiver - Trading at the Close** <sub> &nbsp;&nbsp;[[比赛介绍]](https://www.kaggle.com/competitions/optiver-trading-at-the-close) | [[Leaderboard]](https://www.kaggle.com/competitions/optiver-trading-at-the-close/leaderboard)</sub>  

- **时间：** 2023.11 - 2024.1  
- **领域：** **时间序列预测**，**AI for Trading**  
- **角色：** 团队(主力队员)  
- **研究背景：**  
  1. 股票交易以高波动性和快速的价格变化为特征，特别是在纳斯达克交易所，每个交易日都以收盘交叉拍卖结束。该过程确定了证券的官方收盘价格，是市场参与者评估市场表现的关键指标。
  2. 在交易的最后十分钟，做市商会将传统订单簿数据与拍卖簿数据相结合，提供最佳的价格参考。在这次比赛中，挑战在于开发一个模型，利用订单簿和收盘拍卖数据来预测数百支纳斯达克股票的收盘价走势。
- **我们的方法：**  
  1. **特征工程：** 进行特征转换，处理时序数据（如时间特征提取、滚动窗口统计等），并进行特征选择。
  2. **回归算法测试：** 尝试多种回归算法（如CatBoost、XGB、LGBM、神经网络等），最终确定LGBM与神经网络为最佳模型。
  3. **超参数优化：** 使用Grid Search和Randomized Search方法分别进行超参数优化，综合考虑后选取合适的超参数。
- **项目成果：**  
  * 取得了5.4724的最终分数，获得铜牌(Top 6%)。

# 🧩 Research Experience-Large Language Models

## **💡 Kaggle: LMSYS-Chatbot Arena Human Preference Predictions** <sub> &nbsp;&nbsp;[[比赛介绍]](https://www.kaggle.com/competitions/lmsys-chatbot-arena) | [[Leaderboard]](https://www.kaggle.com/competitions/lmsys-chatbot-arena/leaderboard)</sub>  

- **时间：** 2024.5 - 2024.8  
- **领域：** **大语言模型**，**LLM问答**  
- **角色：** 团队(主力成员)  
- **研究背景：**  
  1. 本次竞赛的挑战是预测用户在两个人工智能对话系统（LLM）之间的对决中更偏爱哪个回答。参赛者将获得一组来自Chatbot Arena的对话数据，这些对话是由不同的LLM生成的。
  2. 通过开发一个获胜的机器学习模型，目标是改进聊天机器人与人类的互动方式，使其更符合人类的偏好。
- **我们的方法：**  
  1. **模型选择与测试：** 最初测试了Deberta base、Deberta v2、Xlarge、Deberta v3 large等“小语言”模型，效果不佳。参考公开方案和讨论区观点后，转向“大语言”模型测试。
  2. **大语言模型尝试：** 尝试了Gemma2 9b，Gemma2 27b，Llama3 8b模型。Gemma2 27b在本地测试表现最佳，但因超出比赛环境GPU显存限制，最终选择Gemma2 9b和Llama3 8b模型。
  3. **微调与集成：** 使用QLoRA对两个模型进行微调，尝试两种方案：[对Gemma2 9b设置较高的Rank（32,64）微调作为单模型]和[对Gemma2 9b和Llama3 8b均设置较低的Rank（16）进行微调，最后集成]，最终选择了集成方案。
- **项目成果：**  
  * 取得了0.98739的最终分数，获得银牌(Top 2%)。

## **💡 长安陌上 - 基于Qwen大模型的语料库问答平台** <sub> &nbsp;&nbsp;[[演示文档]](https://btlazzq.github.io/docs/changanmoshangPPT.pdf)</sub>

- **时间：** 2023.6 - 2024.2  
- **领域：** **大语言模型微调**，**RAG**  
- **角色：** 团队(主力成员)  
- **研究背景：**  
  1. 大语言模型（LLM）具备处理复杂任务的能力和强大的语言理解能力，可以为文旅行业提供支持和赋能。
  2. 然而，通用型LLM在特定领域缺乏足够的领域专业知识，且现有LLM系统在生成输出时存在一定的幻觉问题，导致输出结果可能不符合用户的预期。
  3. 因此，亟需开发一个基于LLM的高准确度文旅语料库问答平台，以提供精准的文旅信息服务。
- **我们的方法：**  
  1. **数据获取与模型微调：** 使用爬虫技术获取西安文旅数据，构建专用语料库，并对Qwen大模型进行LoRA微调，提升模型在特定领域的知识深度。
  2. **知识整合与交互平台：** 通过RAG技术整合外部知识库，使用Gradio构建交互式界面，为用户提供智能化、准确的文旅信息查询和推荐服务。
- **项目成果：**  
  * 作为主力队员参加第十五届全国大学生服务外包创新创业大赛，并在省赛中荣获三等奖。

# 📝 Research Experience-Other

## **💡《肃巡直通车》系统开发 - 甘肃省酒泉市巡察办** <sub> &nbsp;&nbsp;[[表彰文件]](https://btlazzq.github.io/docs/suxunzhitongcheZHENGMING.pdf)</sub>

- **时间：** 2024.4 - 2024.8  
- **领域：** **前后端开发**  
- **角色：** 实习生/骨干成员  
- **开发背景：**  
  1. 甘肃省酒泉市巡察办主导的《肃巡直通车》微信小程序旨在为巡察组提供一个更便捷的平台，用于收集数据和调查信息，同时让群众能够更直接地向巡察组反馈问题和意见，从而提高巡察工作的效率和质量。
- **我的贡献：**  
  1. **前后端开发工作：** 作为主要开发人员，负责微信小程序和后端数据管理平台的前后端开发，包括数据收集、反馈机制、数据管理和安全保障等功能。巡察组成员可以记录巡察过程中的问题和调查结果，群众可以反馈问题或提出建议，小程序还提供数据存储、分类、分析和报告生成功能，并设置安全措施确保数据安全性和隐私性。
  2. **智能数据分析：** 应用大模型技术进行巡察数据的智能分析，实现高效的数据处理和报告生成，设计并实现的算法显著提升了数据分析的精准度和处理速度，确保了巡察工作的及时性和有效性。
  3. **数字化互动平台：** 项目充分利用数字经济的概念，通过微信小程序实现群众与巡察组之间的高效互动与信息交流，提升了巡察工作的透明度和参与度，强化了政府与群众之间的信任关系。
- **项目成果：**  
  * 获中共酒泉市肃州区委巡察工作领导小组表彰: “王菡悦在项目开发中展现了卓越的专业素养和技术能力。通过创新的解决方案推动了政府工作透明度和群众参与度的提升。她的努力和贡献不仅得到了项目各方的高度认可，更为未来的数字化政务工作树立了标杆。”

# 🏆 Competition Awards

- **Kaggle: Chatbot Arena Human Preference Predictions：银牌** *国家级* 2024 &nbsp;&nbsp;[[Leaderboard]](https://www.kaggle.com/competitions/lmsys-chatbot-arena/leaderboard)  
- **Kaggle: LLM-Detect AI Generated Text：铜牌** *国家级* 2024 &nbsp;&nbsp;[[Leaderboard]](https://www.kaggle.com/competitions/llm-detect-ai-generated-text/leaderboard)  
- **Kaggle: Optiver - Trading at the Close：铜牌** *国家级* 2024 &nbsp;&nbsp;[[Leaderboard]](https://www.kaggle.com/competitions/optiver-trading-at-the-close/leaderboard)  
- **中国国际“互联网+”大学生创新创业大赛(全国总决赛)：银奖** *国家级* 2023 &nbsp;&nbsp;[[证明]](https://btlazzq.github.io/docs/AWARDhulianwang+guo.pdf)  
- **全国大学生软件创新大赛(全国总决赛)：三等奖** *国家级* 2024 &nbsp;&nbsp;[[证明]](https://btlazzq.github.io/docs/AWARDruanchuang_guo.pdf)  
- **全国大学生数学建模竞赛：特等奖** *省部级* 2023 &nbsp;&nbsp;[[证明]](https://btlazzq.github.io/docs/AWARDshumo.pdf)  
- **中国国际“互联网+”大学生创新创业大赛(省级赛)：金奖** *省部级* 2023 &nbsp;&nbsp;[[证明]](https://btlazzq.github.io/docs/AWARDhulianwang+sheng.pdf)  
- **全国大学生软件创新大赛(西北赛区)：一等奖** *省部级* 2024 &nbsp;&nbsp;[[证明]](https://btlazzq.github.io/docs/AWARDruanchuang_sheng.pdf)  
- **国际大学生程序设计竞赛(ACM-ICPC)：银牌** *省部级* 2023 &nbsp;&nbsp;[[证明]](https://btlazzq.github.io/docs/AWARDicpc.pdf)  
- **中国大学生服务外包创新创业大赛(西部区域赛)：三等奖** *省部级* 2024 &nbsp;&nbsp;[[证明]](https://btlazzq.github.io/docs/AWARDfuchuang.pdf)  
- **中国大学生计算机设计大赛(省级赛)：三等奖** *省部级* 2024 &nbsp;&nbsp;[[证明]](https://btlazzq.github.io/docs/AWARDjishe1.pdf)  
- **中国大学生计算机设计大赛(省级赛)：三等奖** *省部级* 2024 &nbsp;&nbsp;[[证明]](https://btlazzq.github.io/docs/AWARDjishe2.pdf)   

# 🥇 Scholarships and Honors

- *2021-2022* **中国近现代感恩科学家奖学金** (全学院仅1个名额) *新疆大学*  
- *2021-2022* **新疆大学三好学生** *新疆大学* 

# 📖 Educations

- **2021.9 - 至今**，本科生，新疆大学软件学院，专业：软件工程  
- **2022.9 - 2023.9**，本科生，中南大学计算机学院（联合培养），专业：软件工程  

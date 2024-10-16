# LLM-Visualization-Paper-List

- Content
  - [0. Why am I curating this repository?](#0-why-am-i-curating-this-repository)
  - [1. Chart Captioning](#1-chart-captioning)
  - [2. Chart Question Answering](#2-chart-question-answering)
    - [2.0 Data, Model](#20-data-model)
    - [2.1 Benchmark](#21-benchmark)
  - [3. Chart Reverse Engineering](#3-chart-reverse-engineering)
  - [4. Natural Language to Visualization](#4-natural-language-to-visualization)
  - [5. Visualization Design](#5-visualization-design)
    - [5.0 Color](#50-color)
    - [5.1 Design Preferences](#51-design-preferences)
  - [6. Visualization Agents & Automatic Judge](#6-visualization-agents--automatic-judge)
  - [7. Empirical Study on LLM's Chart Understanding](#7-empirical-study-on-llms-chart-understanding)
  - [8. Generic Multimodal Large Language Model](#8-generic-multimodal-large-language-model)
  - [9. Related Survey Papers](#9-related-survey-papers)

## 0. Why am I curating this repository?
- I've found that the **Vis**x**LLM** paper-list repositories are updated infrequently (they're more likely created for a survey paper and then abandoned). I will gradually enrich this repository and keep it updated.
- Feel free to open an issue or a pull request to add a new paper you appreciate.
- Papers under the same category are recorded in reverse chronological order.
  
## 1. Chart Captioning

**Natural Language Dataset Generation Framework for Visualizations Powered by Large Language Models**  
Hyung-Kwon Ko, Hyeon Jeon, Gwanmo Park, Dae Hyun Kim, Nam Wook Kim, Juho Kim, Jinwook Seo  
[CHI 2024](https://arxiv.org/abs/2309.10245) • [Code](https://github.com/hyungkwonko/chart-llm)

**VisText: A Benchmark for Semantically Rich Chart Captioning**  
Benny J. Tang, Angie Boggust, Arvind Satyanarayan  
[ACL 2023 Outstanding paper](https://aclanthology.org/2023.acl-long.401.pdf) • [Code](https://github.com/mitvis/vistext)

--- Pre-LLM ---  
**Chart-to-Text: A Large-Scale Benchmark for Chart Summarization**  
Shankar Kantharaj, Rixie Tiffany Leong, Xiang Lin, Ahmed Masry, Megh Thakkar, Enamul Hoque, Shafiq Joty  
[ACL 2022](https://aclanthology.org/2022.acl-long.277.pdf) • [Code](https://github.com/vis-nlp/Chart-to-text)


## 2. Chart Question Answering


### 2.0 Data, Model
**SynChart: Synthesizing Charts from Language Models**  
Mengchen Liu, Qixiu Li, Dongdong Chen, Dong Chen, Jianmin Bao, Yunsheng Li  
[arXiv](https://arxiv.org/abs/2409.16517)

**ChartMoE: Mixture of Expert Connector for Advanced Chart Understanding**   
Zhengzhuo Xu, Bowen Qu, Yiyan Qi, Sinan Du, Chengjin Xu, Chun Yuan, Jian Guo   
[arXiv, 5 Sep 2024](https://arxiv.org/abs/2409.03277) • [Code](https://chartmoe.github.io/)

**TinyChart: Efficient Chart Understanding with Visual Token Merging and Program-of-Thoughts Learning**  
Liang Zhang*, Anwen Hu*, Haiyang Xu, Ming Yan, Yichen Xu, Qin Jin†, Ji Zhang, Fei Huang  
[arXiv, 25 Apr 2024](https://arxiv.org/pdf/2404.16635) • [Code](https://github.com/X-PLUG/mPLUG-DocOwl/tree/main/TinyChart)

**OneChart: Purify the Chart Structural Extraction via One Auxiliary Token**  
Jinyue Chen*, Lingyu Kong*, Haoran Wei, Chenglong Liu, Zheng Ge, Liang Zhao, Jianjian Sun, Chunrui Han, Xiangyu Zhang  
[ACM MM 2024 (Oral)](https://arxiv.org/pdf/2404.09987) • [Homepage](https://onechartt.github.io/)

**Advancing Multimodal Large Language Models in Chart Question Answering with Visualization-Referenced Instruction Tuning**  
Xingchen Zeng, Haichuan Lin, Yilin Ye, Wei Zeng  
[VIS 2024](https://arxiv.org/abs/2407.20174) • [Code](https://github.com/zengxingchen/ChartQA-MLLM)

**Representing Charts as Text for Language Models: An In-Depth Study of Question Answering for Bar Charts**  
Victor Soares Bursztyn, Jane Hoffswell, Eunyee Koh, Shunan Guo  
[VIS 2024 Short Paper](https://ieeevis.b-cdn.net/vis_2024/pdfs/v-short-1276.pdf)

**ChartInstruct: Instruction Tuning for Chart Comprehension and Reasoning**  
Ahmed Masry, Mehrad Shahmohammadi, Md Rizwan Parvez, Enamul Hoque, Shafiq Joty  
[Findings of ACL 2024](https://github.com/vis-nlp/ChartInstruct) • [Code](https://github.com/vis-nlp/ChartInstruct)  

**ChartAssistant: A Universal Chart Multimodal Language Model via Chart-to-Table Pre-training and Multitask Instruction Tuning**  
Fanqing Meng, Wenqi Shao, Quanfeng Lu, Peng Gao, Kaipeng Zhang, Yu Qiao, Ping Luo  
[Findings of ACL 2024](https://aclanthology.org/2022.findings-acl.177.pdf) • [Code](https://github.com/OpenGVLab/ChartAst)

**MMC: Advancing Multimodal Chart Understanding with Large-scale Instruction Tuning**  
Fuxiao Liu, Xiaoyang Wang, Wenlin Yao, Jianshu Chen, Kaiqiang Song, Sangwoo Cho, Yaser Yacoob, Dong Yu  
[NAACL 2024](https://aclanthology.org/2024.naacl-long.70.pdf) • [Code](https://github.com/FuxiaoLiu/MMC)

**Synthesize Step-by-Step: Tools Templates and LLMs as Data Generators for Reasoning-Based Chart VQA**  
Zhuowan Li, Bhavan Jasani, Peng Tang, Shabnam Ghadar  
[CVPR 2024](https://openaccess.thecvf.com/content/CVPR2024/papers/Li_Synthesize_Step-by-Step_Tools_Templates_and_LLMs_as_Data_Generators_for_CVPR_2024_paper.pdf)

**Chartllama: A multimodal llm for chart understanding and generation**  
Fanqing Meng, Wenqi Shao, Quanfeng Lu, Peng Gao, Kaipeng Zhang, Yu Qiao, Ping Luo  
[arXiv, 27 Nov 2023](https://arxiv.org/pdf/2311.16483) • [Homepage](https://tingxueronghua.github.io/ChartLlama/)

--- Pre-LLM --- 

**UniChart: A Universal Vision-language Pretrained Model for Chart Comprehension and Reasoning**  
Ahmed Masry∗, Parsa Kavehzadeh∗, Xuan Long Do, Enamul Hoque, Shafiq Joty  
[EMNLP 2023](https://aclanthology.org/2023.emnlp-main.906.pdf) • [Code](https://github.com/vis-nlp/UniChart)

**Deplot: One-shot visual language reasoning by plot-to-table translation**  
Fangyu Liu, Julian Martin Eisenschlos, Francesco Piccinno, Syrine Krichene, Chenxi Pang, Kenton Lee, Mandar Joshi, Wenhu Chen, Nigel Collier, Yasemin Altun  
[Findings of ACL 2023](https://aclanthology.org/2023.findings-acl.660.pdf) • [Code](https://github.com/google-research/google-research/tree/master/deplot)

**MatCha: Enhancing Visual Language Pretraining with Math Reasoning and Chart Derendering**  
Fangyu Liu, Francesco Piccinno, Syrine Krichene, Chenxi Pang, Kenton Lee, Mandar Joshi, Yasemin Altun, Nigel Collier, Julian Martin Eisenschlos  
[ACL 2023](https://aclanthology.org/2023.acl-long.714.pdf) • [Code](https://github.com/google-research/google-research/tree/master/deplot)

**Dvqa: Understanding data visualizations via question answering**  
Kushal Kafle, Brian Price, Scott Cohen, Christopher Kanan  
[CVPR 2018](https://openaccess.thecvf.com/content_cvpr_2018/papers/Kafle_DVQA_Understanding_Data_CVPR_2018_paper.pdf) • [Code](https://github.com/kushalkafle/DVQA_dataset)
### 2.1 Benchmark
**CharXiv: Charting Gaps in Realistic Chart Understanding in Multimodal LLMs**  
 Zirui Wang, Mengzhou Xia, Luxi He, Howard Chen, Yitao Liu, Richard Zhu, Kaiqu Liang, Xindi Wu, Haotian Liu, Sadhika Malladi, Alexis Chevalier, Sanjeev Arora, Danqi Chen  
[NeurIPS 2024 Benchmark](http://arxiv.org/abs/2406.18521) • [Homepage](https://charxiv.github.io/)

**Chartx & chartvlm: A versatile benchmark and foundation model for complicated chart reasoning**  
Renqiu Xia, Bo Zhang, Hancheng Ye, Xiangchao Yan, Qi Liu, Hongbin Zhou, Zijun Chen, Min Dou, Botian Shi, Junchi Yan, Yu Qiao  
[arXiv, 19 Feb 2024](https://arxiv.org/pdf/2402.12185)


**ChartBench: A Benchmark for Complex Visual Reasoning in Charts**   
Zhengzhuo Xu*, Sinan Du*, Yiyan Qi, Chengjin Xu, Chun Yuan†, Jian Guo  
 [arXiv 26 Dec 2023](https://arxiv.org/pdf/2312.15915) • [Homepage](https://chartbench.github.io/)

--- Pre-LLM ---  
**ChartQA: A Benchmark for Question Answering about Charts with Visual and Logical Reasoning**  
Ahmed Masry, Xuan Long Do, Jia Qing Tan, Shafiq Joty, Enamul Hoque  
[Findings of ACL 2022](https://aclanthology.org/2022.findings-acl.177.pdf) • [Code](https://github.com/vis-nlp/chartqa)


## 3. Chart Reverse Engineering
**ChartMimic: Evaluating LMM’s Cross-Modal Reasoning Capability via Chart-to-Code Generation**  
Chufan Shi and Cheng Yang and Yaxin Liu and Bo Shui and Junjie Wang and Mohan Jing and Linran Xu and Xinyu Zhu and Siheng Li and Yuxiang Zhang and Gongye Liu and Xiaomei Nie and Deng Cai and Yujiu Yang  
[arXiv](https://arxiv.org/pdf/2406.09961) • [Homepage](https://chartmimic.github.io/)

--- Pre-LLM ---  

**Deep colormap extraction from visualizations**  
Lin-Ping Yuan, Wei Zeng, Siwei Fu, Zhiliang Zeng, Haotian Li, Chi-Wing Fu, Huamin Qu  
[TVCG 2022](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9395231)

**Reverse‐engineering visualizations: Recovering visual encodings from chart images**  
Jorge Poco and Jeffrey Heer  
[EuroVis 2017](https://onlinelibrary.wiley.com/doi/pdf/10.1111/cgf.13193)


## 4. Natural Language to Visualization
**VisEval: A benchmark for data visualization in the era of large language models**  
Nan Chen, Yuge Zhang, Jiahang Xu, Kan Ren, and Yuqing Yang  
[VIS 2024](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=10670425)  • [Code](https://github.com/microsoft/VisEval)

**Chartgpt: Leveraging LLMs to generate charts from abstract natural language**  
Yuan Tian, Weiwei Cui, Dazhen Deng, Xinjing Yi, Yurun Yang, Haidong Zhang, Yingcai Wu  
[TVCG 2024](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=10443572)


**LLM4Vis: Explainable Visualization Recommendation using ChatGPT**  
Lei Wang, Songheng Zhang, Yun Wang, Ee-Peng Lim, Yong Wang  
[EMNLP 2023 Industry](https://aclanthology.org/2023.emnlp-industry.64.pdf)  • [Code](https://github.com/demoleiwang/LLM4Vis)  

--- Pre-LLM ---  

**Natural Language to Visualization by Neural Machine Translation**  
Yuyu Luo, Nan Tang, Guoliang Li, Jiawei Tang, Chengliang Chai, Xuedi Qin  
[VIS 2021](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9617561) • [Code](https://github.com/HKUSTDial/ncNet) 

**nvBench: A Large-Scale Synthesized Dataset for Cross-Domain Natural Language to Visualization Task**  
Yuyu Luo, Jiawei Tang, Guoliang Li  
[Workshop on NL VIZ 2021 at IEEE VIS 2021](https://arxiv.org/pdf/2112.12926) • [Code](https://github.com/TsinghuaDatabaseGroup/nvBench)

## 5. Visualization Design
### 5.0 Color
**NL2Color: Refining Color Palettes for Charts with Natural Language**  
Chuhan Shi, Weiwei Cui, Chengzhong Liu, Chengbo Zheng, Haidong Zhang, Qiong Luo, and Xiaojuan Ma  
[VIS 2023](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10292693)

**Large Language Models estimate fine-grained human color-concept associations**  
[arXiv, 4 May 2024](https://arxiv.org/abs/2406.17781)

### 5.1 Design Preferences
**DracoGPT: Extracting Visualization Design Preferences from Large Language Models**  
Huichen Will Wang, Mitchell Gordon, Leilani Battle, and Jeffrey Heer  
[VIS 2024](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10681108)

**Bavisitter: Integrating Design Guidelines into Large Language Models for Visualization Authoring**  
Jiwon Choi, Jaeung Lee, Jaemin Jo  
[VIS 2024 Short Paper](https://idclab.skku.edu/assets/Bavisitter.pdf)

## 6. Visualization Agents & Automatic Judge
**The Visualization JUDGE: Can Multimodal Foundation Models Guide Visualization Design Through Visual Perception?**  
Matthew Berger, Shusen Liu  
[arXiv, 5 Oct 2024](https://arxiv.org/pdf/2410.04280)  

**WaitGPT: Monitoring and Steering Conversational LLM Agent in Data Analysis with On-the-Fly Code Visualization**  
Liwenhan Xie, Chengbo Zheng, Haijun Xia, Huamin Qu, Chen Zhu-Tian   
[UIST 2024](https://arxiv.org/pdf/2408.01703)

**AVA: Towards Autonomous Visualization Agents through Visual Perception‐Driven Decision‐Making**  
Shusen Liu, Haichao Miao, Zhimin Li, Matthew Olson, Valerio Pascucci, P‐T Bremer  
[EuroVis 2024](https://onlinelibrary.wiley.com/doi/pdf/10.1111/cgf.15093)  


## 7. Empirical Study on LLM's Chart Understanding & Chart Generation 
**How Aligned are Human Chart Takeaways and LLM Predictions? A Case Study on Bar Charts with Varying Layouts**  
Huichen Will Wang, Jane Hoffswell, Sao Myat Thazin Thane, Victor S Bursztyn, Cindy Xiong Bearfield  
[VIS 2024](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=10681139)

**An Empirical Evaluation of the GPT-4 Multimodal Language Model on Visualization Literacy Tasks**  
Alexander Bendeck, John Stasko  
[VIS 2024](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=10670574)

**Promises and Pitfalls: Using Large Language Models to Generate Visualization Items**
Yuan Cui, Lily W. Ge, Yiren Ding, Lane Harrison, Fumeng Yang, and Matthew Kay  
[VIS2024](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=10670418)

**How Good (Or Bad) Are LLMs at Detecting Misleading Visualizations?**  
Leo Yu-Ho Lo, Huamin Qu  
[VIS 2024](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=10679256)

**Exploring the Capability of LLMs in Performing Low-Level Visual Analytic Tasks on SVG Data Visualizations**  
Zhongzheng Xu, Emily Wall  
[VIS 2024 Short Paper](https://arxiv.org/pdf/2404.19097)

**Evaluating the Semantic Profiling Abilities of LLMs for Natural Language Utterances in Data Visualization**
Hannah K Bako, Arshnoor Buthani, Xinyi Liu, Kwesi A Cobbina, Zhicheng Liu  
[VIS 2024 Short Paper](https://arxiv.org/pdf/2407.06129) • [Code](https://github.com/hdi-umd/Semantic_Profiling_LLM_Evaluation)

## 8. Generic Multimodal Large Language Model
**MM1.5: Methods, Analysis & Insights from Multimodal LLM Fine-tuning**  
Haotian Zhang, Mingfei Gao, Zhe Gan, Philipp Dufter, Nina Wenzel, Forrest Huang, Dhruti Shah, Xianzhi Du, Bowen Zhang, Yanghao Li, Sam Dodge, Keen You, Zhen Yang, Aleksei Timofeev, Mingze Xu, Hong-You Chen, Jean-Philippe Fauconnier, Zhengfeng Lai, Haoxuan You, Zirui Wang, Afshin Dehghan, Peter Grasch, Yinfei Yang  
[arXiv, 30 Sep 2024](https://arxiv.org/pdf/2409.20566)  
**EAGLE: Exploring The Design Space for Multimodal LLMs with Mixture of Encoders**  
Min Shi*, Fuxiao Liu*, Shihao Wang, Shijia Liao, Subhashree Radhakrishnan, De-An Huang, Hongxu Yin, Karan Sapra, Yaser Yacoob, Humphrey Shi, Bryan Catanzaro, Andrew Tao, Jan Kautz, Zhiding Yu, Guilin Liu  
[arXiv, 28 Aug 2024](https://arxiv.org/abs/2408.15998) • [Code](https://github.com/NVlabs/EAGLE)

**Cambrian-1: A Fully Open, Vision-Centric Exploration of Multimodal LLMs**  
Shengbang Tong*, Ellis Brown*, Penghao Wu*, Sanghyun Woo, Manoj Middepogu, Sai Charitha Akula, Jihan Yang, Shusheng Yang, Adithya Iyer, Xichen Pan, Austin Wang, Rob Fergus, Yann LeCun, Saining Xie  
[arXiv, 24 Jun 2024](https://arxiv.org/abs/2408.15998) • [Code](https://github.com/cambrian-mllm/cambrian)

## 9. Related Survey Papers
**Generative AI for visualization: State of the art and future directions**  
Yilin Ye, Jianing Hao, Yihan Hou, Zhan Wang, Shishi Xiao, Yuyu Luo, Wei Zeng  
[Visual Informatics 2024](https://www.sciencedirect.com/science/article/pii/S2468502X24000160)

**From Detection to Application: Recent Advances in Understanding Scientific Tables and Figures**  
Jiani Huang, Haihua Chen, Fengchang Yu, Wei Lu  
[ACM Computing Surveys 2024](https://dl.acm.org/doi/pdf/10.1145/3657285)

**Leveraging large models for crafting narrative visualization: a survey**  
Yi He, Shixiong Cao, Yang Shi, Qing Chen, Ke Xu, Nan Cao  
[arXiv, 25 Jan 2024](https://arxiv.org/pdf/2401.14010)

**Chart Question Answering: State of the Art and Future Directions**  
Enamul Hoque, Parsa Kavehzadeh, Ahmed Masry  
[EuroVis 2022](https://onlinelibrary.wiley.com/doi/epdf/10.1111/cgf.14573) 


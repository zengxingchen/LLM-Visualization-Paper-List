# Awesome-LLMxVisualization-Paper-List
<p align="center" width="100%">
    <img width="517" alt="Screenshot 2024-10-16 at 12 48 06" src="https://github.com/user-attachments/assets/3c27de69-364e-4e6f-a4fb-7f5f48a40c42">
</p>

- Content
  - [0. Why am I curating this repository?](#0-why-am-i-curating-this-repository)
  - [1. Chart Captioning](#1-chart-captioning)
  - [🔥 2. Chart Question Answering](#2-chart-question-answering)
    - [2.0 Data, Model](#20-data-model)
    - [2.1 Benchmark](#21-benchmark)
    - [2.3 Application Scenarios (e.g., Accessibility)](#23-application-scenarios)
  - [3. Chart Reverse Engineering](#3-chart-reverse-engineering)
  - [4. Natural Language to Visualization](#4-natural-language-to-visualization)
     - [4.0 Method, Framework, and Benchmark](#40-method-framework-and-benchmark)
     - [4.1 Application Scenarios (e.g., Storytelling)](#41-application-scenarios)
  - [5. Visualization Design](#5-visualization-design)
    - [5.0 Color](#50-color)
    - [5.1 Design Preferences](#51-design-preferences)
    - [5.2 User-Adaptive Visualization](#52-user-adaptive-visualization)
  - [6. Visualization Agents & Automatic Judge](#6-visualization-agents--automatic-judge)
  - [7. Empirical Study on LLM's Chart Understanding & Chart Generation](#7-empirical-study-on-llms-chart-understanding--chart-generation)
  - [🔥 8. Visualization for Interpreting, Evaluating, and Improving LLM](#8-visualization-for-interpreting-evaluating-and-improving-llm)
  - [9. Generic Multimodal Large Language Model](#9-generic-multimodal-large-language-model)
  - [10. Related Survey Papers](#10-related-survey-papers)
  - [11. Others](#11-others)

## 0. Why am I curating this repository?
- I've found that the existing **Vis**x**LLM** paper-list repositories are updated infrequently (they're more likely created for a survey paper and then abandoned). I will gradually enrich this repository and keep it updated.
- Feel free to open an issue or a pull request to add a new paper you appreciate.
- **Star and watch this repo for future updates 😁.**
- **Strongly recommend the tutorial [LLM4Vis: Large Language Models for Information Visualization](https://nlp4vis.github.io/) delivered by Prof. Hoque.**
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


##  2. Chart Question Answering


### 2.0 Data, Model
**Advancing Multimodal Large Language Models in Chart Question Answering with Visualization-Referenced Instruction Tuning**  
Xingchen Zeng, Haichuan Lin, Yilin Ye, Wei Zeng  
[VIS 2024](https://arxiv.org/abs/2407.20174) • [Code](https://github.com/zengxingchen/ChartQA-MLLM)

**AskChart: Universal Chart Understanding through Textual Enhancement**  
Xudong Yang, Yifan Wu, Yizhang Zhu, Nan Tang, Yuyu Luo <br>
[arXiv, 26 Dec 2024](https://arxiv.org/abs/2412.19146)

**Distill Visual Chart Reasoning Ability from LLMs to MLLMs** <br>
Wei He, Zhiheng Xi, Wanxu Zhao, Xiaoran Fan, Yiwen Ding, Zifei Shan, Tao Gui, Qi Zhang, Xuanjing Huang <br>
[arXiv, 24 Oct 2024](https://arxiv.org/abs/2410.18798) • [Code](https://github.com/hewei2001/ReachQA)

**SynChart: Synthesizing Charts from Language Models**  
Mengchen Liu, Qixiu Li, Dongdong Chen, Dong Chen, Jianmin Bao, Yunsheng Li  
[arXiv, 25 Sep 2024](https://arxiv.org/abs/2409.16517)

**ChartMoE: Mixture of Expert Connector for Advanced Chart Understanding**   
Zhengzhuo Xu, Bowen Qu, Yiyan Qi, Sinan Du, Chengjin Xu, Chun Yuan, Jian Guo   
[arXiv, 5 Sep 2024](https://arxiv.org/abs/2409.03277) • [Code](https://chartmoe.github.io/)

**On Pre-training of Multimodal Language Models Customized for Chart Understanding** <br>
Wan-Cyuan Fan, Yen-Chun Chen, Mengchen Liu, Lu Yuan, Leonid Sigal <br>
[arXiv, 19 Jul 2024](https://arxiv.org/abs/2407.14506)

**ChartGemma: Visual Instruction-tuning for Chart Reasoning in the Wild** <br>
Ahmed Masry, Megh Thakkar, Aayush Bajaj, Aaryaman Kartha, Enamul Hoque, Shafiq Joty <br>
[arXiv, 4 Jul 2024](https://arxiv.org/pdf/2407.04172) • [Code](https://github.com/vis-nlp/ChartGemma)

**TinyChart: Efficient Chart Understanding with Visual Token Merging and Program-of-Thoughts Learning**  
Liang Zhang*, Anwen Hu*, Haiyang Xu, Ming Yan, Yichen Xu, Qin Jin†, Ji Zhang, Fei Huang  
[EMNLP 2024](https://arxiv.org/pdf/2404.16635) • [Code](https://github.com/X-PLUG/mPLUG-DocOwl/tree/main/TinyChart)

**OneChart: Purify the Chart Structural Extraction via One Auxiliary Token**  
Jinyue Chen*, Lingyu Kong*, Haoran Wei, Chenglong Liu, Zheng Ge, Liang Zhao, Jianjian Sun, Chunrui Han, Xiangyu Zhang  
[ACM MM 2024 (Oral)](https://arxiv.org/pdf/2404.09987) • [Homepage](https://onechartt.github.io/)


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

**Chart-based Reasoning: Transferring Capabilities from LLMs to VLMs** <br>
Victor Carbune, Hassan Mansoor, Fangyu Liu, Rahul Aralikatte, Gilles Baechler, Jindong Chen, Abhanshu Sharma<br>
[NAACL'24 Findings](https://arxiv.org/pdf/2403.12596)

**Synthesize Step-by-Step: Tools Templates and LLMs as Data Generators for Reasoning-Based Chart VQA**  
Zhuowan Li, Bhavan Jasani, Peng Tang, Shabnam Ghadar  
[CVPR 2024](https://openaccess.thecvf.com/content/CVPR2024/papers/Li_Synthesize_Step-by-Step_Tools_Templates_and_LLMs_as_Data_Generators_for_CVPR_2024_paper.pdf)

**Chartllama: A multimodal llm for chart understanding and generation**  
Yucheng Han, Chi Zhang, Xin Chen, Xu Yang, Zhibin Wang, Gang Yu, Bin Fu, Hanwang Zhang <br>
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

**LEAF-QA: Locate, Encode & Attend for Figure Question Answering** <br>
haudhry, Ritwick and Shekhar, Sumit and Gupta, Utkarsh and Maneriker, Pranav and Bansal, Prann and Joshi, Ajay <br>
[WACV 2020](https://openaccess.thecvf.com/content_WACV_2020/papers/Chaudhry_LEAF-QA_Locate_Encode__Attend_for_Figure_Question_Answering_WACV_2020_paper.pdf)


### 2.1 Benchmark
**CharXiv: Charting Gaps in Realistic Chart Understanding in Multimodal LLMs**  
 Zirui Wang, Mengzhou Xia, Luxi He, Howard Chen, Yitao Liu, Richard Zhu, Kaiqu Liang, Xindi Wu, Haotian Liu, Sadhika Malladi, Alexis Chevalier, Sanjeev Arora, Danqi Chen  
[NeurIPS 2024 Benchmark](http://arxiv.org/abs/2406.18521) • [Homepage](https://charxiv.github.io/)

**ChartInsights: Evaluating Multimodal Large Language Models for Low-Level Chart Question Answering**  
Yifan Wu, Lutao Yan, Leixian Shen, Yunhai Wang, Nan Tang, Yuyu Luo  
[Findings of EMNLP 2024](https://arxiv.org/pdf/2405.07001)  • [Code](https://chartinsight.github.io/)

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

**InfographicVQA** <br>
Minesh Mathew, Viraj Bagal, Rubèn Pérez Tito, Dimosthenis Karatzas, Ernest Valveny, C.V Jawahar <br>
[WACV 2022](https://openaccess.thecvf.com/content/WACV2022/papers/Mathew_InfographicVQA_WACV_2022_paper.pdf)  • [Homepage](https://www.docvqa.org/datasets/infographicvqa)

**PlotQA: Reasoning over Scientific Plots**  <br>
Pritha Ganguly, Nitesh Methani, Mitesh Khapra, Pratyush Kumar  <br>
[WACV 2020](https://arxiv.org/pdf/1909.00997.pdf) • [Code](https://github.com/NiteshMethani/PlotQA)

**Dvqa: Understanding data visualizations via question answering**  
Kushal Kafle, Brian Price, Scott Cohen, Christopher Kanan  
[CVPR 2018](https://openaccess.thecvf.com/content_cvpr_2018/papers/Kafle_DVQA_Understanding_Data_CVPR_2018_paper.pdf) • [Code](https://github.com/kushalkafle/DVQA_dataset)

**FigureQA: An Annotated Figure Dataset for Visual Reasoning** <br>
Samira Ebrahimi Kahou, Vincent Michalski, Adam Atkinson, Akos Kadar, Adam Trischler, Yoshua Bengio <br>
[ICLR 2018 Workshop track](https://arxiv.org/pdf/1710.07300) • [Code](https://github.com/vmichals/FigureQA-baseline)

### 2.3 Application Scenarios
**VizAbility: Enhancing Chart Accessibility with LLM-based Conversational Interaction** <br>
Joshua Gorniak, Yoon Kim, Donglai Wei, Nam Wook Kim <br>
[UIST 2024](https://dl.acm.org/doi/abs/10.1145/3654777.3676414)

## 3. Chart Reverse Engineering
**ChartCoder: Advancing Multimodal Large Language Model for Chart-to-Code Generation** <br>
Xuanle Zhao, Xianzhen Luo, Qi Shi, Chi Chen, Shuo Wang, Wanxiang Che, Zhiyuan Liu, Maosong Sun <br>
[arXiv, 11 Jan 2025](https://arxiv.org/abs/2501.06598) • [Code](https://github.com/thunlp/ChartCoder)

**ChartMimic: Evaluating LMM’s Cross-Modal Reasoning Capability via Chart-to-Code Generation**  
Chufan Shi and Cheng Yang and Yaxin Liu and Bo Shui and Junjie Wang and Mohan Jing and Linran Xu and Xinyu Zhu and Siheng Li and Yuxiang Zhang and Gongye Liu and Xiaomei Nie and Deng Cai and Yujiu Yang  
[arXiv, 14 Jun 2024](https://arxiv.org/pdf/2406.09961) • [Homepage](https://chartmimic.github.io/)

**Plot2Code: A Comprehensive Benchmark for Evaluating Multi-modal Large Language Models in Code Generation from Scientific Plots**
Chengyue Wu, Yixiao Ge, Qiushan Guo, Jiahao Wang, Zhixuan Liang, Zeyu Lu, Ying Shan, Ping Luo <br>
[arXiv, 13 May 2024](https://arxiv.org/pdf/2405.07990)

**Is GPT-4V (ision) All You Need for Automating Academic Data Visualization? Exploring Vision-Language Models’ Capability in Reproducing Academic Charts** <br>
Zhehao Zhang, Weicheng Ma, Soroush Vosoughi <br>
[EMNLP2024 Findings](https://aclanthology.org/2024.findings-emnlp.485.pdf)  • [Code](https://github.com/zzh-SJTU/AcademiaChart)




--- Pre-LLM ---  
**InvVis: Large-scale data embedding for invertible visualization** <br>
Huayuan Ye, Chenhui Li, Yang Li and Changbo Wang <br>
[VIS 2023](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10290968)

**Deep colormap extraction from visualizations**  
Lin-Ping Yuan, Wei Zeng, Siwei Fu, Zhiliang Zeng, Haotian Li, Chi-Wing Fu, Huamin Qu  
[TVCG 2022](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9395231)

**Chartem: Reviving Chart Images with Data Embedding** <br>
Jiayun Fu, Bin Zhu, Weiwei Cui, Song Ge, Yun Wang, Haidong Zhang, He Huang, Yuanyuan Tang, Dongmei Zhang, and Xiaojing Ma <br>
[TVCG 2021](https://ieeexplore.ieee.org/abstract/document/9293003)



**Reverse‐engineering visualizations: Recovering visual encodings from chart images**  
Jorge Poco and Jeffrey Heer  
[EuroVis 2017](https://onlinelibrary.wiley.com/doi/pdf/10.1111/cgf.13193)


## 4. Natural Language to Visualization
### 4.0 Method, Framework, and Benchmark

**ChartifyText: Automated Chart Generation from Data-Involved Texts via LLM** <br>
Songheng Zhang, Lei Wang, Toby Jia-Jun Li, Qiaomu Shen, Yixin Cao, Yong Wang <br>
[arXiv, 7 Nov 2024](https://arxiv.org/pdf/2410.14331)

**VisEval: A benchmark for data visualization in the era of large language models**  
Nan Chen, Yuge Zhang, Jiahang Xu, Kan Ren, and Yuqing Yang  
[VIS 2024](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=10670425)  • [Code](https://github.com/microsoft/VisEval)


**Chartgpt: Leveraging LLMs to generate charts from abstract natural language**  
Yuan Tian, Weiwei Cui, Dazhen Deng, Xinjing Yi, Yurun Yang, Haidong Zhang, Yingcai Wu  
[TVCG 2024](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=10443572)

**LLM4Vis: Explainable Visualization Recommendation using ChatGPT**  
Lei Wang, Songheng Zhang, Yun Wang, Ee-Peng Lim, Yong Wang  
[EMNLP 2023 Industry](https://aclanthology.org/2023.emnlp-industry.64.pdf)  • [Code](https://github.com/demoleiwang/LLM4Vis)  

**LIDA: A Tool for Automatic Generation of Grammar-Agnostic Visualizations and Infographics using Large Language Models**  
Victor Dibia  
[ACL 2023 Demo](https://arxiv.org/pdf/2303.02927) • [Code](https://github.com/microsoft/lida)

--- Pre-LLM ---  

**Natural Language to Visualization by Neural Machine Translation**  
Yuyu Luo, Nan Tang, Guoliang Li, Jiawei Tang, Chengliang Chai, Xuedi Qin  
[VIS 2021](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9617561) • [Code](https://github.com/HKUSTDial/ncNet) 

**nvBench: A Large-Scale Synthesized Dataset for Cross-Domain Natural Language to Visualization Task**  
Yuyu Luo, Jiawei Tang, Guoliang Li  
[Workshop on NL VIZ 2021 at IEEE VIS 2021](https://arxiv.org/pdf/2112.12926) • [Code](https://github.com/TsinghuaDatabaseGroup/nvBench)

**Table2Charts: Recommending Charts by Learning Shared Table Representations** <br>
Zhou, Mengyu and Li, Qingtao and He, Xinyi and Li, Yuejiang and Liu, Yibo and Ji, Wei and Han, Shi and Chen, Yining and Jiang, Daxin and Zhang, Dongmei <br>
[KDD 2021](https://dl.acm.org/doi/pdf/10.1145/3447548.3467279) • [Code](https://github.com/microsoft/Table2Charts)

### 4.1 Application Scenarios

**DataNarrative: Automated Data-Driven Storytelling with Visualizations and Texts** <br>
Mohammed Saidul Islam, Enamul Hoque, Shafiq Joty, Md Tahmid Rahman Laskar, Md Rizwan Parvez <br>
[EMNLP 2024](https://arxiv.org/pdf/2408.05346) • [Code](https://github.com/saidul-islam98/DataNarrative)

**Beyond generating code: Evaluating gpt on a data visualization course**  
Zhutian Chen, Chenyang Zhang, Qianwen Wang, Jakob Troidl, Simon Warchol, Johanna Beyer  
[EduVis 2024](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10344146)  • [Code](https://github.com/GPT4VIS/GPT-4-CS171)

**SNIL: Generating Sports News from Insights with Large Language Models** <br>
Liqi Cheng, Dazhen Deng, Xiao Xie, Rihong Qiu, Mingliang Xu, Yingcai Wu  
[TVCG 2024](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=10507016)


## 5. Visualization Design
### 5.0 Color
**Large Language Models estimate fine-grained human color-concept associations** <br>
Kushin Mukherjee, Timothy T. Rogers, Karen B. Schloss <br>
[arXiv, 4 May 2024](https://arxiv.org/abs/2406.17781)

**NL2Color: Refining Color Palettes for Charts with Natural Language**  
Chuhan Shi, Weiwei Cui, Chengzhong Liu, Chengbo Zheng, Haidong Zhang, Qiong Luo, and Xiaojuan Ma  
[VIS 2023](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10292693)

### 5.1 Design Preferences
**DracoGPT: Extracting Visualization Design Preferences from Large Language Models**  
Huichen Will Wang, Mitchell Gordon, Leilani Battle, and Jeffrey Heer  
[VIS 2024](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10681108)

**Bavisitter: Integrating Design Guidelines into Large Language Models for Visualization Authoring**  
Jiwon Choi, Jaeung Lee, Jaemin Jo  
[VIS 2024 Short Paper](https://idclab.skku.edu/assets/Bavisitter.pdf)

### 5.2 User-Adaptive Visualization
**User-Adaptive Visualizations: An Exploration with GPT-4**  
F. Yanez and C. Nobre  
[MLVis 2024](https://diglib.eg.org/server/api/core/bitstreams/23abe5fb-4de1-432f-97ab-ad757f5418e3/content)

## 6. Visualization Agents & Automatic Judge
**The Visualization JUDGE: Can Multimodal Foundation Models Guide Visualization Design Through Visual Perception?**  
Matthew Berger, Shusen Liu  
[arXiv, 5 Oct 2024](https://arxiv.org/pdf/2410.04280)  

**MatPlotAgent: Method and Evaluation for LLM-Based Agentic Scientific Data Visualization**
Zhiyu Yang and Zihan Zhou and Shuo Wang and Xin Cong and Xu Han and Yukun Yan and Zhenghao Liu and Zhixing Tan and Pengyuan Liu and Dong Yu and Zhiyuan Liu and Xiaodong Shi and Maosong Sun  
[Findings of ACL 2024](https://aclanthology.org/2024.findings-acl.701.pdf) • [Code](https://github.com/thunlp/MatPlotAgent)  

**WaitGPT: Monitoring and Steering Conversational LLM Agent in Data Analysis with On-the-Fly Code Visualization**  
Liwenhan Xie, Chengbo Zheng, Haijun Xia, Huamin Qu, Chen Zhu-Tian   
[UIST 2024](https://arxiv.org/pdf/2408.01703)

**AVA: Towards Autonomous Visualization Agents through Visual Perception‐Driven Decision‐Making**  
Shusen Liu, Haichao Miao, Zhimin Li, Matthew Olson, Valerio Pascucci, P‐T Bremer  
[EuroVis 2024](https://onlinelibrary.wiley.com/doi/pdf/10.1111/cgf.15093)  

**AVA: An automated and AI-driven intelligent visual analytics framework**  
Jiazhe Wang, Xi Li, Chenlu Li, Di Peng, Arran Zeyu Wang, Yuhui Gu, Xingui Lai, Haifeng Zhang, Xinyue Xu, Xiaoqing Dong, Zhifeng Lin, Jiehui Zhou, Xingyu Liu, Wei Chen  
[Visual Informatics 2024](https://www.sciencedirect.com/science/article/pii/S2468502X24000226)

**LEVA: Using large language models to enhance visual analytics** <be>
Yuheng Zhao, Yixing Zhang, Yu Zhang, Xinyi Zhao, Junjie Wang, Zekai Shao, Cagatay Turkay, Siming Chen <br>
[TVCG 2024](https://arxiv.org/pdf/2403.05816)

## 7. Empirical Study on LLM's Chart Understanding & Chart Generation 
**How Aligned are Human Chart Takeaways and LLM Predictions? A Case Study on Bar Charts with Varying Layouts**  
Huichen Will Wang, Jane Hoffswell, Sao Myat Thazin Thane, Victor S Bursztyn, Cindy Xiong Bearfield  
[VIS 2024](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=10681139)

**An Empirical Evaluation of the GPT-4 Multimodal Language Model on Visualization Literacy Tasks**  
Alexander Bendeck, John Stasko  
[VIS 2024](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=10670574)

**Visualization Literacy of Multimodal Large Language Models: A Comparative Study**  
Zhimin Li, Haichao Miao, Valerio Pascucci, Shusen Liu  
[arXiv, 24 Jun 2024](https://arxiv.org/pdf/2407.10996)

**Enhancing Data Literacy On-demand: LLMs as Guides for Novices in Chart Interpretation**  
Kiroong Choe, Chaerin Lee, S. Lee, Jiwon Song, Aeri Cho, Nam Wook Kim, Jinwook Seo  
[VIS 2024](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10555321)

**Promises and Pitfalls: Using Large Language Models to Generate Visualization Items**  
Yuan Cui, Lily W. Ge, Yiren Ding, Lane Harrison, Fumeng Yang, and Matthew Kay  
[VIS 2024](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=10670418)

**How Good (Or Bad) Are LLMs at Detecting Misleading Visualizations?**  
Leo Yu-Ho Lo, Huamin Qu  
[VIS 2024](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=10679256)

**Exploring the Capability of LLMs in Performing Low-Level Visual Analytic Tasks on SVG Data Visualizations**  
Zhongzheng Xu, Emily Wall  
[VIS 2024 Short Paper](https://arxiv.org/pdf/2404.19097)

**Evaluating the Semantic Profiling Abilities of LLMs for Natural Language Utterances in Data Visualization**  
Hannah K Bako, Arshnoor Buthani, Xinyi Liu, Kwesi A Cobbina, Zhicheng Liu  
[VIS 2024 Short Paper](https://arxiv.org/pdf/2407.06129) • [Code](https://github.com/hdi-umd/Semantic_Profiling_LLM_Evaluation)

## 8. Visualization for Interpreting, Evaluating, and Improving LLM
> If you are interested in this topic, you can find some interesting interactive papers/demos in the [VISxAI workshop](https://visxai.io/).

**LVLM-Interpret: An Interpretability Tool for Large Vision-Language Models** <br>
Gabriela Ben Melech Stan, Estelle Aflalo, Raanan Yehezkel Rohekar, Anahita Bhiwandiwalla, Shao-Yen Tseng, Matthew Lyle Olson, Yaniv Gurwicz, Chenfei Wu, Nan Duan, Vasudev Lal <br>
[arXiv, 3 Apr 2024](https://arxiv.org/abs/2404.03118) • [Homepage](https://intellabs.github.io/multimodal_cognitive_ai/lvlm_interpret/)

**LLM Comparator: Interactive Analysis of Side-by-Side Evaluation of Large Language Models**  
Minsuk Kahng, Ian Tenney, Mahima Pushkarna, Michael Xieyang Liu, James Wexler, Emily Reif, Krystal Kallarackal, Minsuk Chang, Michael Terry, and Lucas Dixon  
[VIS 2024](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10670495)  • [Code](https://github.com/PAIR-code/llm-comparator) • [Demo](https://pair-code.github.io/llm-comparator/)

**Towards Dataset-scale and Feature-oriented Evaluation of Text Summarization in Large Language Model Prompts**  
Sam Yu-Te Lee, Aryaman Bahukhandi, Dongyu Liu, Kwan-Liu Ma  
[VIS 2024](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=10669798) 

**LLM Attributor: Attribute LLM's Generated Text to Training Data**  
Seongmin Lee, Zijie J. Wang, Aishwarya Chakravarthy, Alec Helbling, ShengYun Peng, Mansi Phute, Duen Horng (Polo) Chau, Minsuk Kahng  
[VIS 2024 Poster](http://arxiv.org/abs/2404.01361) • [Code](https://github.com/poloclub/LLM-Attributor)

**Can Large Language Models Explain Their Internal Mechanisms?**
Nada Hussein, Asma Ghandeharioun, Ryan Mullins, Emily Reif, Jimbo Wilson, Nithum Thain and Lucas Dixon  
[VISxAI Workshop 2024 & Demo](https://pair.withgoogle.com/explorables/patchscopes/)

**ExplainPrompt: Decoding the language of AI prompts**  
Shawn Simister  
[VISxAI Workshop 2024 & Demo](https://www.explainprompt.com/)

**Attentionviz: A global view of transformer attention**  
Catherine Yeh, Yida Chen, Aoyu Wu, Cynthia Chen, Fernanda Viégas, Martin Wattenberg  
[VIS 2023](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=10297591) • [Demo](http://attentionviz.com)

**Do Machine Learning Models Memorize or Generalize?**  
Adam Pearce, Asma Ghandeharioun, Nada Hussein, Nithum Thain, Martin Wattenberg and Lucas Dixon  
[VISxAI Workshop 2023 & Demo](https://pair.withgoogle.com/explorables/grokking/)

## 9. Generic Multimodal Large Language Model
> Refer to [Awesome-Multimodal-Large-Language-Models](https://github.com/BradyFU/Awesome-Multimodal-Large-Language-Models) for a more comprehensive list. This repo only records papers that bring insights to **LLM**x**Vis**.

**ControlMLLM: Training-Free Visual Prompt Learning for Multimodal Large Language Models** <br>
Mingrui Wu, Xinyue Cai, Jiayi Ji, Jiale Li, Oucheng Huang, Gen Luo, Hao Fei, Guannan Jiang, Xiaoshuai Sun, Rongrong Ji <br>
[NIPS 2024](https://arxiv.org/pdf/2407.21534) • [Code](https://github.com/mrwu-mac/ControlMLLM)


**MM1.5: Methods, Analysis & Insights from Multimodal LLM Fine-tuning**  
Haotian Zhang, Mingfei Gao, Zhe Gan, Philipp Dufter, Nina Wenzel, Forrest Huang, Dhruti Shah, Xianzhi Du, Bowen Zhang, Yanghao Li, Sam Dodge, Keen You, Zhen Yang, Aleksei Timofeev, Mingze Xu, Hong-You Chen, Jean-Philippe Fauconnier, Zhengfeng Lai, Haoxuan You, Zirui Wang, Afshin Dehghan, Peter Grasch, Yinfei Yang  
[arXiv, 30 Sep 2024](https://arxiv.org/pdf/2409.20566)  

**Law of Vision Representation in MLLMs** <br>
Shijia Yang, Bohan Zhai, Quanzeng You, Jianbo Yuan, Hongxia Yang, Chenfeng Xu <br>
[arXiv, 29 Aug 2024](https://arxiv.org/pdf/2408.16357)

**EAGLE: Exploring The Design Space for Multimodal LLMs with Mixture of Encoders**  
Min Shi*, Fuxiao Liu*, Shihao Wang, Shijia Liao, Subhashree Radhakrishnan, De-An Huang, Hongxu Yin, Karan Sapra, Yaser Yacoob, Humphrey Shi, Bryan Catanzaro, Andrew Tao, Jan Kautz, Zhiding Yu, Guilin Liu  
[arXiv, 28 Aug 2024](https://arxiv.org/abs/2408.15998) • [Code](https://github.com/NVlabs/EAGLE)

**Cambrian-1: A Fully Open, Vision-Centric Exploration of Multimodal LLMs**  
Shengbang Tong*, Ellis Brown*, Penghao Wu*, Sanghyun Woo, Manoj Middepogu, Sai Charitha Akula, Jihan Yang, Shusheng Yang, Adithya Iyer, Xichen Pan, Austin Wang, Rob Fergus, Yann LeCun, Saining Xie  
[arXiv, 24 Jun 2024](https://arxiv.org/abs/2408.15998) • [Code](https://github.com/cambrian-mllm/cambrian)

**DeCo: Decoupling Token Compression from Semantic Abstraction in Multimodal Large Language Models** <br>
Linli Yao, Lei Li, Shuhuai Ren, Lean Wang, Yuanxin Liu, Xu Sun, Lu Hou <br>
[arXiv, 31 May 2024](https://arxiv.org/abs/2405.20985) • [Code](https://github.com/yaolinli/DeCo)


**Eyes Wide Shut? Exploring the Visual Shortcomings of Multimodal LLMs** <br>
Shengbang Tong, Zhuang Liu, Yuexiang Zhai, Yi Ma, Yann LeCun, Saining Xie <br>
[CVPR 2024](https://openaccess.thecvf.com/content/CVPR2024/papers/Tong_Eyes_Wide_Shut_Exploring_the_Visual_Shortcomings_of_Multimodal_LLMs_CVPR_2024_paper.pdf)

**InternVL: Scaling up Vision Foundation Models and Aligning for Generic Visual-Linguistic Tasks** <br>
Zhe Chen, Jiannan Wu, Wenhai Wang, Weijie Su, Guo Chen, Sen Xing, Muyan Zhong, Qinglong Zhang, Xizhou Zhu, Lewei Lu, Bin Li, Ping Luo, Tong Lu, Yu Qiao, Jifeng Dai <br>
[CVPR 2024](https://arxiv.org/abs/2312.14238)

**Shikra: Unleashing Multimodal LLM’s Referential Dialogue Magic** <br>
[arXiv, 27 Jun 2023](https://arxiv.org/abs/2306.15195) • [Code](https://github.com/shikras/shikra)

## 10. Related Survey Papers
**Natural Language Generation for Visualizations: State of the Art, Challenges and Future Directions** <br>
Enamul Hoque, Mohammed Saidul Islam <br>
[arXiv, 29 Sep 2024](https://arxiv.org/pdf/2409.19747) 

**Generative AI for visualization: State of the art and future directions**  
Yilin Ye, Jianing Hao, Yihan Hou, Zhan Wang, Shishi Xiao, Yuyu Luo, Wei Zeng  
[Visual Informatics 2024](https://www.sciencedirect.com/science/article/pii/S2468502X24000160)

**Datasets of Visualization for Machine Learning**  
Can Liu, Ruike Jiang, Shaocong Tan, Jiacheng Yu, Chaofan Yang, Hanning Shao, Xiaoru Yuan  
[arXiv, 23 Jul 2024](https://arxiv.org/pdf/2407.16351) 

**Foundation models meet visualizations: Challenges and opportunities**  
Weikai Yang, Mengchen Liu, Zheng Wang, Shixia Liu  
[CVM 2024](https://link.springer.com/article/10.1007/s41095-023-0393-x)

**From Detection to Application: Recent Advances in Understanding Scientific Tables and Figures**  
Jiani Huang, Haihua Chen, Fengchang Yu, Wei Lu  
[ACM Computing Surveys 2024](https://dl.acm.org/doi/pdf/10.1145/3657285)

**From Pixels to Insights: A Survey on Automatic Chart Understanding in the Era of Large Foundation Models**  
Kung-Hsiang Huang, Hou Pong Chan, Yi R. Fung, Haoyi Qiu, Mingyang Zhou, Shafiq Joty, Shih-Fu Chang, Heng Ji  
[arXiv, 18 Mar 2024](https://arxiv.org/pdf/2403.12027)

**Leveraging large models for crafting narrative visualization: a survey**  
Yi He, Shixiong Cao, Yang Shi, Qing Chen, Ke Xu, Nan Cao  
[arXiv, 25 Jan 2024](https://arxiv.org/pdf/2401.14010)

**Natural Language Interfaces for Tabular Data Querying and Visualization: A Survey** <br>
Weixu Zhang, Yifei Wang, Yuanfeng Song, Victor Junqiu Wei, Yuxing Tian, Yiyan Qi, Jonathan H. Chan, Raymond Chi-Wing Wong, Haiqin Yang <br>
[arXiv, 27 Oct 2023](https://arxiv.org/pdf/2310.17894) 

**AI4VIS: Survey on Artificial Intelligence Approaches for Data Visualization**  
Aoyu Wu, Yun Wang, Xinhuan Shu, Dominik Moritz, Weiwei Cui, Haidong Zhang, Dongmei Zhang, and Huamin Qu  
[TVCG 2022](https://arxiv.org/pdf/2102.01330) • [Homepage](https://ai4vis.github.io/)

**Chart Question Answering: State of the Art and Future Directions**  
Enamul Hoque, Parsa Kavehzadeh, Ahmed Masry  
[EuroVis 2022](https://onlinelibrary.wiley.com/doi/epdf/10.1111/cgf.14573) 

**Towards Natural Language Interfaces for Data Visualization: A Survey**  
Leixian Shen, Enya Shen, Yuyu Luo, Xiaocong Yang, Xuming Hu, Xiongshuai Zhang, Zhiwei Tai, Jianmin Wang  
[TVCG 2022](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9699035)


## 11. Others
**VisAnatomy: An SVG Chart Corpus with Fine-Grained Semantic Labels** <br>
Chen Chen, Hannah K. Bako, Peihong Yu, John Hooker, Jeffrey Joyal, Simon C. Wang, Samuel Kim, Jessica Wu, Aoxue Ding, Lara Sandeep, Alex Chen, Chayanika Sinha, Zhicheng Liu <br>
[arXiv, 16 Oct 2024](https://arxiv.org/pdf/2410.12268)  • [Homepage](https://visanatomy.github.io/)

**Multimodal Chart Retrieval: A Comparison of Text, Table and Image Based Approaches** <br>
Averi Nowak, Francesco Piccinno, Yasemin Altun <br>
[NAACL 2024](https://aclanthology.org/2024.naacl-long.307/)


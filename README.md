# LLM-Visualization-Paper-List
Why am I curating this repository?
- I've found that the chart-LLM-related repositories are updated infrequently (they're more likely created for a survey paper and then abandoned). I will gradually enrich this repository and keep it updated.


## 0. Chart Captioning

**Natural Language Dataset Generation Framework for Visualizations Powered by Large Language Models** \
Hyung-Kwon Ko, Hyeon Jeon, Gwanmo Park, Dae Hyun Kim, Nam Wook Kim, Juho Kim, Jinwook Seo \
[CHI 2024](https://arxiv.org/abs/2309.10245) • [Code](https://github.com/hyungkwonko/chart-llm)

**VisText: A Benchmark for Semantically Rich Chart Captioning** \
Benny J. Tang, Angie Boggust, Arvind Satyanarayan \
[ACL 2023 Outstanding paper](https://aclanthology.org/2023.acl-long.401.pdf) • [Code](https://github.com/mitvis/vistext)

--- Pre-LLM --- \
**Chart-to-Text: A Large-Scale Benchmark for Chart Summarization** \
Shankar Kantharaj, Rixie Tiffany Leong, Xiang Lin, Ahmed Masry, Megh Thakkar, Enamul Hoque, Shafiq Joty  
[ACL 2022](https://aclanthology.org/2022.acl-long.277.pdf) • [Code](https://github.com/vis-nlp/Chart-to-text)


## 1. Chart Question Answering


### 1.0 Data, Model
**SynChart: Synthesizing Charts from Language Models** \
Mengchen Liu, Qixiu Li, Dongdong Chen, Dong Chen, Jianmin Bao, Yunsheng Li \
[arXiv](https://arxiv.org/abs/2409.16517)

**ChartMoE: Mixture of Expert Connector for Advanced Chart Understanding**  \
Zhengzhuo Xu, Bowen Qu, Yiyan Qi, Sinan Du, Chengjin Xu, Chun Yuan, Jian Guo  \
[arXiv, 5 Sep 2024](https://arxiv.org/abs/2409.03277) • [Code](https://chartmoe.github.io/)


**Advancing Multimodal Large Language Models in Chart Question Answering with Visualization-Referenced Instruction Tuning** \
Xingchen Zeng, Haichuan Lin, Yilin Ye, Wei Zeng \
[VIS 2024](https://arxiv.org/abs/2407.20174) • [Code](https://github.com/zengxingchen/ChartQA-MLLM)

**ChartAssistant: A Universal Chart Multimodal Language Model via Chart-to-Table Pre-training and Multitask Instruction Tuning** 
Fanqing Meng, Wenqi Shao, Quanfeng Lu, Peng Gao, Kaipeng Zhang, Yu Qiao, Ping Luo \
[Findings of ACL 2024](https://aclanthology.org/2022.findings-acl.177.pdf) • [code](https://github.com/OpenGVLab/ChartAst)

**Chartllama: A multimodal llm for chart understanding and generation**  
Fanqing Meng, Wenqi Shao, Quanfeng Lu, Peng Gao, Kaipeng Zhang, Yu Qiao, Ping Luo  
[arXiv](https://arxiv.org/pdf/2311.16483) • [homepage](https://tingxueronghua.github.io/ChartLlama/)


--- Pre-LLM --- \
**UniChart: A Universal Vision-language Pretrained Model for Chart Comprehension and Reasoning**  
Ahmed Masry∗, Parsa Kavehzadeh∗, Xuan Long Do, Enamul Hoque, Shafiq Joty  
[EMNLP 2023](https://aclanthology.org/2023.emnlp-main.906.pdf) • [code](https://github.com/vis-nlp/UniChart)

**Deplot: One-shot visual language reasoning by plot-to-table translation**  
Fangyu Liu, Julian Martin Eisenschlos, Francesco Piccinno, Syrine Krichene, Chenxi Pang, Kenton Lee, Mandar Joshi, Wenhu Chen, Nigel Collier, Yasemin Altun  
[Findings of ACL2023](https://aclanthology.org/2023.findings-acl.660.pdf) • [code](https://github.com/google-research/google-research/tree/master/deplot)

**MatCha: Enhancing Visual Language Pretraining with Math Reasoning and Chart Derendering**  
Fangyu Liu, Francesco Piccinno, Syrine Krichene, Chenxi Pang, Kenton Lee, Mandar Joshi, Yasemin Altun, Nigel Collier, Julian Martin Eisenschlos  
[ACL2023](https://aclanthology.org/2023.acl-long.714.pdf) • [code](https://github.com/google-research/google-research/tree/master/deplot)
### 1.1 Benchmark
**CharXiv: Charting Gaps in Realistic Chart Understanding in Multimodal LLMs**  
 Zirui Wang, Mengzhou Xia, Luxi He, Howard Chen, Yitao Liu, Richard Zhu, Kaiqu Liang, Xindi Wu, Haotian Liu, Sadhika Malladi, Alexis Chevalier, Sanjeev Arora, Danqi Chen \
[NeurIPS 2024 Benchmark](http://arxiv.org/abs/2406.18521) • [Homepage](https://charxiv.github.io/)

**ChartBench: A Benchmark for Complex Visual Reasoning in Charts**   
Zhengzhuo Xu*, Sinan Du*, Yiyan Qi, Chengjin Xu, Chun Yuan†, Jian Guo  
 [arXiv 26 Dec 2023](https://arxiv.org/pdf/2312.15915) • [homepage](https://chartbench.github.io/)

--- Pre-LLM --- \
**ChartQA: A Benchmark for Question Answering about Charts with Visual and Logical Reasoning** \
Ahmed Masry, Xuan Long Do, Jia Qing Tan, Shafiq Joty, Enamul Hoque \
[Findings of ACL 2022](https://aclanthology.org/2022.findings-acl.177.pdf) • [code](https://github.com/vis-nlp/chartqa)


## 2. Chart Reverse Engineering
**ChartMimic: Evaluating LMM’s Cross-Modal Reasoning Capability via Chart-to-Code Generation** \
Chufan Shi and Cheng Yang and Yaxin Liu and Bo Shui and Junjie Wang and Mohan Jing and Linran Xu and Xinyu Zhu and Siheng Li and Yuxiang Zhang and Gongye Liu and Xiaomei Nie and Deng Cai and Yujiu Yang  
[arXiv](https://arxiv.org/pdf/2406.09961) • [homepage](https://chartmimic.github.io/)

--- Pre-LLM --- \
**Reverse‐engineering visualizations: Recovering visual encodings from chart images** \
Jorge Poco and Jeffrey Heer \
[EuroVis 2017](https://onlinelibrary.wiley.com/doi/pdf/10.1111/cgf.13193)



## 2. Generic Multimodal Large Language Model
**EAGLE: Exploring The Design Space for Multimodal LLMs with Mixture of Encoders** \
Min Shi*, Fuxiao Liu*, Shihao Wang, Shijia Liao, Subhashree Radhakrishnan, De-An Huang, Hongxu Yin, Karan Sapra, Yaser Yacoob, Humphrey Shi, Bryan Catanzaro, Andrew Tao, Jan Kautz, Zhiding Yu, Guilin Liu \
[arXiv, 28 Aug 2024](https://arxiv.org/abs/2408.15998) • [code](https://github.com/NVlabs/EAGLE)

**Cambrian-1: A Fully Open, Vision-Centric Exploration of Multimodal LLMs** \
Shengbang Tong*, Ellis Brown*, Penghao Wu*, Sanghyun Woo, Manoj Middepogu, Sai Charitha Akula, Jihan Yang, Shusheng Yang, Adithya Iyer, Xichen Pan, Austin Wang, Rob Fergus, Yann LeCun, Saining Xie \
[arXiv, 24 Jun 2024](https://arxiv.org/abs/2408.15998) • [code](https://github.com/cambrian-mllm/cambrian)

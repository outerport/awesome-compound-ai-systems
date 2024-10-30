# Survey of Systems & Infrastructure for Compound AI

As society (individuals & enterprises) adopt generative AI, the use cases have moved beyond simple chat (response -> query) to automation workflows that involve multiple models, databases, API endpoints, microservices, and more. Reminiscent of the transition from monolith to microservices (and today, serverless orchestration), we are shifting from monolithic models to compound systems. As with previous technological shifts like photography, printing press, and record players, the artists are the innovators leading the adoption of compound systems, with systems like ComfyUI already showcasing what compound systems can do. 

As these systems mature and use cases shift from prototypes / PoCs to everyday features, however, so does the end user's expectaiton on quality of service. Balancing the complexity of compound systems with reliability is no easy task; and there is an increasing body of systems research done on this subject. 

This repository collects papers, talks, and blog posts which broadly discuss systems & infrastructure for compound AI. This is multidisciplinary field that involves systems, databases, machine learning, artificial intelligence, and more. 

This is very much work in progress and is missing lots of papers and works- and papers will be classified into categories eventually.

## Position Papers / Broadly Applicable Papers

[The Shift from Models to Compound AI Systems](https://bair.berkeley.edu/blog/2024/02/18/compound-ai-systems/)

## Papers

[MetaGPT: Meta Programming for A Multi-Agent Collaborative Framework](https://openreview.net/forum?id=VtmBAGCN7o)\
Sirui Hong, Mingchen Zhuge, Jonathan Chen, Xiawu Zheng, Yuheng Cheng, Ceyao Zhang, Jinlin Wang, Zili Wang, Steven Ka Shing Yau, Zijuan Lin, Liyang Zhou, Chenyu Ran, Lingfeng Xiao, Chenglin Wu, Jürgen Schmidhuber\
ICLR 2024

[Networks of Networks: Complexity Class Principles Applied to Compound AI Systems Design](https://arxiv.org/abs/2407.16831)\
Jared Quincy Davis, Boris Hanin, Lingjiao Chen, Peter Bailis, Ion Stoica, Matei Zaharia\
arXiv 2024

[Are More LLM Calls All You Need? Towards Scaling Laws of Compound Inference Systems](https://arxiv.org/abs/2403.02419)\
Lingjiao Chen, Jared Quincy Davis, Boris Hanin, Peter Bailis, Ion Stoica, Matei Zaharia, James Zou\
arXiv 2024

[Fine-Tuning Language Models Using Formal Methods Feedback: A Use Case in Autonomous Systems](https://arxiv.org/abs/2310.18239)\
Yunhao Yang, Neel P. Bhatt, Tyler Ingebrand, William Ward, Steven Carr, Atlas Wang, Ufuk Topcu\
MLSys 2024

[Parrot: Efficient Serving of LLM-based Applications with Semantic Variable](https://arxiv.org/abs/2405.19888)\
Chaofan Lin, Zhenhua Han, Chengruidong Zhang, Yuqing Yang, Fan Yang, Chen Chen, Lili Qiu\
OSDI 2024

[Conveyor: Efficient Tool-aware LLM Serving with Tool Partial Execution](https://openreview.net/forum?id=A0VvDN4arV)\
ICLR 2025 (in review)



### Scheduling and Orchestration

[dLoRA: Dynamically Orchestrating Requests and Adapters for LoRA LLM Serving](https://bingyangwu.github.io/publication/dlora/)\
Bingyang Wu, Ruidong Zhu, Zili Zhang, Peng Sun, Xuanzhe Liu, Xin Jin\
OSDI 2024

[Llumnix: Dynamic Scheduling for Large Language Model Serving](https://arxiv.org/abs/2406.03243)\
Biao Sun, Ziming Huang, Hanyu Zhao, Wencong Xiao, Xinyi Zhang, Yong Li, Wei Lin\
OSDI 2024

[ALTO: An Efficient Network Orchestrator for Compound AI Systems](https://dl.acm.org/doi/abs/10.1145/3642970.3655844)\
Keshav Santhanam, Deepti Raghavan, Muhammad Shahir Rahman, Thejas Venkatesh, Neha Kunjal, Pratiksha Thaker, Philip Levis, Matei Zaharia\
EuroMLSys 2024

[Punica: Multi-Tenant LoRA Serving](https://proceedings.mlsys.org/paper_files/paper/2024/hash/054de805fcceb78a201f5e9d53c85908-Abstract-Conference.html)\
Lequn Chen, Zihao Ye, Yongji Wu, Danyang Zhuo, Luis Ceze, Arvind Krishnamurthy\
MLSys 2024

[SLoRA: Scalable Serving of Thousands of LoRA Adapters](https://proceedings.mlsys.org/paper_files/paper/2024/hash/906419cd502575b617cc489a1a696a67-Abstract-Conference.html)\
Ying Sheng, Shiyi Cao, Dacheng Li, Coleman Hooper, Nicholas Lee, Shuo Yang, Christopher Chou, Banghua Zhu, Lianmin Zheng, Kurt Keutzer, Joseph Gonzalez, Ion Stoica\
MLSys 2024

[Preble: Efficient Distributed Prompt Scheduling for LLM Serving](https://openreview.net/forum?id=meKEKDhdnx)\
ICLR 2025 (in review)

[TPI-LLM: Serving 70B-scale LLMs Efficiently on Low-resource Edge Devices](https://openreview.net/forum?id=0cadcLKbt7)\
ICLR 2025 (in review)

### Caching

[DeepSpeed Inference: Enabling Efficient Inference of Transformer Models at Unprecedented Scale](https://arxiv.org/abs/2207.00032)\
Reza Yazdani Aminabadi, Samyam Rajbhandari, Minjia Zhang, Ammar Ahmad Awan, Cheng Li, Du Li, Elton Zheng, Jeff Rasley, Shaden Smith, Olatunji Ruwase, Yuxiong He\
arXiv 2022

[FlexGen: High-Throughput Generative Inference of Large Language Models with a Single GPU](https://arxiv.org/abs/2303.06865)\
Ying Sheng, Lianmin Zheng, Binhang Yuan, Zhuohan Li, Max Ryabinin, Daniel Y. Fu, Zhiqiang Xie, Beidi Chen, Clark Barrett, Joseph E. Gonzalez, Percy Liang, Christopher Ré, Ion Stoica, Ce Zhang\
ICML 2023

[Do Large Language Models Need a Content Delivery Network?](https://arxiv.org/abs/2409.13761)\
Yihua Cheng, Kuntai Du, Jiayi Yao, Junchen Jiang\
arXiv 2024

[Compute Or Load KV Cache? Why Not Both?](https://arxiv.org/abs/2410.03065)\
Shuowei Jin, Xueshen Liu, Qingzhao Zhang, Z. Morley Mao\
arXiv 2024

[CacheGen: KV Cache Compression and Streaming for Fast Large Language Model Serving](https://arxiv.org/abs/2310.07240)\
Yuhan Liu, Hanchen Li, Yihua Cheng, Siddhant Ray, Yuyang Huang, Qizheng Zhang, Kuntai Du, Jiayi Yao, Shan Lu, Ganesh Ananthanarayanan, Michael Maire, Henry Hoffmann, Ari Holtzman, Junchen Jiang\
arXiv 2024

[CacheBlend: Fast Large Language Model Serving for RAG with Cached Knowledge Fusion](https://arxiv.org/abs/2405.16444)\
Jiayi Yao, Hanchen Li, Yuhan Liu, Siddhant Ray, Yihua Cheng, Qizheng Zhang, Kuntai Du, Shan Lu, Junchen Jiang\
arXiv 2024

[TurboRAG: Accelerating Retrieval-Augmented Generation with Precomputed KV Caches for Chunked Text](https://arxiv.org/abs/2410.07590)\
Songshuo Lu, Hua Wang, Yutian Rong, Zhi Chen, Yaohua Tang\
arXiv 2024

[RAGCache: Efficient Knowledge Caching for Retrieval-Augmented Generation](https://arxiv.org/abs/2404.12457)\
Chao Jin, Zili Zhang, Xuanlin Jiang, Fangyue Liu, Xin Liu, Xuanzhe Liu, Xin Jin\
arXiv 2024

[LayerKV: Optimizing Large Language Model Serving with Layer-wise KV Cache Management](https://arxiv.org/abs/2410.00428)\
Yi Xiong, Hao Wu, Changxu Shao, Ziqing Wang, Rui Zhang, Yuhong Guo, Junping Zhao, Ke Zhang, Zhenxuan Pan\
arXiv 2024

[Harnessing Your DRAM and SSD for Sustainable and Accessible LLM Inference with Mixed-Precision and Multi-level Caching](https://arxiv.org/abs/2410.14740)\
Jie Peng, Zhang Cao, Huaizhi Qu, Zhengyu Zhang, Chang Guo, Yanyong Zhang, Zhichao Cao, Tianlong Chen\
arXiv 2024

[InstInfer: In-Storage Attention Offloading for Cost-Effective Long-Context LLM Inference](https://arxiv.org/abs/2409.04992)\
Xiurui Pan, Endian Li, Qiao Li, Shengwen Liang, Yizhou Shan, Ke Zhou, Yingwei Luo, Xiaolin Wang, Jie Zhang\
arXiv 2024

[MoE-Infinity: Offloading-Efficient MoE Model Serving](https://arxiv.org/abs/2401.14361)\
Leyang Xue, Yao Fu, Zhan Lu, Luo Mai, Mahesh Marina\
arXiv 2024

[Prompt Cache: Modular Attention Reuse for Low-Latency Inference](https://proceedings.mlsys.org/paper_files/paper/2024/hash/a66caa1703fe34705a4368c3014c1966-Abstract-Conference.html)\
In Gim, Guojun Chen, Seung-seob Lee, Nikhil Sarda, Anurag Khandelwal, Lin Zhong\
MLSys 2024

[InfiniGen: Efficient Generative Inference of Large Language Models with Dynamic KV Cache Management](https://arxiv.org/abs/2406.19707)\
Wonbeom Lee, Jungi Lee, Junghwan Seo, Jaewoong Sim\
OSDI 2024

[ServerlessLLM: Low-Latency Serverless Inference for Large Language Models](https://arxiv.org/abs/2401.14351)\
Yao Fu, Leyang Xue, Yeqi Huang, Andrei-Octavian Brabete, Dmitrii Ustiugov, Yuvraj Patel, Luo Mai\
OSDI 2024

### Compression

[Zero-Delay QKV Compression for Mitigating KV Cache and Network Bottlenecks in LLM Inference](https://arxiv.org/abs/2408.04107)\
Zeyu Zhang, Haiying Shen\
arXiv 2024

[MatryoshkaKV: Adaptive KV Compression via Trainable Orthogonal Projection](https://arxiv.org/abs/2410.14731)\
Bokai Lin, Zihao Zeng, Zipeng Xiao, Siqi Kou, Tianqi Hou, Xiaofeng Gao, Hao Zhang, Zhijie Deng\
arXiv 2024

[Compress then Serve: Serving Thousands of LoRA Adapters with Little Overhead](https://openreview.net/forum?id=hHNVn4hFPk)\
ICLR 2025 (in review)

[Interfering with Interference: Blind Shuffling and Superposition for Better Multi-Model Compression](https://openreview.net/forum?id=4wuvmJRAU4)\
ICLR 2025 (in review)

## Case Studies

[Agent S: An Open Agentic Framework that Uses Computers Like a Human](https://arxiv.org/abs/2410.08164)\
Saaket Agashe, Jiuzhou Han, Shuyu Gan, Jiachen Yang, Ang Li, Xin Eric Wang\
arXiv 2024

[Large Language Models for Software Engineering: A Systematic Literature Review](https://arxiv.org/abs/2308.10620)\
Xinyi Hou, Yanjie Zhao, Yue Liu, Zhou Yang, Kailong Wang, Li Li, Xiapu Luo, David Lo, John Grundy, Haoyu Wang\
Transactions on Software Engineering and Methodology 2024

[The AI Scientist: Towards Fully Automated Open-Ended Scientific Discovery](https://arxiv.org/abs/2408.06292)\
Chris Lu, Cong Lu, Robert Tjarko Lange, Jakob Foerster, Jeff Clune, David Ha\
arXiv 2024

[Self-Evolving Multi-Agent Collaboration Networks for Software Development](https://arxiv.org/abs/2410.16946)\
Yue Hu, Yuzhu Cai, Yaxin Du, Xinyu Zhu, Xiangrui Liu, Zijie Yu, Yuchen Hou, Shuo Tang, Siheng Chen\
arXiv 2024

[GraphTeam: Facilitating Large Language Model-based Graph Analysis via Multi-Agent Collaboration](https://arxiv.org/abs/2410.18032)\
Xin Li, Qizhi Chu, Yubin Chen, Yang Liu, Yaoqi Liu, Zekai Yu, Weize Chen, Chen Qian, Chuan Shi, Cheng Yang\
arXiv 2024

[Improving Planning with Large Language Models: A Modular Agentic Architecture](https://openreview.net/forum?id=iNcEChuYXD)\
ICLR 2025 (in submission)

## Surveys

[A Survey of Resource-efficient LLM and Multimodal Foundation Models](https://bingyangwu.github.io/publication/llmsurvey/)\
Mengwei Xu, Wangsong Yin, Dongqi Cai, Rongjie Yi, Daliang Xu, Qipeng Wang, Bingyang Wu, Yihao Zhao, Chen Yang, Shihe Wang, Qiyang Zhang, Zhenyan Lu, Li Zhang, Shangguang Wang, Yuanchun Li, Yunxin Liu, Xin Jin, Xuanzhe Liu\
arXiv 2024

[LLM Inference Serving: Survey of Recent Advances and Opportunities](https://arxiv.org/abs/2407.12391)\
Baolin Li, Yankai Jiang, Vijay Gadepally, Devesh Tiwari\
arXiv 2024

[On-Device LLMs for SMEs: Challenges and Opportunities](https://arxiv.org/abs/2410.16070)\
Jeremy Stephen Gabriel Yee, Pai Chet Ng, Zhengkui Wang, Ian McLoughlin, Aik Beng Ng, Simon See\
arXiv 2024


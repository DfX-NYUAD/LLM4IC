# LLM4IC

__Paper Title__: LLMs and the Future of Chip Design: Unveiling Security Risks and Building Trust
<u><a href="https://arxiv.org/pdf/2405.07061">[paper]</a></u>

__Author List__: Zeng Wang, Lilas Alrahis, Likhitha Mankali, Johann Knechtel, and Ozgur Sinanoglu

__Abstract__: Chip design is about to be revolutionized by the integration of large language, multimodal, and circuit models (collectively LxMs). While exploring this exciting frontier with tremendous potential, the community must also carefully consider the related security risks and the need for building trust into using LxMs for chip design. First, we review the recent surge of using LxMs for chip design in general. We cover state-of-the- art works for the automation of hardware description language code generation and for scripting and guidance of essential but cumbersome tasks for electronic design automation tools, e.g., design-space exploration, tuning, or designer training. Second, we raise and provide initial answers to novel research questions on critical issues for security and trustworthiness of LxM-powered chip design from both the attack and defense perspectives.

We summarize the resources on LLMs for chip design, focusing on various applications of LLMs, security concerns, and open sources.
## Table of Contents

- [1. Survey Papers](#survey-papers)
- [2. LLMs for EDA](#llm-for-eda)
  - [2.1 Verilog RTL Generation](#verilog-rtl-generation)
  - [2.2 RTL Design Optimization](#rtl-design-optimization)
  - [2.3 HLS Code Generation](#hls-code-generation)
  - [2.4 Interaction with EDA tools](#interaction-with-eda-tools)
  - [2.5 Detection and Repair of HDL Bugs](#detection-and-repair-of-hdl-bugs)
- [3. LLMs for Hardware Security](#llms-for-hardware-security)
  - [3.1 Fixing of Hardware-Security Bugs](#fixing-of-hardware-security-bugs)
  - [3.2 Generation of Security Properties and Assertions](#generation-of-security-properties-and-assertions)
  - [3.3 Hardware Trojan Insertion](#hardware-trojan-insertion)
  - [3.4 Side Channel Attack Countermeasures](#side-channel-attack-countermeasures)



## [Survey Papers](#content)
- **LLM4EDA: Emerging Progress in Large Language Models for Electronic Design Automation.** arXiv:2401.12224, 2023. [[paper]](https://arxiv.org/pdf/2401.12224.pdf)

    *Ruizhe Zhong, Xingbo Du, Shixiong Kai, Zhentao Tang, Siyuan Xu, Hui-Ling Zhen, Jianye Hao, Qiang Xu, Mingxuan Yuan, Junchi Yan.* 

- **LLM for SoC Security: A Paradigm Shift.** arXiv:2310.06046, 2023. [[paper]](https://arxiv.org/pdf/2310.06046)

    *Dipayan Saha, Shams Tarek, Katayoon Yahyaei, Sujan Kumar Saha, Jingbo Zhou, Mark Tehranipoor, Farimah Farahmandi.*
  
- **Evolutionary Large Language Models for Hardware Security: A Comparative Survey.** arXiv:2404.16651, 2024. [[paper]](https://arxiv.org/pdf/2404.16651)

    *Mohammad Akyash, Hadi Mardani Kamali.*

- **The Dawn of AI-Native EDA: Promises and Challenges of Large Circuit Models.** arXiv:2403.07257, 2024. [[paper]](https://arxiv.org/pdf/2403.07257.pdf)

    *Lei Chen, Yiqi Chen, Zhufei Chu, Wenji Fang, Tsung-Yi Ho, Ru Huang, Yu Huang, Sadaf Khan, Min Li, Xingquan Li, Yu Li, Yun Liang, Jinwei Liu, Yi Liu, Yibo Lin, Guojie Luo, Zhengyuan Shi, Guangyu Sun, Dimitrios Tsaras, Runsheng Wang, Ziyi Wang, Xinming Wei, Zhiyao Xie, Qiang Xu, Chenhao Xue, Junchi Yan, Jun Yang, Bei Yu, Mingxuan Yuan, Evangeline F.Y. Young, Xuan Zeng, Haoyi Zhang, Zuodong Zhang, Yuxiang Zhao, Hui-Ling Zhen, Ziyang Zheng, Binwu Zhu, Keren Zhu, Sunan Zou.*

## [LLM for EDA](#content)
### [Verilog RTL Generation](#content)
- **DAVE: Deriving Automatically Verilog from English.** ACM/IEEE Workshop on Machine Learning for CAD (MLCAD), 2020. [[paper]](https://dl.acm.org/doi/pdf/10.1145/3643681) 

  	*Hammond Pearce, Benjamin Tan, Ramesh Karri.*
  
- **VeriGen: A Large Language Model for Verilog Code Generation.** ACM Transactions on Design Automation of Electronic Systems, 2024. [[paper]](https://dl.acm.org/doi/10.1145/3400302.3415657) [[code]](https://github.com/shailja-thakur/VGen)

  	*Shailja Thakur, Baleegh Ahmad, Hammond Pearce, Benjamin Tan, Brendan Dolan-Gavitt, Ramesh Karri, Siddharth Garg.*

- **VerilogEval: Evaluating Large Language Models for Verilog Code Generation.** IEEE/ACM International Conference on Computer Aided Design (ICCAD), 2023. [[paper]](https://arxiv.org/pdf/2309.07544.pdf) [[code]](https://github.com/NVlabs/verilog-eval)

  	*Mingjie Liu, Nathaniel Pinckney, Brucek Khailany, Haoxing Ren.*

- **RTLCoder: Outperforming GPT-3.5 in Design RTL Generation with Our Open-Source Dataset and Lightweight Solution.** arXiv:2312.08617 (2023). [[paper]](https://arxiv.org/pdf/2312.08617)[[code]](https://github.com/hkust-zhiyao/RTL-Coder)

  	*Shang Liu, Wenji Fang, Yao Lu, Qijun Zhang, Hongce Zhang, Zhiyao Xie.*

- **Chip-Chat: Challenges and Opportunities in Conversational Hardware Design.** ACM/IEEE 5th Workshop on Machine Learning for CAD (MLCAD), 2023. [[paper]](https://arxiv.org/pdf/2312.08617) [[code]](https://zenodo.org/records/7953725)

  	*Jason Blocklove, Siddharth Garg, Ramesh Karri, Hammond Pearce.*

- **AutoChip: Automating HDL Generation Using LLM Feedback.** arXiv:2311.04887, 2023. [[paper]](https://arxiv.org/pdf/2311.04887) [[code]](https://github.com/shailja-thakur/AutoChip)

  	*Shailja Thakur, Jason Blocklove, Hammond Pearce, Benjamin Tan, Siddharth Garg, Ramesh Karri.*

- **RTLLM: An Open-Source Benchmark for Design RTL Generation with Large Language Model.** 29th Asia and South Pacific Design Automation Conference (ASP-DAC), IEEE, 2024. [[paper]](https://ieeexplore.ieee.org/iel7/10473777/10473787/10473904.pdf) [[code]](https://github.com/hkust-zhiyao/RTLLM)

  	*Yao Lu, Shang Liu, Qijun Zhang, Zhiyao Xie.*


### [RTL Design Optimization](#content)
- **ChipGPT: How far are we from natural language hardware design.** arXiv:2305.14019, 2023. [[paper]](https://arxiv.org/pdf/2305.14019)

  	*Kaiyan Chang, Ying Wang, Haimeng Ren, Mengdi Wang, Shengwen Liang, Yinhe Han, Huawei Li, Xiaowei Li.*

- **BetterV: Controlled Verilog Generation with Discriminative Guidance.** arXiv:2402.03375, 2024. [[paper]](https://arxiv.org/pdf/2402.03375)

  	*Zehua Pei, Hui-Ling Zhen, Mingxuan Yuan, Yu Huang, Bei Yu.*

- **Make Every Move Count: LLM-based High-Quality RTL Code Generation Using MCTS.** arXiv:2402.03289, 2024. [[paper]](https://arxiv.org/pdf/2402.03289)

  	*Matthew DeLorenzo, Animesh Basak Chowdhury, Vasudev Gohil, Shailja Thakur, Ramesh Karri, Siddharth Garg, Jeyavijayan Rajendran.*

### [HLS Code Generation](#content)
- **GPT4AIGChip: Towards Next-Generation AI Accelerator Design Automation via Large Language Models.** IEEE/ACM International Conference on Computer Aided Design (ICCAD), 2023. [[paper]](https://ieeexplore.ieee.org/iel7/10323590/10323543/10323953.pdf)
  	
    *Yonggan Fu, Yongan Zhang, Zhongzhi Yu, Sixu Li, Zhifan Ye, Chaojian Li, Cheng Wan, Yingyan (Celine) Lin.*

- **Software/Hardware Co-design for LLM and Its Application for Design Verification (Invited Paper).** 29th Asia and South Pacific Design Automation Conference (ASP-DAC), IEEE, 2024. [[paper]](https://ieeexplore.ieee.org/iel7/10323590/10323543/10323953.pdf) [[code]](https://github.com/UIUC-ChenLab/Chrysalis-HLS)
  	
    *Lily Jiaxin Wan, Yingbing Huang, Yuhong Li, Hanchen Ye, Jinghua Wang, Xiaofan Zhang, Deming Chen.*

### [Interaction with EDA tools](#content)
- **ChipNeMo: Domain-Adapted LLMs for Chip Design.** arXiv:2311.00176, 2023. [[paper]](https://arxiv.org/pdf/2311.00176)
  	
    *Mingjie Liu, Teodor-Dumitru Ene, Robert Kirby, Chris Cheng, Nathaniel Pinckney, Rongjian Liang, Jonah Alben, Himyanshu Anand, Sanmitra Banerjee, Ismet Bayraktaroglu, Bonita Bhaskaran, Bryan Catanzaro, Arjun Chaudhuri, Sharon Clay, Bill Dally, Laura Dang, Parikshit Deshpande, Siddhanth Dhodhi, Sameer Halepete, Eric Hill, Jiashang Hu, Sumit Jain, Ankit Jindal, Brucek Khailany, George Kokai, Kishor Kunal, Xiaowei Li, Charley Lind, Hao Liu, Stuart Oberman, Sujeet Omar, Ghasem Pasandi, Sreedhar Pratty, Jonathan Raiman, Ambar Sarkar, Zhengjiang Shao, Hanfei Sun, Pratik P Suthar, Varun Tej, Walker Turner, Kaizhe Xu, Haoxing Ren.*

- **ChatEDA: A Large Language Model Powered Autonomous Agent for EDA.** IEEE Transactions on Computer-Aided Design of Integrated Circuits and Systems, 2024. [[paper]](https://ieeexplore.ieee.org/iel7/43/6917053/10485372.pdf)
  	
    *Haoyuan Wu, Zhuolun He, Xinyun Zhang, Xufeng Yao, Su Zheng, Haisheng Zheng, Bei Yu.*

### [Detection and Repair of HDL Bugs](#content)
- **RTLFixer: Automatically Fixing RTL Syntax Errors with Large Language Models.** arXiv:2311.16543, 2023. [[paper]](https://arxiv.org/pdf/2311.16543)
  	
    *Yun-Da Tsai, Mingjie Liu, Haoxing Ren.*

- **HDLdebugger: Streamlining HDL debugging with Large Language Models.** arXiv:2403.11671, 2024. [[paper]](https://arxiv.org/pdf/2403.11671)
  	
    *Xufeng Yao, Haoyang Li, Tsz Ho Chan, Wenyi Xiao, Mingxuan Yuan, Yu Huang, Lei Chen, Bei Yu.*

- **LLM4SecHW: Leveraging Domain-Specific Large Language Model for Hardware Debugging.** Asian Hardware Oriented Security and Trust Symposium (AsianHOST), 2024. [[paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10409307) [[code]](https://huggingface.co/datasets/KSU-HW-SEC/LLM4SecHW-OSHD)
  	
    *Weimin Fu, Kaichen Yang, Raj Gautam Dutta‡, Xiaolong Guo, Gang Qu.*

## [LLMs for Hardware Security](#content)
### [Fixing of Hardware-Security Bugs](#content)
- **Examining Zero-Shot Vulnerability Repair with Large Language Models.** IEEE Symposium on Security and Privacy (SP), 2023. [[paper]](https://ieeexplore.ieee.org/iel7/10179215/10179280/10179324.pdf) [[code]](https://drive.google.com/drive/folders/1xJ-z2Wvvg7JSaxfTQdxayXFEmoF3y0ET)
  	
    *Hammond Pearce, Benjamin Tan, Baleegh Ahmad, Ramesh Karri, Brendan Dolan-Gavitt.*

- **Generating Secure Hardware using ChatGPT Resistant to CWEs.** Cryptology ePrint Archive, 2023. [[paper]](https://eprint.iacr.org/2023/212.pdf)
  	
    *Madhav Nair, Rajat Sadhukhan, Debdeep Mukhopadhyay.*

- **On Hardware Security Bug Code Fixes by Prompting Large Language Models.** IEEE Transactions on Information Forensics and Security, 2024. [[paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10462177) [[code]](https://zenodo.org/records/10416865)
  	
    *Baleegh Ahmad, Shailja Thakur, Benjamin Tan, Ramesh Karri, Hammond Pearce.*

### [Generation of Security Properties and Assertions](#content)
- **Unlocking Hardware Security Assurance: The Potential of LLMs.** arXiv:2308.11042, 2023. [[paper]](https://arxiv.org/pdf/2308.11042)
  	
    *Xingyu Meng, Amisha Srivastava, Ayush Arunachalam, Avik Ray, Pedro Henrique Silva, Rafail Psiakis, Yiorgos Makris, Kanad Basu.*

- **DIVAS: An LLM-based End-to-End Framework for SoC Security Analysis and Policy-based Protection.** arXiv:2308.06932, 2023. [[paper]](https://arxiv.org/pdf/2308.06932)
  	
    *Sudipta Paria, Aritra Dasgupta, Swarup Bhunia.*

- **Using LLMs to Facilitate Formal Verification of RTL.** arXiv:2309.09437, 2023. [[paper]](https://arxiv.org/pdf/2309.09437)[[code]](https://github.com/gpt4rtl/AutoSVA2)
  	
    *Marcelo Orenes-Vera, Margaret Martonosi, David Wentzlaff.*

- **(Security) Assertions by Large Language Models.** IEEE Transactions on Information Forensics and Security, 2024. [[paper]](https://ieeexplore.ieee.org/iel7/10206/4358835/10458667.pdf) 
  	
    *Rahul Kande, Hammond Pearce, Benjamin Tan, Brendan Dolan-Gavitt, Shailja Thakur, Ramesh Karri, Jeyavijayan Rajendran.*

- **ChIRAAG: ChatGPT Informed Rapid and Automated Assertion Generation.** arXiv:2402.00093, 2024. [[paper]](https://arxiv.org/pdf/2402.00093)
  	
    *Bhabesh Mali, Karthik Maddala, Sweeya Reddy, Vatsal Gupta, Chandan Karfa, Ramesh Karri.*

- **AssertLLM: Generating and Evaluating Hardware Verification Assertions from Design Specifications via Multi-LLMs.** arXiv:2402.00386 , 2024. [[paper]](https://arxiv.org/pdf/2402.00386) [[code]](https://github.com/hkust-zhiyao/AssertLLM)
  	
    *Wenji Fang, Mengming Li, Min Li, Zhiyuan Yan, Shang Liu, Hongce Zhang, Zhiyao Xie.*

### [Hardware Trojan Insertion](#content)
- **Harnessing the Power of General-Purpose LLMs in Hardware Trojan Design.** 5th Workshop on Artificial Intelligence in Hardware Security, in conjunction with ACNS, 2024. [[paper]](https://angelosk.github.io/Papers/2024/AIHWS2024.pdf)
  	
    *Georgios Kokolakis, Athanasios Moschos, and Angelos D. Keromytis.*

### [Side Channel Attack Countermeasures](#content)
- **Netlist Whisperer: AI and NLP Fight Circuit Leakage!.** Workshop on Attacks and Solutions in Hardware Security, 2023. [[paper]](https://dl.acm.org/doi/pdf/10.1145/3605769.3623989)
  	
    *Madhav Nair, Rajat Sadhukhan, Hammond Pearce, Debdeep Mukhopadhyay, Ramesh Karri.*

- **SCAR: Power Side-Channel Analysis at RTL Level.** IEEE Transactions on Very Large Scale Integration (VLSI) Systems, 2024. [[paper]](https://ieeexplore.ieee.org/iel7/92/4359553/10508974.pdf)
  	
    *Srivastava Amisha, Das Sanjay, Choudhury Navnil, Psiakis Rafail, Silva Pedro Henrique, Pal Debjit, Basu Kanad.*


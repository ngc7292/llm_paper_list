# New AI World's fundamental: Model, Data and Eval.

![25-paper](https://img.shields.io/badge/ModelPaperNumber-25-brightgreen)

In this blog/repo, we collect some paper about fundational model's training methods, architecture, evaluation and training data processing, to find some key point to reproduce the more intelligent and more openful large language model!

(This repo is constantly updated.)

<!--more-->


## Pre-training large language models

This part maintains the paper about how to train a fundational models.

1. **Language Models are Few-Shot Learners** 

   *Tom B. Brown, Benjamin Mann, Nick Ryder, Melanie Subbiah etc.*  from *Openai*  2020.15

   [[pdf](https://arxiv.org/pdf/2005.14165.pdf)] GPT-3

2. **A General Language Assistant as a Laboratory for Alignment** 

   *Amanda Askell, Yuntao Bai, Anna Chen,  Dawn Drain,  Deep Ganguli etc.* from *Anthropic*  2021.12

   [[pdf](https://arxiv.org/pdf/2112.00861.pdf)] Anthropic-LM

3. **Improving language models by retrieving from trillions of tokens**

   *Sebastian Borgeaud ,  Arthur Mensch,  Jordan Hoffmann etc.*  from *deepmind*  2021.12 
   
   [[pdf](https://arxiv.org/pdf/2112.04426.pdf)]  RETRO

4. **Scaling Language Models: Methods, Analysis & Insights from Training Gopher**

   *deepmind* 2021.12
   
   [[pdf](https://arxiv.org/pdf/2112.11446.pdf)] Gopher
   
5. **JURASSIC-1: TECHNICAL DETAILS AND EVALUATION**

   *Opher Lieber, Or Sharir, Barak Lenz, Yoav Shoham* from *AI21 Labs* 2021

   [[pdf](https://uploads-ssl.webflow.com/60fd4503684b466578c0d307/61138924626a6981ee09caf6_jurassic_tech_paper.pdf)] J1-Jumbo
   
6. **LaMDA: Language Models for Dialog Applications**

   *google* 2022.1
   
   [[pdf](https://arxiv.org/pdf/2201.08239.pdf)] LaMDA
   
7. **Using DeepSpeed and Megatron to Train Megatron-Turing NLG 530B, A Large-Scale Generative Language Model**

   *Shaden Smith , Mostofa Patwary etc.* from *Microsoft and Nvidia* 2022.1
   
   [[pdf](https://arxiv.org/pdf/2201.11990.pdf)] MT-NLG
   
8. **Training Compute-Optimal Large Language Models**

   *Jordan Hoffmann,  Sebastian Borgeaud,  Arthur Mensch etc.* from *deepmind* 2022.3
   
   [[pdf](https://arxiv.org/pdf/2203.15556.pdf)] Chinchilla

9. **PaLM: Scaling Language Modeling with Pathways** 

   *google* 2022.4

   [[pdf](https://arxiv.org/pdf/2204.02311.pdf)] PaLM

10. *GPT-NeoX-20B: An Open-Source Autoregressive Language Model*

    *Sid Black, Stella Biderman, Eric Hallahan* in *EleutherAI* 2022.4

    [[pdf](https://arxiv.org/pdf/2204.06745.pdf)] GPT-NeoX-20B

11. **SUPER-NATURALINSTRUCTIONS: Generalization via Declarative Instructions on 1600+ NLP Tasks**

    *Yizhong Wang, Swaroop Mishra* in *Allen AI and Univ of Washington* 2022.4

    [[pdf](https://arxiv.org/pdf/2204.07705.pdf)] Tk-INSTRUCT

12. **OPT: Open Pre-trained Transformer Language Models**

    *Susan Zhang, Stephen Roller, Naman Goyal* in *Meta AI* 2022.5

    [[pdf](https://arxiv.org/pdf/2205.01068.pdf)] OPT

13. **Scaling Instruction-Finetuned Language Models**

    *Hyung Won Chung, Le Hou, Shayne Longpre etc.* in *Google* 2022.10

    [[pdf](https://arxiv.org/pdf/2210.11416.pdf)] Flan-T5

14. **LLaMA: Open and Efficient Foundation Language Models**

    *Hugo Touvron, Thibaut Lavril, Gautier Izacard* in *MetaAI* 2023.2

    [[pdf](https://scontent-hkg4-1.xx.fbcdn.net/v/t39.8562-6/333078981_693988129081760_4712707815225756708_n.pdf?_nc_cat=108&ccb=1-7&_nc_sid=ad8a9d&_nc_ohc=0JlbsRuMCfYAX9WpBiC&_nc_ht=scontent-hkg4-1.xx&oh=00_AfD6f_1ziFoK1HhZiIJ3dE9ECxyipnNjguzEqAWQoVzh9g&oe=63FDD562)] LLaMA

15. **OPT-IML: Scaling Language Model Instruction Meta Learning through the Lens of Generalization**

    *Srinivasan Iyer, Xi Victoria Lin, Ramakanth Pasunuru etc.* in *2022.12*

    [[pdf](https://arxiv.org/pdf/2212.12017.pdf)] OPT-IML

## Pre-training Dataset

1. **The Pile: An 800GB Dataset of Diverse Text for Language Modeling**

   *EleutherAI*
   
   [[pdf](https://arxiv.org/pdf/2101.00027.pdf)]
   
2. **WuDaoCorpora: A super large-scale Chinese corpora for pre-training language models**

   *Beijing Academy of Artificial Intelligence, China*

   [[pdf](https://pdf.sciencedirectassets.com/777606/1-s2.0-S2666651021X00022/1-s2.0-S2666651021000152/main.pdf?X-Amz-Security-Token=IQoJb3JpZ2luX2VjEMv%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEaCXVzLWVhc3QtMSJHMEUCIQCgx948NzjCEOiNRb0ic5RDKecuYPFuIA2k14p6MephTAIgBzAyOUeXFjUTAJwXr0EuJex0y2EmmA5huGVbBh%2BjF6QqswUIcxAFGgwwNTkwMDM1NDY4NjUiDJ%2F04s%2FyM2axraYodyqQBY6g2XBilWfl3rP4%2F%2Bx9L5ESb83ruzT8y1FW6zP3har5tKU2zZ9xEkvNWiRgTwT1vVBLzl9LJkS029kLczFXO9HHBAdWclWAB4yh%2FpvyOy4MlMdtG8Lj1xDnH24buJGm19GIlOmtLMJg3vckk7nX7uYhMjb4m1forGdSIBHqAaBK%2B6g2Gqzoo4cr2NazBpadPLS6OOe1AyVntH1z1v5Kf8vBwEWyObSjuqhC36dSAA3m7JedhUb1OudzL27pFrD%2FDw1%2ForEJKfA4%2FL4sRLBYmZwK4vPUb6NhJmSpcwJ6cR1iyhYNxsgTUq6JHqqj6pTHIy%2FKKfHT4BWwhrieC1GpdOW2aqAC3ca2FYCpgmexomTPMjuZ%2F%2BHeK4afLVQqV5HFLS2Fi%2FvY6T%2FIT1t1NXEYa7KcQt7G1VUzg761Af%2FNqgyKPA8i6ENcLJQMcs7y8yeEuEcZIqluRmqwYDcMedjNOmwoqXyTOW42KglhqL8RKeVJJ3QjQ1YOlCbbgxOXP5C6ccvo6CNDar8PqCXe8FKGcFWJj6kvjmRkH0Fif60FFKPqkzVi9hndMhoez6lFZH1drPjiNUutUFYRYRMwA9FFSyr7qnBgL49FDfdin3zhXRDCIqcG6ahIC5%2Bllt7I%2BWOo%2BVlfbIqf%2BV0WVCoAtng8AmsRIZIgX8qAIO4g%2Bqmv39lHpCdvdrVLgWL5Pk%2FG%2FmB5K5r5xAvGwx6RsGLno8XfrOJTmXepcqNkqVyQ%2Brwuee5ZwZcuwnIEOuReBSTYveECdBTwNXyYib1BDD2Yx8p0XeFnsq%2BHEqNUqsHKw2%2FFx%2FS8G%2BiC5uaJI7ps53bOmv9haxwy3Vbm%2BIVMjHp86%2BJhXHZaLN0ZT3mxTDkWgps%2FdyMQMPul958GOrEB%2FKu1f1Syjnn5gWWnECMxbPphU%2BheIkA7hCzHYDQWSXstdRz1zO8LxtWaNJhgTuLigKoePByi3dn9bPJ3mHqwFl3cPaPcO1ImQbqVFcVu8eWSO3V8t3ysOlwKTORDKlL%2F01bJDY2lqS%2FF3n9QbDBDXROmkgFGE8jBMu9HZApuvMu%2BEU4H%2FUzqE7xZJGtOF6ias2BAOV4QhHfN%2BR7SwTwsLQfoaY8qPxDQgibDLrgfg70Y&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Date=20230228T105054Z&X-Amz-SignedHeaders=host&X-Amz-Expires=300&X-Amz-Credential=ASIAQ3PHCVTY75K4KAHI%2F20230228%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Signature=2923a94fc59500d2c0f34e42336b82710ce8ad6faea2c447b30cd244816590cd&hash=e7f51ffa1321f139fbf6580a8b56287946f16c1e2eca595f3529b9a662d819a1&host=68042c943591013ac2b2430a89b270f6af2c76d8dfd086a07176afe7c76c2c61&pii=S2666651021000152&tid=spdf-dd2690a4-0155-471f-94ea-ad665435b9af&sid=c9927fc84b2ae148b91878c34025033816d0gxrqa&type=client&tsoh=d3d3LnNjaWVuY2VkaXJlY3QuY29t&ua=19085707535d57025e075d&rr=7a089a1a9ed90fc0&cc=cn)]

3. **CCNet: Extracting High Quality Monolingual Datasets from Web Crawl Data**

   *Facebook AI*

   [[pdf](https://aclanthology.org/2020.lrec-1.494.pdf)] [[project](https://github.com/facebookresearch/cc_net)]


## Towards AIGC

This filed will contains the paper of RLHF and other possible way to achieve AIGC.

1. **Training language models to follow instructions with human feedback**

   *Open AI* 2022.3
   
   [[pdf](https://arxiv.org/pdf/2203.02155.pdf)] instruct-GPT
   
2. **Training a Helpful and Harmless Assistant with Reinforcement Learning from Human Feedback**

   *Anthropic* 2022.4
   
   [[pdf](https://arxiv.org/pdf/2204.05862.pdf)] 
   
3. **Training Language Models with Language Feedback**

   *1New York University, 2University of the Basque Country, 3Genentech, 4CIFAR LMB* 2022.4
   
   [[pdf](https://arxiv.org/pdf/2204.14146.pdf)]


## Evaluation

1. **Holistic Evaluation of Language Models**

   *Stanford University*
   
   [[pdf](https://arxiv.org/pdf/2211.09110.pdf)]

2. **A Multitask, Multilingual, Multimodal Evaluation of ChatGPT on Reasoning, Hallucination, and Interactivity**

   *Centre for Artificial Intelligence Research* 

   [[pdf](https://arxiv.org/pdf/2302.04023.pdf)]
   
3. **On the Robustness of ChatGPT: An Adversarial and Out-of-distribution Perspective**

   *1Microsoft Research, 2City University of Hong Kong etc.*

   [[pdf](https://arxiv.org/pdf/2302.12095v1.pdf)]

4. **ON THE PLANNING ABILITIES OF LARGE LANGUAGE MODELS (A CRITICAL INVESTIGATION WITH A PROPOSED BENCHMARK)**

   *Arizona State University, Tempe.* 

   [[pdf](https://arxiv.org/pdf/2302.06706v1.pdf)]







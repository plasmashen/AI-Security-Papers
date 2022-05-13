# <p align="center"> NLP Backdoor

#### Universal Adversarial Triggers for Attacking and Analyzing NLP

*Method*

We propose a gradient-guided search over tokens which finds short trigger sequences (e.g., one word for classification and four words for language modeling) that successfully trigger the target prediction.

作者利用梯度引导搜索，找到较短的 trigger sequence然后这些 trigger 可以使句子被分类到目标类目。
本文使用了 GPT2，ELMo 两个模型，然后他针对的使已经微调好的模型，模型在整个过程中参数使不变的，然后作者的任务是去找这个后门或者说是 trigger


#### BadNL: Backdoor Attacks Against NLP Models 
*Method*

In this paper, we present the first systematic investigation of the backdoor attack against models designed for natural language processing (NLP) tasks. Specifically, we propose three methods to construct triggers in the NLP setting, including Char-level, Word-level, and Sentence-level triggers. Our Attacks achieve an almost perfect success rate without jeopardizing the original model utility. 

本文构造了三种level的后门 trigger 注入方法，字符级，单词级和语句级的 trigger。
本文使用的模型使 LSTM 和 BERT，针对的是微调模型，他们在训练（即微调）阶段的嵌入后门攻击
Natural Backdoor Attack on Text Data 和BadNL的几乎相同，但是本文的完成度还很低，可能是看到BadNL这篇文章发到 arxiv 上了急忙放上来的

#### Weight Poisoning Attacks on Pre-trained Models
*Method*

In this paper, we show that it is possible to construct “weight poisoning” attacks where pre-trained weights are injected with vulnerabilities that expose “backdoors” after fine-tuning, enabling the attacker to manipulate the model prediction simply by injecting an arbitrary keyword.

本文构造了投毒攻击其实就是后门注入，它针对预训练好的模型参数注入了后门，然后该模型经过微调后，攻击者可以通过插入某些关键词使得模型错误分类。
本文使用 BERT 模型，然后他针对的使预训练模型，攻击方法也是训练阶段攻击，属于后门 trigger 注入攻击。


#### BadNets: Identifying Vulnerabilities in the Machine Learning Model Supply Chain

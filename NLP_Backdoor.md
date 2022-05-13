# <p align="center"> NLP Backdoor

#### Universal Adversarial Triggers for Attacking and Analyzing NLP

*Method*

We propose a gradient-guided search over tokens which finds short trigger sequences (e.g., one word for classification and four words for language modeling) that successfully trigger the target prediction.

作者利用梯度引导搜索，找到较短的 trigger sequence然后这些 trigger 可以使句子被分类到目标类目。
本文使用了 GPT2，ELMo 两个模型，然后他针对的使已经微调好的模型，模型在整个过程中参数使不变的，然后作者的任务是去找这个后门或者说是 trigger
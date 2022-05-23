# <p align="center"> Prompt Learning

## Typology of Prompting Methods
*refer to [NLPedia](https://github.com/pfliu-nlp/NLPedia-Pretrain)*

### Pre-traiÍned Models (Detailed Description)

- Left-to-right Language Model
	
	#### [Improving Language Understanding by Generative Pre-Training (GPT)](https://cdn.openai.com/research-covers/language-unsupervised/language_understanding_paper.pdf)
	#### [Language Models are Unsupervised Multitask Learners (GPT-2)](https://cdn.openai.com/better-language-models/language_models_are_unsupervised_multitask_learners.pdf)
	#### [Language Models are Few-Shot Learners (GPT-3)](https://arxiv.org/pdf/2005.14165.pdf)
	
- Masked Language Model

	#### [BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding](https://arxiv.org/pdf/1810.04805.pdf)
	![BERT](img/PL4.png)
	
- Prefix Language Model

	#### [UNILMv2: Pseudo-Masked Language Models for Unified Language Model Pre-Training](https://arxiv.org/pdf/2002.12804.pdf)
	![UniLM2](img/PL2.png)
	
- Encoder-Decoder
	#### [Exploring the Limits of Transfer Learning with a Unified Text-to-Text Transformer](http://arxiv.org/pdf/1910.10683.pdf)
	![T5](img/PL3.png)

![](img/PL1.png)

### Prompt Engineering (Detailed Description)

- Shape
	- Cloze prompt: 
		#### [Language Models as Knowledge Bases?](https://aclanthology.org/D19-1250.pdf)
		<img src="img/PL5.png" width=50% height=50%>
	
	- Prefix prompt: 
		#### [Prefix-Tuning: Optimizing Continuous Prompts for Generation](https://aclanthology.org/2021.acl-long.353.pdf)
		<img src="img/PL6.png" width=49% height=50%>	<img src="img/PL8.png" width=49% height=50%>
		#### [The Power of Scale for Parameter-Efficient Prompt Tuning](https://aclanthology.org/2021.emnlp-main.243.pdf)
		<img src="img/PL7.png" width=50% height=50%>
	
	
- Human Effort
	- Hand-crated
		
		[LAMA](#language-models-as-knowledge-bases)
		[GPT-3](#language-models-are-few-shot-learners-gpt-3)
	- Automated
		- Discrete: 
			#### [AUTOPROMPT: Eliciting Knowledge from Language Models with Automatically Generated Prompts](https://aclanthology.org/2020.emnlp-main.346.pdf)
			![AUTOPROMPT](img/PL9.png)
	
			#### [Universal Adversarial Triggers for Attacking and Analyzing NLP](https://aclanthology.org/D19-1221.pdf)
			<img src="img/PL10.png" width=50% height=50%>
			
		- Continuous: 

			[Prefix-Tuning](#prefix-tuning-optimizing-continuous-prompts-for-generation)
			
			[Prompt Tuning](#the-power-of-scale-for-parameter-efficient-prompt-tuning)

### Answer Engineering (Detailed Description)

- Shape
	- Token: 
		#### [WARP: Word-level Adversarial ReProgramming](https://aclanthology.org/2021.acl-long.381.pdf)
		![WARP](img/PL11.png)
		[LAMA](#language-models-as-knowledge-bases)

	- Span: 
		#### [It’s Not Just Size That Matters: Small Language Models Are Also Few-Shot Learners](https://aclanthology.org/2021.naacl-main.185.pdf)
		
		#### [X-FACTR: Multilingual Factual Knowledge Retrieval from Pretrained Language Models](https://aclanthology.org/2020.emnlp-main.479.pdf)
	- Sentence: 
		[GPT-3](#language-models-are-few-shot-learners-gpt-3)
		[Prefix-Tuning](#prefix-tuning-optimizing-continuous-prompts-for-generation)
- Human Effort
	- Hand-crated: 
		PET-TC
		PET-GLUE
	- Automated
		- Discrete: 
			#### [Making Pre-trained Language Models Better Few-shot Learners](https://aclanthology.org/2021.acl-long.295.pdf)
			![LM-BFF](img/PL12.png)
			
			[AutoPrompt](#autoprompt-eliciting-knowledge-from-language-models-with-automatically-generated-prompts)
			
		- Continuous: 

			[WARP](#warp-word-level-adversarial-reprogramming)
### Multi-Prompt Learning (Detailed Description)

- Prompt Ensemble: 
- Prompt Augmentation: 
- Prompt Composition: 
- Prompt Decomposition: 

### Prompt-based Training Strategies (Detailed Description)

- Parameter Updating
	- Promptless Fine-tuning
	- Tuning-free Prompting: 
	- Fixed-LM Prompt Tuning: 
	- Fixed-prompt LM Tuning: 
	- Prompt+LM Tuning: 
- Training Sample Size
	- Zero-shot: 
	- Few-shot: 
	- Full-data: 
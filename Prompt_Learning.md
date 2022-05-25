# <p align="center"> Prompt Learning

## Typology of Prompting Methods
*refer to [NLPedia](https://github.com/pfliu-nlp/NLPedia-Pretrain)*

### Pre-traiÍned Models (Detailed Description)

- Left-to-right Language Model
	
	[GPT](https://cdn.openai.com/research-covers/language-unsupervised/language_understanding_paper.pdf)
	
	[GPT-2](https://cdn.openai.com/better-language-models/language_models_are_unsupervised_multitask_learners.pdf)
	
	[GPT-3](https://arxiv.org/pdf/2005.14165.pdf)
	
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
		PET-GLUE: PET with Multiple Masks
		
		#### [X-FACTR: Multilingual Factual Knowledge Retrieval from Pretrained Language Models](https://aclanthology.org/2020.emnlp-main.479.pdf)
		<img src="img/PL14.png" width=50% height=50%>
		
	- Sentence: 
		
		[GPT-3](#language-models-are-few-shot-learners-gpt-3)
		
		[Prefix-Tuning](#prefix-tuning-optimizing-continuous-prompts-for-generation)
- Human Effort
	- Hand-crated: 
		#### [Exploiting Cloze Questions for Few Shot Text Classification and Natural Language Inference](https://aclanthology.org/2021.eacl-main.20.pdf)
		<img src="img/PL13.png" width=50% height=50%>
		
		[PET-GLUE](#its-not-just-size-that-matters-small-language-models-are-also-few-shot-learners)
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
		
		[BERT](#bert-pre-training-of-deep-bidirectional-transformers-for-language-understanding)
		
	- Tuning-free Prompting: 

		[GPT-3](#language-models-are-few-shot-learners-gpt-3)
		
	- Fixed-LM Prompt Tuning: 

		[Prefix-Tuning](#prefix-tuning-optimizing-continuous-prompts-for-generation)
		
		[WARP](#warp-word-level-adversarial-reprogramming)

	- Fixed-prompt LM Tuning: 

		[T5](#exploring-the-limits-of-transfer-learning-with-a-unified-text-to-text-transformer)
		
		[PET](#exploiting-cloze-questions-for-few-shot-text-classification-and-natural-language-inference)
		
	- Prompt+LM Tuning: 

		[P-Tuning](https://arxiv.org/pdf/2103.10385.pdf)
		
		#### [PTR: Prompt Tuning with Rules for Text Classification](https://arxiv.org/pdf/2105.11259)
		![PTR](img/PL16.png)

- Training Sample Size
	- Zero-shot: 

		[GPT-3](#language-models-are-few-shot-learners-gpt-3)
		
	- Few-shot: 

		[PET](#exploiting-cloze-questions-for-few-shot-text-classification-and-natural-language-inference)
		
	- Full-data: 
		
		[KnowPrompt](https://arxiv.org/pdf/2104.07650)
		
		
		[PTR](#exploiting-cloze-questions-for-few-shot-text-classification-and-natural-language-inference)
		
		
## Detailed Papers

#### [GPT Understands, Too (P-Tuning)](https://arxiv.org/pdf/2103.10385.pdf)
![P-Tuning](img/PL15.png)

*Challenges*
- Discreteness: random initialized prompt embedding would fall into local minima.
- Association: intuitively, the author believe the values of prompt embedding should be dependent on each other.

*Method*

- P-tuning use pseudo prompts with trainable embedding. 
- To solve discreteness and association, P-tuning use a BiLSTM to generate prompt embedding.
- In the inference, keep only embedding and discard LSTM.


#### [PTR: Prompt Tuning with Rules for Text Classification](https://arxiv.org/pdf/2105.11259.pdf)
![PTR](img/PL17.png)

*Challenges*
- most auto-generated prompts cannot achieve comparable performance to human- picked ones
- auto-generated prompts require extra computation costs for generation and verification

*Method*
- Using three conditional function to determine the subject entity types, the object entity types and the semantic connection between entities.
- Usinh sub-prompts for conditional function.
- Composing sub-prompts for tasks.


#### [KnowPrompt: Knowledge-aware Prompt-tuning with Synergistic Optimization for Relation Extraction](https://arxiv.org/pdf/2104.07650)


#### [Improving Language Understanding by Generative Pre-Training](https://cdn.openai.com/research-covers/language-unsupervised/language_understanding_paper.pdf)

#### [Language Models are Unsupervised Multitask Learners](https://cdn.openai.com/better-language-models/language_models_are_unsupervised_multitask_learners.pdf)

#### [Language Models are Few-Shot Learners](https://arxiv.org/pdf/2005.14165.pdf)
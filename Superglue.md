## GLUE

### Tasks

|Name|Metric|
|-|-|
|The Corpus of Linguistic Acceptability|Matthew's Corr|
|The Stanford Sentiment Treebank|Accuracy|
|Microsoft Research Paraphrase Corpus|F1 / Accuracy|
|Semantic Textual Similarity Benchmark|Pearson-Spearman Corr|
|Quora Question Pairs|F1 / Accuracy|
|MultiNLI Matched|Accuracy|
|MultiNLI Mismatched|Accuracy|
|Question NLI|Accuracy|
|Recognizing Textual Entailment|Accuracy|
|Winograd NLI|Accuracy|
|Diagnostics Main|Matthew's Corr|


### The Corpus of Linguistic Acceptability (CoLA)
The Corpus of Linguistic Acceptability (CoLA) in its full form consists of 10657 sentences from 23 linguistics publications, expertly annotated for acceptability (grammaticality) by their original authors.

### The Stanford Sentiment Treebank (SST)

### Microsoft Research Paraphrase Corpus
a text file containing 5800 pairs of sentences which have been extracted from news sources on the web, along with human annotations indicating whether each pair captures a paraphrase/semantic equivalence relationship. 

### Semantic Textual Similarity Benchmark


### Quora Question Pairs
### MultiNLI Matched
### MultiNLI Mismatched
### Question NLI
### Recognizing Textual Entailment
### Winograd NLI
### Diagnostics Main

## SuperGLUE

### Tasks

|Name|Identifier|Metric|
|:-|:-|-|
|[Broadcoverage Diagnostics](#broadcoverage-diagnostics)|AX-b|Matthew's Corr|
|CommitmentBank|CB|Avg. F1 / Accuracy|
|Choice of Plausible Alternatives|COPA|Accuracy|
|Multi-Sentence Reading Comprehension|MultiRC|F1a / EM|
|Recognizing Textual Entailment|RTE|Accuracy|
|Words in Context|WiC|Accuracy|
|The Winograd Schema Challenge|WSC|Accuracy|
|BoolQ|BoolQ|Accuracy|
|Reading Comprehension with Commonsense Reasoning|ReCoRD|F1 / Accuracy|
|Winogender Schema Diagnostics|AX-g|Gender Parity / Accuracy|


### Broadcoverage Diagnostics
This dataset evaluates sentence understanding through Natural Language Inference (NLI) problems. 

The data is distributed in .tsv format with the following columns:

0. ~~Lexical Semantics (Lexical Entailment, Morphological Negation, Factivity, Symmetry/Collectivity, Redundancy, Named Entities, Quantifiers)~~
1. ~~Predicate-Argument Structure~~
2. ~~Logic~~
3. ~~Knowledge & Common Sense~~
4. Domain (News, Reddit, Wikipedia, ACL, or Artificial)
5. Premise
6. Hypothesis
7. Label (entailment, contradiction, or neutral)


### CommitmentBank (CB)
The CommitmentBank is a corpus of 1,200 naturally occurring discourses whose final sentence contains a clause-embedding predicate under an entailment canceling operator.
("premise", "hypothesis")

### Choice of Plausible Alternatives (COPA)
Each question is composed of a premise and two alternatives, where the task is to select the alternative that more plausibly has a causal relation with the premise.
 
*Examples*

Premise: The man broke his toe. What was the CAUSE of this?
Alternative 1: He got a hole in his sock. 
Alternative 2: He dropped a hammer on his foot.

### Multi-Sentence Reading Comprehension

MultiRC (Multi-Sentence Reading Comprehension) is a dataset of short paragraphs and multi-sentence questions, i.e., questions that can be answered by combining information from multiple sentences of the paragraph. The dataset was designed with three key challenges in mind: * The number of correct answer-options for each question is not pre-specified. This removes the over-reliance on answer-options and forces them to decide on the correctness of each candidate answer independently of others. In other words, the task is not to simply identify the best answer-option, but to evaluate the correctness of each answer-option individually. * The correct answer(s) is not required to be a span in the text. * The paragraphs in the dataset have diverse provenance by being extracted from 7 different domains such as news, fiction, historical text etc., and hence are expected to be more diverse in their contents as compared to single-domain datasets. The entire corpus consists of around 10K questions (including about 6K multiple-sentence questions). 

### Recognizing Textual Entailment

This task requires to recognize, given two text fragments, whether the meaning of one text is entailed (can be inferred) from the other text.

### Words in Context

A system's task on the WiC dataset is to identify the intended meaning of words. WiC is framed as a binary classification task. Each instance in WiC has a target word w, either a verb or a noun, for which two contexts are provided. Each of these contexts triggers a specific meaning of w. The task is to identify if the occurrences of w in the two contexts correspond to the same meaning or not. In fact, the dataset can also be viewed as an application of Word Sense Disambiguation in practice.

|Label	|Target	|Context-1	|Context-2|
|:-:|:-:|-|-|
|F	|bed	|There's a lot of trash on the bed of the river	|I keep a glass of water next to my bed when I sleep|
|T	|beat	|We beat the competition	|Agassi beat Becker in the tennis championship|
### The Winograd Schema Challenge

A Winograd schema is a pair of sentences that differ in only one or two words and that contain an ambiguity that is resolved in opposite ways in the two sentences and requires the use of world knowledge and reasoning for its resolution. 

    {“text": "I tried to paint a picture of an orchard, with lemons in the lemon trees , but they came out looking more like light bulbs.", "target": {"span2_index": 17, "span1_index": 13, "span1_text": "lemon trees", "span2_text": "they"}, "idx": 2, "label": false}
### BoolQ

BoolQ is a question answering dataset for yes/no questions containing 15942 examples. These questions are naturally occurring ---they are generated in unprompted and unconstrained settings.

Each example is a triplet of (question, passage, answer), with the title of the page as optional additional context. The text-pair classification setup is similar to existing natural language inference tasks.

    {
    "question": "is france the same timezone as the uk",
    "passage": "At the Liberation of France in the summer of 1944, Metropolitan France kept GMT+2 as it was the time then used by the Allies (British Double Summer Time). In the winter of 1944--1945, Metropolitan France switched to GMT+1, same as in the United Kingdom, and switched again to GMT+2 in April 1945 like its British ally. In September 1945, Metropolitan France returned to GMT+1 (pre-war summer time), which the British had already done in July 1945. Metropolitan France was officially scheduled to return to GMT+0 on November 18, 1945 (the British returned to GMT+0 in on October 7, 1945), but the French government canceled the decision on November 5, 1945, and GMT+1 has since then remained the official time of Metropolitan France.",
    "answer": false,
    "title": "Time in France",
    }

### Reading Comprehension with Commonsense Reasoning

Reading Comprehension with Commonsense Reasoning Dataset (ReCoRD) is a large-scale reading comprehension dataset which requires commonsense reasoning. ReCoRD consists of queries automatically generated from CNN/Daily Mail news articles; the answer to each query is a text span from a summarizing passage of the corresponding news. The goal of ReCoRD is to evaluate a machine's ability of commonsense reasoning in reading comprehension. ReCoRD is pronounced as [ˈrɛkərd].


### Winogender Schema Diagnostics

Winogender Schemas (inspired by Winograd Schemas) are minimal pairs of sentences that differ only by the gender of one pronoun in the sentence, designed to test for the presence of gender bias in automated coreference resolution systems.

1. The nurse notified the patient that...
	- her shift would be ending in an hour.
	- his shift would be ending in an hour.
	- their shift would be ending in an hour.
2. The nurse notified the patient that...
	- her blood would be drawn in an hour.
	- his blood would be drawn in an hour.
	- their blood would be drawn in an hour.

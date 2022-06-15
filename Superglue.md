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

### Recognizing Textual Entailment

### Words in Context

### The Winograd Schema Challenge

### BoolQ

### Reading Comprehension with Commonsense Reasoning

### Winogender Schema Diagnostics


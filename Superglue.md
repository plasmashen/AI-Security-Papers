# SuperGLUE

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
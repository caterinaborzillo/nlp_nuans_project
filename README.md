# Use of a QA-based method for the comparison of two (or more) Text Summarization models

NUANS (Natural Language Processing) project on the implementation of a solution for an NLP task.

## Details
The aim of this project is to use a Question Answering model to compare two (or more) Text Summarization models. That’s because in recent years NLP evaluation metrics such BLEU or ROUGE have been shown to be inappropriate with regard to the evaluation of machine-made summaries, both for the purely syntactic assessment and the length of the output that they have to measure. For this purpose, I implemented a two-stage method that is able, given a summary, to answer human-annotated questions; the basic idea is that if the model succeeds in answering the questions correctly, it means that the model-generated summary is an high-quality summary since it contains the most important information, and vice versa. 

- nlp_project.ipynb: .ipynb file containing the code solution for the NLP task
- project_report.pdf: a .pdf file with the detailed description of the implemented solution along with the final results 

## Dataset
Narrative QA dataset [^1]

## Language, libraries and frameworks
Python, pytorch, Hugging Face Transformers, spaCy

## Models and summarization tools
BM25Okapi, PreTrainedTokenizer, T5ForConditionalGeneration, SBertSummarizer, GPT2 Transformer

[^1]: Tomáš Kočiský, Jonathan Schwarz, Phil Blunsom, Chris Dyer, Karl Moritz Hermann, Gábor Melis, and Edward Grefenstette. 2017. The narrative qa reading comprehension challenge.
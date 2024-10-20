# Negation
## Deep Learning - Final Project
###Buket Sak, *Ludmila Bajuk* , Kascha Kruschwitz
##CLASSIFYING NEGATION
For this project, we decided to work on negation since it is know to be a difficult aspect of natural language to process. Negation is very complex and it comes in different ways in language, in the form of lexical, (such as antonyms or opposites), semantic negation (contradiction and neative particles) clause negation (not- and no-negation), and many other forms. Exactly this, and the difference in syntactic structures when negation is used are some of the features that make negation difficult to implement, generate and classify for models.

To tackle this phenomena, we decided to use three different approaches. In order to have "benchmark" that could actually tell us that language models have difficulties when identifying, classifying and generating negation, we few-shoted GPT2 (EleutherAI/gpt-neo-1.3B) using examples taken manually from the dataset to evaluate its performance. After observing that clearly, at a first very simple approach language models struggle with negation, we decided to explore a bit more. First, we fine-tuned one already pre-trained model (bert-base-en-uncased) and adapt it to be a classifier that differentiates between negated and non-negated pairs of sentences. Secondly, we create BERT embeddings and fed to another model (BertBackbone) we created. Finally, we created a third model with different layers and other parameters, to manage this phenomena in diverse approaches.

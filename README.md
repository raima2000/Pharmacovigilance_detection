# Pharmacovigilance_detection
Detection of Adverse drug reactions from clinical text data and classifying them into ADR and non-ADR using Transformer models.

This is my final year Masters degree project. Advancements in pharmaceutical science have incorporated various technologies to prevent and revolutionize the treatment of diseases varying from mild ones to fatal cases.  One such break with the past is in the identification of drug-related events and actions. This project aims to harvest information that can be employed to ascertain if a medication is leading to adverse effects in its consumers or patients. We have used NLP methods that transform text data or corpus into formats that are understandable by machines and hence the machines can be trained to find any inimical events in people due to the medicinal drug consumption. In this paper, we intend to classify the texts into ADR and Non-ADR based on adverse events in each text. We have implemented four models - BERT, DistillBERT, BioBERT, and RoBERTa to analyze how Transformer Models work differently in the given problem statement and came to the conclusion that RoBERTa outperforms all other techniques.

Bert stands for Bi-directional encoder representations from transformers which was introduced by Google AI in 2018 to enhance and improve NLP tasks. It's a pre-trained model that is trained on a large corpus of text data including Wikipedia articles. BERT's pre-trained representations can be transferred to a wide range of downstream NLP tasks, reducing the need for task-specific feature engineering and often achieving state-of-the-art results with minimal task-specific data.

We have used the distilBERT architecture, which is a lighter and compressed version of BERT designed for efficient text classification tasks and typically has around forty per cent fewer parameters. It is the objective of this exploratory approach is to classify textual data into critical categories of ADRs (Adverse Drug Reaction) and NON-ADR. The efficient exploitation of the distilBERT tokenizer and model is at the centre of this model. 

A state-of-the-art NLP model, RoBERTa, or "A Robustly Optimised BERT Pretraining Approach," builds on the success of BERT while integrating numerous significant adjustments to improve its performance. As the foundation of our methodology in this study, we used the RoBERTa architecture, a cutting-edge transformer-based model, to categorize textual data into two separate groups: Adverse Drug Reactions (ADR) and Non-ADR. 

A specialized language representation model created specifically for the biomedical and clinical area is called BioBERT, or Biomedical BERT. Although it is specifically designed for large-scale biomedical corpora, such as content from PubMed and other sources of biomedical literature, it is built upon the fundamental BERT (Bidirectional Encoder Representations from Transformers) architecture. This specialty training gives BioBERT a thorough understanding of the special terminology, vocabulary, and grammatical constructions used in biomedical literature. BioBERT is particularly useful for tasks like named entity recognition, relation extraction, and information extraction in the biomedical field thanks to its understanding of biological and medical jargon.

**DATASET**-The dataset we used is the psyTAR Dataset which stands for “Psychiatric Treatment Adverse Reaction”. This dataset comprises feedback from patients regarding the efficacy and negative effects of psychiatric medications. The creation of the dataset started with the collection of 891 drug reviews from patients who posted on the “askpatient.com” online healthcare forum. The reviews specifically pertain to four psychiatric drugs: Zoloft, Lexapro, Cymbalta, and Effexor XR. Each drug review contains details about the patient’s demographics, treatment period, and level of contentment with the respective drug. The data amounted to a total of 891 records.  The ADE containing sub-corpus had 709 records and the ADE negative sentences contained 59 records.

The approach taken in this paper is binary classification that we classify the comment into Adverse Drug Reaction and Non Adverse Drug Reaction. Through our research journey we have reached a major discovery in text classification for adverse drug reaction detection: RoBERTa stands out amongst all transformer models as an exact and efficient model to classify ADE. We have produced excellent results in our rigorous research and comparative analysis of the transformer-based models, including BERT, BioBERT and DistilBERT. In the accurate identification of ADR mentions in clinical and biomedical text, RoBERTa demonstrated exceptional skill with its advanced architecture and pre trained knowledge. The detailed proceedure and results is given shown in the colab notebooks.

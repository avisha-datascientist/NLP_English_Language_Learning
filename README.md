# NLP_English_Language_Learning

- **Goal and Overview**: The goal is to evaluate the language proficiency of 8th-12th grade English Language Learners (ELLs). This evaluation will be based on a dataset of essays written by ELLs, and the aim is to develop proficiency models that can offer more accurate feedback to students and expedite the grading process for teachers.
- **Dataset**:  This dataset, known as the ELLIPSE corpus, consists of argumentative essays which have been assessed using six analytical criteria: cohesion, syntax, vocabulary, phraseology, grammar, and conventions. Each of these criteria reflects a specific aspect of essay writing proficiency, where higher scores indicate a higher level of proficiency in that particular aspect. The scoring system ranges from 1.0 to 5.0, with increments of 0.5. Your task in this competition is to predict the scores for each of these six measures for the essays provided in the test set. https://www.kaggle.com/competitions/feedback-prize-english-language-learning/data
- **Notebook**: I have first performed in depth EDA. For modeling I have made use of non fine tuned pre trained embeddings from **DeBERTa Large**, **DeBERTa V3 base**, **DeBERTa v3 Large**, **Big Bird** and **Funnel** transformers. Dimensionality reduction of these embeddings is performed using PCA. Moreover, a multioutput regression is added as the head of the model which is fed with embeddings and features to output a score. 






# BA2-final-paper-data
final paper data 
Project description, RQ, headline finding, instructions to reproduce
Prject description 
This project uses Latent Direchlet Allocation (LDA) topic modelling to analyse a corpus of 615 Korean poems from five poets who lived during the Japanese colonial period. The goal is to identify recurring themes and determine whether computional text analysis can distinguish differences in thematic focus between poets. The poems were preproccessed by tokenishing the Korean text, retaining the nouns, removing stopwords and filtering rare and overly common terms before applying LDA topic modeling. 

Reseach Question
To what extent can Latent Dirichlet Allocation (LDA) reveal differences in thematic focus among the five Korean poets from the Japanese colonial period? 

Headline Finding
LDA was moderately successful in identifying thematic differences between poets. some topics were strongly associated with specific poets, such as:
1. Topic 2 being most prevalant in poems from Han Yong-un.
2. Topic 1 being most prevalant in poems from Kim So-wol.
At the same time several topics were shared over multible poets suggesting a more common theme of the colonial period such as identity, family and nature. The result shows that there are both broader thematic similarities aswell as distinctive author preferences within the corpus.

Instructions to reproduce
View pipeline.svg for orange data mining widget pipeline. 
make sure You have the "text" add on in Orange data mining. 
1. load the kpoem_sample CSV dataset(615 poems) in to the corpus
2. clean the text using the python script in repo: custom_preprocessing_Kpoet.py
3. import the Processed text into Orange through the corpus widget.
4. apply additional stopwords with the preprocess widget, from repo upload: stopwords_ko
5. Run the Topic Modelling widget using LDA with 8 topics.
6. Analyse the results Using the widgets:
   - LDAvis
   - t-SNE + Corpus Viewer
   - Data Table
7. interpret the generated topics and compare topic prevalence across poets using the topic persentages and t-SNE visualisation.


   

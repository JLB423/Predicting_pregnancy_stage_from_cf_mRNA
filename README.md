# Predicting_pregnancy_stage_from_cf_mRNA

The dataset from the study titled, "Microarray Data of cell-free RNA across pregnancy time course" (Koh et
al., 2014) was downloaded from NCBI GEO database. The dataset includes cell-free RNA expression of 12
patients (including a non-pregnant control) over 3 trimesters and post-partum. 33,297 transcripts are
measured in the dataset. By analyzing the expression and presence of cf-RNA in the blood, an overview of
tissue development and overall health of a fetus can be determined (2014). This study aimed to provide a
non-invasive technique for examining fetal tissue development.

Our goal with this dataset is to determine what trimester a patient is in given the expression levels. From
this analysis, we are hoping to find which transcript has the highest differential expression during the final
stages of pregnancy. Using various Machine Learning models to classify the data to learn and understand
how and when these transcripts are expressed, and what up-regulate genes they code for during
pregnancy.

Most models performed at nearly 100% accuracy when predicting between class 3 and class 4 (3rd
trimester vs postpartem). It is important to note that model parameter tuning is an important part of
creating any machine learning models. All datasets will require different model tuning and therefore it is
often not known which model and which parameters will be the best choice. Thus, it is important to
experiment with running different models and to utilize methods like grid search to find the best parameter
for a given model.

All of the models that we ran on our final dataset can be useful for determining the expected expression
levels for patients at later stages of pregnancy vs patients who are not pregnant. Note that the postpartem
samples represent a baseline level due to the immediate drop in fetal cfRNA after delivery. These models
can also be used to train the expected levels during early pregnancy and middle pregnancy as well, and
then could be used to predict if a woman is pregnant and at which stage she is in. More data processing
would need to be done first to determine the top differentiated genes in each of those stages to see if the
fluctuate during different stages of pregnancy.

The models could then be adjusted and potentially used to determine the health of the fetus based on the
expected level of transcript expression vs the acutal level for an individual at a specific point and time
during her pregnancy.

References: Koh W, Pan W, Gawad C, Fan HC et al. Noninvasive in vivo monitoring of tissue-specific global gene
expression in humans. Proc Natl Acad Sci U S A 2014 May 20;111(20):7361-6. PMID: 24799715

# csci451-project

##Abstract

Deep learning image classification models have shown promise in identifying diseases through Chest X-rays. However, a series of results have also shown that with considerable accuracy, it is possible to determine the self-reported ethnicity of the patient. We aim to reproduce these results and outline the ethical concerns this poses both in terms of phrenology and the privacy of the patient.

##Motivation and Question

We aim to use the publicly available ChexPert (https://stanfordmlgroup.github.io/competitions/chexpert/) database, which consists of 224,316 chest radiographs of 65,240 patients from Stanford Hospital, collected between October 2002 and July 2017. The data is mainly intended for classifying a variety of chest diseases, for which radiologists have provided separate annotations. This includes the self-reported age, gender, and ethnicity of the patient.

However, papers as "AI recognition of patient race in medical imaging: a modelling study" by Gichoya et. al (https://www.thelancet.com/journals/landig/article/PIIS2589-7500(22)00063-2/fulltext) have used the Chexpert dataset (along with other public and private chest radiographs) to accurately determine the self-reported age, gender, and ethnicity of the patient. That ethnicity can be detected is especially concerning as it may indicate that ML models for medical imaging classification can use race to make predictions. As they note, this could perpetuate existing inequalities in medical care for minority groups.

We want to see if it is possible to reproduce their results for ethnicity classification. The data they use, unsurprisingly, is a majority White, so we want to investigate whether our algorithm shows any bias in its classifications.

We also want to investigate the ethical concerns with creating an algorithm that can identify the race of the patient. For one, we want to discuss its implications for other medical imaging algorithms. Furthermore, a concern is that it may support racial determinism, the belief that race is a key factor in ones phenotypic abilities. To this end, we will discuss the paper's own investigations into the reasons why the algorithm can detect race as well as finding other papers on the impacts of racial determinism. Another concern we may investigate is de-anonymization. While we will not try to de-anonymize the data, it may be worthwhile discussing the impacts that having this information on age, gender, and ethnicity can have on revealing a patient's identity.


## Planned Deliverables

We plan to create a model that can predict a person's race based on the image of their chest X-ray. We will also include a Jupyter notebook that demonstrates the efficacy of this model.

If everything works out as planned, we will have a great predictive model and a beautiful analysis of its efficacy in a Jupyter notebook. We will also have a chance to analyze the factors that contribute to the model's accuracy; we can look at the most interesting features and the potential biases that may be present in the data. We can start to think about how this model can be used (ethically) in a clinical setting (does this help with diagnosis at all? etc.).

If things don't 100% work out, we at least tried and I think that's great. Our deliverables will be a Python package and a Jupyter notebook explaining exactly why we fail: there may not be enough data; the rib cages of people from different ethnic backgrounds may not look very different (we may need to look for research papers on this); etc. We can also badmouth the model in this Jupyter notebook to justify that failing may actually be a good thing (the model can become evil if it falls into the wrong hands, etc.).

## Resources Required

We need chest X-ray datasets that include the race of the patient. Right now we're considering using data from [here](https://stanfordaimi.azurewebsites.net/datasets/192ada7c-4d43-466e-b8bb-b81992bb80cf). This has a .csv file with race labels for the patients in study 1. We're still looking for more data because knowledge is power.

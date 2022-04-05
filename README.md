# Identifying-Entities-in-Healthcare-Data

‘BeHealthy’ has a web platform that allows doctors to list their services and manage patient interactions and provides services for patients such as booking interactions with doctors and ordering medicines online. Here, doctors can easily organise appointments, track past medical records and provide e-prescriptions.

 

So, companies like ‘BeHealthy’ are providing medical services, prescriptions and online consultations and generating huge data day by day.

 

Let’s take a look at the following snippet of medical data that may be generated when a doctor is writing notes to his/her patient or as a review of a therapy that he or she has done.

 

“The patient was a 62-year-old man with squamous cell lung cancer, which was first successfully treated by a combination of radiation therapy and chemotherapy.”

 

As you can see in this text, a person with a non-medical background cannot understand the various medical terms. We have taken a simple sentence from a medical data set to understand the problem and where you can understand the terms ‘cancer’ and ‘chemotherapy’. 

 

Suppose you have been given such a data set in which a lot of text is written related to the medical domain. As you can see in the dataset, there are a lot of diseases that can be mentioned in the entire dataset and their related treatments are also mentioned implicitly in the text, which you saw in the aforementioned example that the disease mentioned is cancer and its treatment can be identified as chemotherapy using the sentence.

 

But, note that it is not explicitly mentioned in the dataset about the diseases and their treatment, but somehow, you can build an algorithm to map the diseases and their respective treatment.

 

Suppose you have been asked to determine the disease name and its probable treatment from the dataset and list it out in the form of a table or a dictionary like this.

 ![alt text](https://github.com/sambisht8/Identifying-Entities-in-Healthcare-Data/blob/main/0891d77b-b9ca-4e9d-8934-d9a9b078a51c-syntactic%20sol%20pic1.png?raw=true)

 
After discussing the problem given above, you need to build a custom NER to get the list of diseases and their treatment from the dataset.

In this assignment, you need to perform the following broad steps:

    You need to process and modify the data into sentence format. This step has to be done for the 'train_sent' and ‘train_label’ datasets and for test    datasets as well.
    After that, you need to define the features to build the CRF model.
    Then, you need to apply these features in each sentence of the train and the test dataset to get the feature values.
    Once the features are computed, you need to define the target variable and then build the CRF model.
    Then, you need to perform the evaluation using a test data set.
    After that, you need to create a dictionary in which diseases are keys and treatments are values.

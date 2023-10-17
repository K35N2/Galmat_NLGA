# Galmat_NLGA
Code for Task 3 of the GALMAT Honours project (2023) at UCT

PROJECT TITLE: Generating Adaptive Learning Materials (GALMAT) - Task 3

---------DESCRIPTION AND OVERVIEW---------

This task of the GALMAT project produces the final output of the project, an informative document containing verbalisations of triples provided within the learner knowledge model. 3 Large Language Models are tested and then evaluated. This readMe will provide a guide on how to run the scripts to replicate our results.

---------SCRIPT DETAILS---------

There are 6 scripts in total for this task:

GPT2_prompt: Prompts (in a zero-shot setting) a base, medium-sized GPT-2 model.

fine_tuning_GPT2: Fine-tunes a medium-sized GPT-2 model using a custom dataset and infers from that model.

create_data.py: Extracts information from the WebNLG dataset and creates the custom dataset used to fine-tune the GPT-2 model. The food domain in WebNLG v2.1 dataset is originally in XML format and was converted into the JSON format using JSONconvert.py, which is based on XML corpus reader by Anastasia Shimorina (Also available in Google Drive).

Prompt_BLOOM: Loads the BLOOM (6 billion parameter version) model and prompts it in the zero-shot and few-shot setting

PromptOpenAI: Uses the openAI API to infer from the base GPT-3 model.

Evaluation: Uses the outputs from the models and reference sentences to generate SacreBLEU, ROUGE-L and METEOR scores.

NOTE: TO TEST THE GPT-2 AND BLOOM MODEL, A GPU IS REQUIRED. ALL THE SCRIPTS WERE WRITTEN ON GOOGLE COLAB TO GAIN ACCESS TO THAT. IT IS RECOMMENDED THAT THEY ARE RUN ON GOOGLE COLABORATORY INSTEAD OF A LOCAL SYSTEM.

---------SCRIPT ACCESS AND USAGE---------

All the scripts were saved on Google Drive. Below is the email-address and password for accessing them and running them on Google Colaboratory. The drive also have the files used as input or to make the inputs and the outputs we obtained:

E-mail address: ************************
Password: **********************

Should the scripts be run on a local machine, make sure it has a supported GPU and that the paths used in the scripts have been changed to local and valid ones. The requirements.txt file contains a list of all the libraries that need to be installed for the scripts to work.


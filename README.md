# DMTS2021
UCL MSc Project

Code for UCL Masters Project: Can neural networks match the abilities of honey bees in the delayed match to sample visual reasoning task?

The code from a previous dissertation by Orestis Bastas:

https://github.com/ob00042/ucl_thesis_19

was used as the foundation for the project of the repository.

This Githib repository contains only the code for this current project. A more comprehensive collection of project resources including all the code, data and results can be found within the following shared Google Drive folder, however, it will probably identify me so it is probably best just to use the code here for anonymous marking. I included the Google Drive folder link because there was not the time to upload all the data to Github, but the submision guidelines only asked for the code anyway. The Google Drive folder is here:

https://drive.google.com/drive/folders/1o7ATIeChlZhhmVjMcD7z3tfQVkg8NmKK?usp=sharing

With its own README:

https://docs.google.com/document/d/1I6siys_Y_ePTC4Yj8_UdWMRMjPTQjx12M1vPWBXlRpc/edit?usp=sharing

The first notebooks concern data generation and within those notebooks can be found more on the location of the different datasets stored within the Google Drive folder.

During the writeup the names of the experiments and datasets were changed for the sake of clarity, but this is not currently reflected in the code.

Set B in the code is now set A in the write up
Set A in the code is now set B in the write up
Experiment 3’s held out angles set is now set C in the write up

Experiment 1 in the code is now experiment A in the writeup
Experiment 2 in the code is now experiment B in the writeup
Experiment 3 in the code is now experiment C in the writeup

The data generation code can be found in **0_data_generation.ipynb**.

Additional data generation for the CIFAR-100 based DMTS examples can be found in **0_CIFAR_DMTS_example_generator.ipynb**.

Experiment A is split between:

**1a_experiment_a_col_noise.ipynb** covering experiments A1 and A5.
**1b_experiment_a_bw_noise.ipynb** covering experiments A2 and A6.
**1c_experiment_a_col_no_noise.ipynb** covering experiments A3 and A7.
**1d_experiment_a_bw_no_noise.ipynb** covering experiments A4 and A8.
**1e_experiment_a_col_noise_sample_exchanging.ipynb** covering experiments A9 and A10.

Experiment B pretraining is covered in **2_experiment_b_pretraining.ipynb**.

Experiment B fine tuning is split between
**3a1_experiment_b1_finetuning_with_pretrained_DMTS_col_noise.ipynb** covering experiments A1 and A5 after DMTS-maze pretraining. 
**3a2_experiment_b2_finetuning_with_pretrained_ymaze_col_noise.ipynb** covering experiments A1 and A5 after y-maze pretraining. 
**3a3_experiment_b3_finetuning_with_pretrained_1maze_col_noise.ipynb** covering experiments A1 and A5 after 1-maze pretraining.
**3b3_experiment_b3_finetuning_with_pretrained_1maze_bw_noise.ipynb** covering experiments A2 and A6 after 1-maze pretraining. 
**3c3_experiment_b3_finetuning_with_pretrained_1maze_col_no_noise.ipynb** covering experiments A3 and A7 after 1-maze pretraining. 
**3d3_experiment_b3_finetuning_with_pretrained_1maze_bw_no_noise.ipynb** covering experiments A4 and A8 after 1-maze pretraining. 
**3e3_experiment_b3_finetuning_with_pretrained_1maze_col_noise_sample_exchanging.ipynb** covering experiments A9 and A10 after 1-maze pretraining. 

Experiment C is covered in **4_experiment_c.ipynb**
And the experiment A models used were generated within the **4_experiment_c_models_from_experiment_a** folder: 

Extension 1 is in **5_extension_1.ipynb**

Extension 2 is in **5_extension_1.ipynb**

Extension 3 is in **5_extension_1.ipynb**

Extensions 4 and 5 are in **5_extension_4_5.ipynb** which use code stored in **5_maml_code** and data stored in **5_maml_data** (in Google Drive, but not on Github). The data should be downloaded and then re-uploaded to Colab as instructed in the notebook for faster processing, rather than accessed from Google Drive. Note, this data consists of single images which are then compiled into DMTS sequences by the code, rather than starting as pre-made DMTS sequences as in the datasets for experiments A, B and C. This is again for speed when sampling tasks in MAML and speed of upload to Colab.

Some of the plots used in the study were generated in **6_summary_plots**.

The statistical comparison test examples can be found in **stats_tests.ipynb**.

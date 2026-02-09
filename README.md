# Generative-VQA-Using-BLIP_2
Generative Multimodal Visual Question Answering using BLIP-2

# Project Overview

Visual Question Answering (VQA) is a multimodal task that combines computer vision and natural language processing to answer questions about images. Traditional VQA systems often rely on fixed answer sets, limiting their flexibility and real-world applicability. This project implements a generative VQA system using the BLIP-2 (Bootstrapped Language–Image Pretraining) multimodalarchitecture. The model is capable of producing open-ended, natural language answers based on both the image content and the input question, making it more suitable for real-world scenarios. The model was fine-tuned on the VQAv2 dataset and saved as a PyTorch checkpoint (.pt).
This repository containes 
1. requirements.txt: All the required libaries and their version
2. VQA_EDA.ipynb: EDA done on 10k samples
3. BLIP-2 VQA.ipynb: Loading and training of the model and save .pt file
4. BLIP-2 Evaluation using pt.ipynb: Evaluation of model using .pt file and also shows the working of the .pt file
5. vqa_2000_results.csv: Results of evaluation on 2000 test samples
6. Multimodal Visual Question Answering Using BLIP-2.pptx: Presentaton slides of the project


# Objective

• To use a pre-trained model BLIP-2 on the VQAv2 dataset for generative question answering. 
• To compare the proposed approach with traditional VQA approach where vocabulary is fixed. 
• To evaluate the quantitative and qualitative performance of the generative VQA model. 
• To evaluate the strengths and weaknesses of the transfer learning in multimodal VQA in pretrained model.

# BLIP-2 Model Used

Salesforce/blip2-opt-2.7b" from huggingface

# Architecture
Frozen Vision Transformer (ViT)
Q-Former for vision-language alignment
Frozen Large Language Model (OPT)

# Dataset:

VQAv2 (https://visualqa.org/)

# Ready to use model

link for .pt file: https://drive.google.com/file/d/16dC31OxdtSR_0p9pgCoa90BNjgMyYhj0/view?usp=sharing
I have also shared a file named BLIP-2 Evaluation using pt.ipynb to show the  evaluation of model and working of .pt file.

# .csv file

The uploaded .csv file named vqa_2000_results.csv contsins the predictions made on 2000 samples of test data. It includes natural language question, ground truth (or real answer), predicted answer and VQA accuracy. Some of the samples have 1 VQA accuracy meaning predicted question is correct. some of them have partial like 0.33 or 0.66 meaning some of them are partially correct and some have 0 meaning the predicted answer is completely incorrect.

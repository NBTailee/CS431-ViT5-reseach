# Conducted By Le Duc Tai (NBTailee)
# CS431-ViT5-research 
- A pretrained Transformer-based encoder-decoder model for the Vietnamese language. With T5-style self-supervised pretraining, ViT5 is trained on a large corpus of high-quality and diverse Vietnamese texts. We benchmark ViT5 on two downstream text generation tasks, Abstractive Text Summarization and Named Entity Recognition. All the experiments are shown in paper ViT5: Pretrained Text-to-Text Transformer for Vietnamese Language Generation.

## Resources
- Dataset **Wikilingua** from **HuggingFace**
- Computational resource **GPU P100** from **Kaggle**
## System settings
- All base size models like Vit5, mT5 and BARTpho was finetuned on **5 epochs** and optimizer is set to **AdamW** with **1e-5** lr and 256 to 1024 max token length.
- Large-size model like Vit5-large have finetuned on **3-5 epochs** due to the limitation of computational resources and the optimizer is set to **Adafactor** and **PEFT techniques**, **Gradient checkpoint - accumulation**, and **Accelerator** was leveraged to fine-tune on such a large model. Also, the model was tested on **512 and 1024 max token length**.
## Results
![Screenshot 2024-12-03 083339](https://github.com/user-attachments/assets/2a8e1cc9-4d9c-4da6-92f7-f5235f222b49)
## Demo
https://github.com/user-attachments/assets/6c066d0d-fe05-4909-96c4-87597b307b91


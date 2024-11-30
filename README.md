# CS431-ViT5-research
## Resources
- Dataset **Wikilingua** from **HuggingFace**
- Computational resource **GPU P100** from **Kaggle**
## System settings
- All base size models like Vit5, mT5 and BARTpho was finetuned on **5 epochs** and optimizer is set to **AdamW** with **1e-5** lr and 256 to 1024 max token length.
- Large-size model like Vit5-large have finetuned on **2-3 epochs** due to the limitation of computational resources and the optimizer is set to **Adafactor** and **PEFT techniques**, **Gradient checkpoint - accumulation**, and **Accelerator** was leveraged to fine-tune on such a large model. Also, the model was tested on **512 and 1024 max token length**.
## Results



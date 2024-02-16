# Awesome-VLM-Architectures
<details> 
  <summary><h3>LLaVA</h3></summary> 
  
  | title                                                                    | model_name | architecture.overview                                                                                                                                     | architecture.components                                                                                                                       | training.methods                                                                                                                                                                                     | alignment_techniques.methods                                                                                                                                                     | datasets.used                         |
| ------------------------------------------------------------------------ | ---------- | --------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------- |
| [LLaVA: Large Language and Vision Assistant](https://llava-vl.github.io) | LLaVA      | LLaVA connects a vision encoder and an LLM for general-purpose visual and language understanding, leveraging Vicuna as the LLM and CLIP's visual encoder. | Vision Encoder (CLIP's ViT-L/14), Language Model (Vicuna), and a simple linear layer to connect image features into the word embedding space. | Two-stage instruction-tuning procedure: 1) Pre-training for Feature Alignment using CC3M filtered to 595K image-text pairs. 2) Fine-tuning End-to-End on LLaVA-Instruct-158K dataset and Science QA. | Converts image-text pairs into instruction-following format using GPT-4 generated data, leveraging symbolic representations like captions and bounding boxes for image encoding. | CC3M, LLaVA-Instruct-158K, Science QA | 
</details>
<details>  
  <summary><h3>LLaVA v2</h3></summary> 
  
  | title                                                                                 | model_name | architecture.overview                                                                                                   | architecture.components                                                                        | training.methods                                                                                                                                                                      | alignment_techniques.methods                                                                                                                               | datasets.used                                                                    |
| ------------------------------------------------------------------------------------- | ---------- | ----------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- |
| [Improved Baselines with Visual Instruction Tuning](https://arxiv.org/abs/2310.03744) | LLaVA-1.5  | Enhanced LLaVA with a two-layer MLP for the vision-language connector and inclusion of academic-task-oriented VQA data. | Vision Encoder (CLIP ViT-L/336px), Language Model (Vicuna 13B), MLP vision-language connector. | Two-stage training with pre-training on LCS-558K dataset and fine-tuning on a mixture of VQA, OCR, and region-level VQA datasets, resulting in a final training dataset size of 665K. | Employment of a two-layer MLP for improved multimodal representation and inclusion of academic-task-oriented VQA datasets for enhanced model capabilities. | LCS-558K, VQA, OCR, region-level VQA, visual conversation, language conversation |
</details>


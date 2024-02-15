# Awesome-VLM-Architectures
<details>
  <summary><h3>LLaVA 1.5</h3></summary>
  ![image](https://github.com/gokayfem/Awesome-VLM-Architectures/assets/88277926/d1cc76f0-cade-4985-bc24-9ee356324113)  
  

  
  | Paper Title                                | Architecture Overview                                                                                                                                                                                                                                   | Training Method Detailed                                                                                                                                                                                               | Alignment techniques                                                                                                                                                                   | Datasets Used                         |
  | ------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------- |
  | LLaVA: Large Language and Vision Assistant | LLaVA connects a vision encoder and an LLM for general-purpose visual and language understanding. It uses the open-set visual encoder of CLIP with the language decoder Vicuna, fine-tuning end-to-end on generated instructional vision-language data. | LLaVA is trained in two stages: pre-training for feature alignment using filtered CC3M image-text pairs, and fine-tuning end-to-end on LLaVA-Instruct-158K dataset for multimodal chatbot and Science QA applications. | A simple linear layer connects image features into the word embedding space of the LLM. The model uses auto-regressive training objective for instruction-tuning on prediction tokens. | CC3M, LLaVA-Instruct-158K, Science QA |

</details>


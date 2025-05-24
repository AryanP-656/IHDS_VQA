# Visual Question Answering on Indian Heritage using BLIP

This project fine-tunes the BLIP (Bootstrapping Language-Image Pre-training) model on the _Indian Heritage in Digital Space (IHDS)_ dataset to perform **Visual Question Answering (VQA)**. The system answers questions about Indian heritage sites using image-question pairs, helping in digital preservation and educational outreach.

## Highlights

- Fine-tuned BLIP on 3,000 annotated images from IHDS
- Achieved **86.42% accuracy** and **0.89 F1 score** on test set
- Beam search used during inference for better answer generation
- Applied techniques: AdamW, learning rate scheduling, dropout, early stopping

## Dataset

- Custom IHDS subset with 50 landmark classes
- Each folder: high-res images + `data.json` (question-answer pairs)
- **Note:** The IHDS dataset is part of the *Indian Heritage in Digital Space (DST/ICPS/IHDS/2018)* initiative under the *Interdisciplinary Cyber Physical Systems Programme*, funded by the **Department of Science and Technology, Government of India**.


## Training

- Epochs: 20
- Batch size: 2
- Optimizer: AdamW
- Scheduler: Cosine Annealing
- Gradient Accumulation: 4

## Future Scope

- Add multilingual support
- Expand dataset to more heritage sites
- Deploy as public API or AR/VR tool

## Authors

Aryan Phadnis, Vibhu V Revadi, Abhishek B R, Vinayak Neginhal, Dr. Uday Kulkarni, Shashank Hegde  
_KLE Technological University, Hubballi_

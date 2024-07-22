QCA Fine-Tuning Framework for Legal Document Retrieval

QAC_fine_tuning/
├── data_preparation/
├── Raw_data/
├── Synthetic_data_generation/
├── data_rag/
│ │ ├── vibilaw/
│ │ ├── coling2020/
│ │ ├── zalo2021/
├── results/
│ ├── results_vibilaw/
│ │ ├── model1_alpha_beta/
│ │ │ ├── epoch_1/
│ │ │ ├── epoch_2/
│ │ │ ├── epoch_3/
│ │ │ ├── epoch_4/
│ │ │ ├── epoch_5/
│ │ │ └── metrics.json
│ │ ├──......
│ ├── results_coling2020/
│ │ ├── model1_alpha_beta/
│ │ │ ├── epoch_1/
│ │ │ ├── epoch_2/
│ │ │ ├── epoch_3/
│ │ │ ├── epoch_4/
│ │ │ ├── epoch_5/
│ │ │ └── metrics.json
│ │ ├──......
│ ├── results_zalo2021/
│ │ ├── model1_alpha_beta/
│ │ │ ├── epoch_1/
│ │ │ ├── epoch_2/
│ │ │ ├── epoch_3/
│ │ │ ├── epoch_4/
│ │ │ ├── epoch_5/
│ │ │ └── metrics.json
│ │ ├──......
├── custom_loss.py
├── fine_tune_model_vibilaw.py
├── fine_tune_model_zalo2021.py
├── fine_tune_model_coling2020.py
└── README

Fine_tune_model

Config for fine-tuning:

models: List of models to train (e.g., keepitreal/vietnamese-sbert).
alphas: List of alpha values to experiment with (e.g., [0.2, 0.3, 0.4, 0.5]).
betas: List of beta values to experiment with (e.g., [0.2, 0.3, 0.4, 0.5]).
loss_option: set "qc-qa" for QC-QA finetuning, "qc-qa-ac" for QC-QA-AC finetuning, and "qc" for baseline fine-tuning.
Fine-tuning results:
The models are saved in folders with the above structure in the results folder.


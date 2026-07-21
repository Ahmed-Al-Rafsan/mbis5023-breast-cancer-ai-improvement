# AI Prompt and Output Log

**AI tool:** ChatGPT (OpenAI)  
**Use:** planning, code generation, code review, debugging guidance, evaluation design, document drafting and formatting  
**Note:** Repetitive prompts are condensed, as permitted by the assessment instructions.

| Iteration | Prompt or instruction summary | Main AI output | Human decision | Verification |
|---|---|---|---|---|
| 1 | Convert the Breast Cancer Wisconsin portfolio brief and supplied dataset into a complete CNN classification submission. | Proposed an end-to-end notebook covering exploration, cleaning, preprocessing, CNN training, validation and evaluation. | Accepted the overall workflow because it matched the portfolio steps. | The executed HTML was opened and reviewed from beginning to end. |
| 2 | Complete the work without asking for additional format decisions. | Produced an executed Jupyter notebook, HTML report and dataset package. | Accepted the notebook as the technical baseline artefact. | Confirmed the student name, model evaluation table, confusion matrix, ROC curve, conclusion and references. |
| 3 | Review what should be submitted and reduce confusion about multiple files. | Explained the purpose of the notebook, HTML and data file. | Modified the submission plan by keeping the notebook as technical evidence and the HTML as readable evidence. | Checked that all files were present in the extracted folder. |
| 4 | Improve the A1 artefact for the A2 process assessment and identify weaknesses in the first-pass model. | Identified raw feature scale differences, absence of a separate validation stage, fixed-length training, weak false-negative control and limited process traceability. | Accepted the diagnosis because each issue could be checked in code or evaluation output. | Compared baseline and improved pipelines on the same held-out test set. |
| 5 | Suggest a stronger CNN workflow while keeping the portfolio requirement for convolutional neural networks. | Suggested training-only standardisation, stratified train/validation/test splitting, a deeper 1D CNN, batch normalisation, dropout, class-weighted loss, weight decay and early stopping. | Accepted most suggestions. Kept a 1D CNN rather than changing to a different algorithm because the portfolio specifically required a CNN. | Executed the notebook with a fixed seed and saved the best validation state. |
| 6 | Design evaluation that does not rely on accuracy alone and gives attention to malignant cases. | Recommended precision, recall, F1, specificity, ROC-AUC, confusion matrices and false-negative counts. | Accepted. Recall and false negatives were treated as major decision criteria. | Baseline and improved metrics were calculated from the same untouched test data. |
| 7 | Critically review whether the model result can be treated as medical evidence. | Warned that the dataset is small, the inputs are tabular measurements rather than raw images, and an academic model is not a clinical diagnostic system. | Accepted and expanded in the ethical reflection. | The limitation is stated in the notebook, README and process report. |
| 8 | A local notebook run produced `ModuleNotFoundError: No module named torch`. | Explained that the failure came from the local Python environment rather than the project code and recommended restoring the original executed notebook. | Accepted. No failed local output was used as project evidence. | The fresh executed notebook and HTML remained the evidence source. |
| 9 | Prepare the A2 process report in original, direct student language and include transparent AI disclosure. | Drafted and formatted the report using the verified technical evidence and prompt log. | Reviewed the draft and removed unsupported claims about branches and merge commits. | The public GitHub repository and its real commits were checked before finalising the report. |

## Examples of rejected or modified AI suggestions

- A suggestion to focus mainly on accuracy was rejected because malignant recall and false negatives are more relevant to the project objective.
- Changing the task to a non-CNN classifier was rejected because the selected portfolio activity specifically required a convolutional neural network.
- Treating the high ROC-AUC as proof of clinical readiness was rejected. The report limits the conclusion to this dataset and academic context.
- Installing packages and rerunning the notebook on an unprepared local environment was not used as evidence. The executed and verified artefact was restored instead.
- Pre-generated branch and merge history was not used. The public repository contains only the genuine commits created through the user's GitHub account.
- AI wording was edited to keep the report direct, specific and consistent with the actual work completed.

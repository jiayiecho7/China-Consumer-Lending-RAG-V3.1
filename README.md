# China Consumer-Lending Regulatory RAG — V3.1

Author: LI JIAYI. Submission materials assembled on 2026-10-03.

This project retrieves Chinese regulatory provisions for consumer-lending compliance questions. It covers mainland China and retains quotations from original Chinese regulations.

## Version and file naming

V3.1 means the historical V3 pipeline with Q36 repaired. It is a project version, not a model name. Every project notebook and report in this submission uses the V3.1 suffix to identify the adopted project release. Supporting audits document that release; their suffix does not imply a new experiment. V5 appears only as a comparison in the evaluation materials.

## Run in Google Colab

1. Open `02_Main_Code_and_API_V3.1.ipynb` in Google Colab, by uploading it or selecting it from this GitHub repository.
2. Run the first three code cells in order for offline reproduction from the embedded corpus and experiment caches. No additional project files need uploading.
3. Keep `RUN_LIVE = False` for the cached demo. To perform a new API run, enable the final cell and enter the API key through the hidden prompt. Five questions are the default; set `N_QUESTIONS = 50` for a full run. New results are saved separately.

The notebook includes its setup instructions. For detailed dependencies, architecture, persona, input/output and metrics, see `README_V3.1.ipynb`. Full module source is readable in `06_Module_Source_and_Explanation_V3.1.ipynb` and embedded in the runnable notebook.

## Submission contents

- [01_Problem_Statement_V3.1.ipynb](01_Problem_Statement_V3.1.ipynb) — Project problem, regional scope, intended user, approach and evaluation.
- [00_Status_and_Submission_Map_V3.1.ipynb](00_Status_and_Submission_Map_V3.1.ipynb)
- [02_Main_Code_and_API_V3.1.ipynb](02_Main_Code_and_API_V3.1.ipynb)
- [03_Data_and_Corpus_V3.1.ipynb](03_Data_and_Corpus_V3.1.ipynb)
- [04_Evals_and_Gold_V3.1.ipynb](04_Evals_and_Gold_V3.1.ipynb)
- [05_Results_and_Failure_Analysis_V3.1.ipynb](05_Results_and_Failure_Analysis_V3.1.ipynb)
- [06_Module_Source_and_Explanation_V3.1.ipynb](06_Module_Source_and_Explanation_V3.1.ipynb)
- [07_Human_Checks_and_Final_Checklist_V3.1.ipynb](07_Human_Checks_and_Final_Checklist_V3.1.ipynb)
- [08_Regulatory_Source_Verification_V3.1.ipynb](08_Regulatory_Source_Verification_V3.1.ipynb)
- [09_Gold_and_Key_Clause_Verification_V3.1.ipynb](09_Gold_and_Key_Clause_Verification_V3.1.ipynb)
- [README_V3.1.ipynb](README_V3.1.ipynb)

## Evaluation scope

Eight regulatory instruments, 199 chunks and fifty development questions underpin the historical experiment. Original Hit@5 is 78% for BM25, 82% for semantic retrieval and 98% for hybrid evidence selection. Coverage within up to ten selected provisions is a separate 100% metric. The questions were used for tuning and are not a held-out test.

The AI-assisted review of fifty gold mappings and source corrections is documented separately in notebook 09. Six answer-review judgments were confirmed by LI JIAYI on 2026-10-03; full independent human review of all fifty labels is not claimed. Post hoc label sensitivity is not a new retrieval experiment. Provider cache costs are not reconciled invoices.

The written report and demonstration video are submitted separately through the course platform. The English report has been approved by the student.

## Upload to GitHub

Extract this archive and upload its contents, including this README.md, the eleven notebooks. Keep the directory structure. Submit the repository URL through the course portal and ensure the instructor can access it. Supply the video separately as required by the portal. Do not embed API keys in files or notebook outputs.

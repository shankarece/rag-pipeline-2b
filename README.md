# Assignment 2B - RAG Pipeline

Single notebook: `assignment_2b_rag.ipynb` (Parts A, B, C, D1, D2).
It reuses the Assignment 1 domain text files, evaluation queries and fine-tuned adapter from `~/grp-165-datavol-1`.

## Run in the lab
1. Free disk first (15 GiB volume; the 7B judge needs about 16-17 GB free): delete `a1b/stage3/merged_bf16`, `a1b/stage2/checkpoints` and unused folders under `a1b/cache/hf/hub`. If space is short the notebook uses Qwen2.5-3B-Instruct as the judge.
2. `git clone https://github.com/shankarece/rag-pipeline-2b`
3. Open `assignment_2b_rag.ipynb`, select kernel **Python (LLM venv)**, Run All. Missing packages are installed by the notebook.
4. Fill the spot-check cell (D2.2: `MY_VERDICTS`, `MY_NOTE`), then re-run it and the cells after it.
5. Export: `jupyter nbconvert --to html assignment_2b_rag.ipynb`
6. Delete unused model caches and stop the server.

Answer spans are proposed automatically and saved to `a1b/stage_2b/answer_spans.json`; they can be edited there.

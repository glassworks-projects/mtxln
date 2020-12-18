# MT-XLN: Multi-Task XLNet for Natural Language Understanding
COMS 6998 E010 final project, rmg2203 + ka2744

Our goal was to construct a version of [MT-DNN](https://github.com/namisan/mt-dnn) that used [XLNet](https://github.com/zihangdai/xlnet) 
for its shared encoder architecture in place of BERT, and to compare performance of the two architectures. We reduced the number of task heads 
from the original MT-DNN methodology, and focused on tasks with more manageable dataset sizes, to allow for more lightweight and flexible training. 
Our results are mixed:

| Task  | CoLA (Matthews Corr.) | STS-B (Pearson/Spearman Corr.) | WNLI (accuracy) |
|-------|-----------------------|--------------------------------|-----------------|
| BERT  | **0.521**             | 0.867/0.86                     | 0.45            |
| XLNet | 0.258                 | **0.885/0.88**                 | **0.56**        |

## Running this repo

1. This repository is set up to run on Python 3.8. Make sure your Python environment has a matching version.
2. Clone this repository.
3. In the repository directory, run `pip install -r requirements.txt`.
4. Run Jupyter, with `jupyter notebook` or similar. 
5. Run (and experiment with) the notebooks.

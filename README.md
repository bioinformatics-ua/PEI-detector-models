# PEI-detector-models

List of deep learning models that are capable of distinguishing computer-generated text from the human-generated text. Each model is inside their respective folder.

## Models
- **chatgpt-roberta**: Recent model (2023) focused on distinguishing chatgpt generated text from a human. They started with the Roberta-base model (which is a masked language model) and then finetuned it in curated data. [PAPER](https://arxiv.org/pdf/2301.07597.pdf) [CODE](https://huggingface.co/Hello-SimpleAI/chatgpt-detector-roberta).
- **openai-roberta-base**: Model trained in 2019 for distinguish gpt2 generated text from human. They started with the Roberta-base model (which is a masked language model) and then finetuned it in curated data. [PAPER](https://d4mucfpksywv.cloudfront.net/papers/GPT_2_Report.pdf#page=12) [CODE](https://huggingface.co/roberta-base-openai-detector).
- **openai-roberta-large**: Model trained in 2019 for distinguish gpt2 generated text from human. They started with the Roberta-large model (which is a masked language model) and then finetuned it in curated data. [PAPER](https://d4mucfpksywv.cloudfront.net/papers/GPT_2_Report.pdf#page=12) [CODE](https://huggingface.co/roberta-large-openai-detector).

## How to run

In each folder there is a `run.sh` script, just run that. The script will build a virtual environment and install all the dependencies.

Inside chatgpt-roberta-detector folder
```bash
python run.sh
```

Inside openai-reberta-detector folder

This runs the base version
```bash
python run-base.sh
```

This runs the large version
```bash
python run-large.sh
```

## Dependencies

The `openai-roberta-detector` only works with python3.7, so python3.7 must be installed!!! (This is a hard requirement due to the transformer library)
The `chatgpt-roberta-detector` works with the latest version of the required libraries, so it should be good to run.

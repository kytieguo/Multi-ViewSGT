# README

## Dependencies & Dataset

PyTorch = 1.11.0

PyG == 2.0.4

## Reproducing results
To reproduce the results, you need to create a directory for recording results:
```
mkdir results
```

Then run the following code for pretraining and finetuning:

```bash
# pre-train and fune-tune the model
sh script/run.sh

python read_results.py --path results/Turbo
```

```bash
# fine-tune a pretrained checkpoint
sh script/finetune.sh

python read_results.py --path results/finetune
```

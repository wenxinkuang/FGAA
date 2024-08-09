
#FGAA: Enhancing the adversarial robustness via fine-grained activation alignment of features

## Requirements

Python = 3.6.9

Pytorch = 1.10.1 + cu113

CUDA = 9.1


## Training

1. Train SAT+FGAA

   ```
   python ./Standard_Adv_Training/train_sas_sas.py --gpu 0 --adv_train 
   ```

2. Train Trades+FGAA

   ```
   python ./Trades/train_trades_cifar10_scas.py
   ```

3. Train MART+FGAA

   ```
   python ./MART/train_mart_scas.py
   ```

## Test

```
python ./pgd_attack_cifar10_sas_sas.py --model_path xxx
```


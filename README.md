# Goal

Recreate part of the results https://github.com/ruqizhang/csgmcmc achieved, only the cSGHMC results which had 4.27% +- 0.03% error rate on CIFAR 10

## Run

From the `experiments` directory, run:

```bash
python3 cifar_csghmc.py \
  --dir=/tmp/csghmc_runs/csghmc_full \
  --data_path=/tmp/csghmc_data \
  --epochs=200 \
  --batch-size=64 \
  --temperature=0.00002 \
  --alpha=0.9 \
  --device_id=0 \
  --seed=1
```

## Result

Ensemble test error: `4.29% - 4.35%`

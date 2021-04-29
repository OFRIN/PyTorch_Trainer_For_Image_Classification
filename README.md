
# Introduction

# Installation
```sh
pip install ray
```

# Preprocessing
```sh
```

# Training

1. Image Classification

```sh
# focal loss
CUDA_VISIBLE_DEVICES=0,1,2,3 python3 train.py \
--architecture efficientnet-b0 --image_size 224 --losses focal --tag EfficientNet-b0@Focal@OGQ-3M \
--gamma 2 --alpha 0.25 \
--train_dataset OGQ_3M --train_data_dir ../OGQ-3M_SH/ --train_domain all \
--test_data_dir ../OPIV6_SH/ --test_domain validation \
--batch_size 768 --max_epoch 100 --lr 0.01 --wd 1e-4 --num_workers 32 --print_ratio 0.01
```

2. Object Detection

```sh
```

3. Semantic Segmentation

```sh
```

4. Instance Segmentation

```sh
```


# Evaluation

```sh
```
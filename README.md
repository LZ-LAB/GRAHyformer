# The GRAHyformer Model
This paper has been submitted to The Web Conference 2025 (WWW 2025).



## Requirements
The version of Python and major packages needed to run the code:
   
    -- python 3.9.16
    -- torch 1.12.0
    -- numpy 1.26.0
    -- tqdm 4.65.0



## How to Run

### GRAHyformer

#### 1. Mixed Arity Knowledge Hypergraph
```
## JF17K dataset
python main-JF.py --dataset JF17K --batch_size 400 --lr 0.00020 --dr 0.999 --input_drop 0.5 --hidden_drop 0.4 --feature_drop 0.2 --dembed 100 --RAD_Size 2 --num_heads 4


## WikiPeople dataset
python main-WP.py --dataset WikiPeople --batch_size 700 --lr 0.00025 --dr 0.995 --input_drop 0.7 --hidden_drop 0.9 --feature_drop 0.5 --dembed 500 --RAD_Size 3 --num_heads 1




## FB-AUTO dataset
python main-FB.py --dataset FB-AUTO --batch_size 800 --lr 0.0001 --dr 0.995 --input_drop 0.6 --hidden_drop 0.5 --feature_drop 0.5 --dembed 400 --RAD_Size 6 --num_heads 4
```


#### 2. Fixed Arity Knowledge Hypergraph
```
## WikiPeople-3 dataset
python main-3ary.py --dataset WikiPeople-3 --batch_size 600 --lr 0.00003 --dr 0.995 --input_drop 0.3 --hidden_drop 0.2 --feature_drop 0.2 --dembed 500 --RAD_Size 10 --num_heads 8

## JF17K-4 dataset
python main-4ary.py --dataset JF17K-4 --batch_size 600 --lr 0.00021 --dr 0.995 --input_drop 0.5 --hidden_drop 0.2 --feature_drop 0.5 --dembed 500 --RAD_Size 3 --num_heads 4

## WikiPeople-4 dataset
python main-4ary.py --dataset WikiPeople-4 --batch_size 300 --lr 0.00025 --dr 0.995 --input_drop 0.7 --hidden_drop 0.9 --feature_drop 0.3 --dembed 100 --RAD_Size 3 --num_heads 4

## JF17K-5 dataset
python main-5ary.py --dataset JF17K-5 --batch_size 600 --lr 0.00031 --dr 0.995 --input_drop 0.6 --hidden_drop 0.1 --feature_drop 0.4 --dembed 300 --RAD_Size 7 --num_heads 12

## WikiPeople-5 dataset
python main-5ary.py --dataset WikiPeople-5 --batch_size 700 --lr 0.00056 --dr 0.999 --input_drop 0.6 --hidden_drop 0.5 --feature_drop 0.2 --dembed 200 --RAD_Size 3 --num_heads 4
```








## Acknowledgments
We are very grateful for all open-source baseline models:

1. HypE/HSimplE: https://github.com/ElementAI/HypE
2. HyperMLN: https://github.com/zirui-chen/HyperMLN
3. RAM: https://github.com/liuyuaa/RAM
4. GETD: https://github.com/liuyuaa/GETD
5. tNaLP+: https://github.com/gsp2014/NaLP
6. PosKHG: https://github.com/zirui-chen/PosKHG
7. HyConvE: https://github.com/CarllllWang/HyConvE/tree/master
8. RD-MPNN: https://github.com/ooCher/RD-MPNN/tree/main/RD_MPNN
9. ReAlE: https://github.com/baharefatemi/ReAlE

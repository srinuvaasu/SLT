# SLT

#Stochastic Latency Training (SLT)
#The code is adapted from the work "Temporal efficient training"

Usage:
python3 ./main_training_parallel.py --lr 0.01 --T 8 --lamb 0.05 --epochs 300 --batch_size 256 --dynamic 1 --TET 1  --cut 1 --seed 1000 --dataset cifar10 --resume 0
python3 ./main_test.py --T 8 --dynamic 1 --TET 1 --cut 1 --dataset cifar10 --batch_size 256


#dynamic: 1/0 denotes SLT swithched on or off
#TET: 1/0 denotes TET loss on or off, when it is off, it corresponds to tdBN

# nanogpt

To create a dataset using Fineweb 
``` python fineweb.py ```

For training
--nproc_per_node is the number of GPUs you want to train on <br/>
``` torchrun --standalone --nproc_per_node=8 train.py ``` <br/>
or <br/>
``` python3 -m torch.distributed.run --standalone --nproc_per_node=8 train.py ```


DATASET:
FineWeb-edu with **10B** Token on the educational dataset

MODEL:
A decoder-only transformer with:
context_length = 1024
vocab_size = 50257
n_layer = 12
n_head = 12
n_embd = 768

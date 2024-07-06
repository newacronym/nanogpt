# nanogpt

To create a dataset using Fineweb  <br/>
``` python fineweb.py ```

**For training** <br/>
--nproc_per_node is the number of GPUs you want to train on <br/>
``` torchrun --standalone --nproc_per_node=8 train.py ``` <br/>
or <br/>
``` python3 -m torch.distributed.run --standalone --nproc_per_node=8 train.py ```


**DATASET:** <br/>
FineWeb-edu with **10B** Token on the educational dataset

**MODEL:**
A decoder-only transformer with:  <br/>
context_length = 1024 <br/>
vocab_size = 50257 <br/>
n_layer = 12 <br/>
n_head = 12 <br/>
n_embd = 768 <br/>

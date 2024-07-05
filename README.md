# nanogpt

To create dataset using fineweb 
``` python fineweb.py ```

For training
--nproc_per_node is the number of gpus you want to train on 
``` torchrun --standalone --nproc_per_node=8 train.py ```

# LAB 8


## Tasks done in this lab
- Checked autograd against a central-difference numerical gradient
- Built the Lab 6 network as an `nn.Module` (`Net`: 2 -> 128 ReLU -> 3, optional dropout)
- Wrote the training step by hand: `zero_grad`, forward, `backward`, `step`
- Wrote `evaluate` with `model.eval()` and `torch.no_grad()`
- Moved batching to a `DataLoader` over a `TensorDataset`
- Combined everything into `run()`, with weight decay and dropout as arguments

## Results
- Autograd and the numerical gradient differ by at most 5.17e-11
- `Net` has 771 parameters, the same count as the Keras model in Lab 7
- Manual loop: loss fell from 1.201 (epoch 1) to 1.003 (epoch 10)
- DataLoader loop: loss 0.996 after 10 epochs, 4 batches per epoch
- `run()` trains 100 epochs in 0.3s and records 21 history rows

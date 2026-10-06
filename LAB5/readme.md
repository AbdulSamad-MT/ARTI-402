# Tasks done in LAB 5


- finished the forward and backward passes for `SpiralNet`. 
- wrote plain SGD and `get_batches` for shuffled mini-batches. Batch size 32 reached 0.80 accuracy, against 0.43 for the full batch. Batch size 8 fell back to 0.57 because the gradients got too noisy.
- built momentum, RMSProp and Adam from scratch, each with its own `update_params`.
- In the 10,000-epoch race, plain SGD reached only 0.70 on training data. Momentum and Adam both got to 0.97, and RMSProp got 0.89. Adam scored 0.82 on the test set.
- Adam still needs a sensible learning rate. It worked best around 0.05 (0.95 accuracy) and failed at 2.0 (0.34, with the loss spiking to about 10).


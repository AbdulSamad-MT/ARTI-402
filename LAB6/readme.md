# LAB 6


## Tasks done in this lab
- Trained a baseline network and saw overfitting in the curves (train 0.983 vs val 0.683)
- Built `evaluate` (loss + accuracy, dropout off)
- Built L1 and L2 regularization (loss and gradient)
- Built a dropout layer (inverted dropout, off at test time)
- Showed why weight initialization matters (He keeps activations stable)
- Built batch norm forward pass
- Compared 4 models: baseline, L2, dropout, L2 + dropout
- Chose the best model on validation and tested once

## Results
- L2 was best: val acc 0.740, test acc 0.710
- Every regularizer shrank the train/val gap

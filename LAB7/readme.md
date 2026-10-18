# LAB 7


## Tasks done in this lab
- Rebuilt the Lab 6 network in Keras (`build_model`) with optional L2 and dropout
- Compiled with Adam, fit for 100 epochs with validation data, and evaluated on train and validation
- Trained an L2-regularized model (5e-4) and checked its penalty in `model.losses`
- Added early stopping (patience 25, restore best weights)
- Used `tf.data` with `steps_per_epoch` to run 2,000 updates efficiently
- Saved and reloaded the model with `model.save` / `load_model`
- Reran the Lab 6 showdown in Keras: baseline, L2, dropout and early stopping
- Plotted decision boundaries and the baseline's training curves

## Results
- Keras baseline (100 epochs): train acc 0.817, val acc 0.593
- Early stopping stopped at epoch 160 of 200 (best epoch 135, val loss 0.931)
- Showdown with 2,000 updates (val loss): baseline 2.301, L2 1.115, dropout 1.852, early stopping 0.946
- L2 was best on validation accuracy (0.733); every regularizer lowered validation loss

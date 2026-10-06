# Tasks done in Lab 4

- Implemented an RNN cell (`rnn_step`) and unrolled it over sequences (`rnn_forward`)
- Counted parameters for RNN, GRU and LSTM (1, 3 and 4 blocks; independent of sequence length)
- Implemented an LSTM cell (`lstm_step`) with forget, input and output gates
- Trained a dense head on the frozen final hidden state (`final_hidden_states`)
- Result: the RNN forgets step 1 by T = 10 (about chance, 0.33); the LSTM stays above 0.94 up to T = 40
- Forget-gate bias test: +4 gives 0.98 accuracy at T = 20, while 0 gives 0.29
- Run with `arti402_figures.py` in the same folder, then Restart & Run All

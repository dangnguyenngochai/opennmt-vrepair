## Overview
This helps keep my mind sane 
### Incremental improvement checklist

- [x] Run RNN Encoder-Decoder pipeline without error
- [x] Check the vocabulary size generated from using config file: both fields size and vocab size are the same with previous experiments
- [ ] Replace everything with Transformer
- [ ] Run the new arch of Transformer without error
- [ ] Add the pre-processing and post-processing steps with VRepair

## Experiment 1
- Desc: This experiement aim for creating a functinable pipeline of VRepair with Opennmt API, the demo use a simple RNN Encoder-Decoder arch for vulnerabilities task with the hyperparameters configuration
    - batch_size: 4
    - valid_batch_size: 1
    - src_vocab_size: 2000
    - tgt_vocab_size: 2000
    - src_seq_length: 1000
    - tgt_seq_length: 100
    - learning_rate: 0.0005
    - rnn_hidden_size: 256
    - input_embedding_size: 256
    - word_vec_size: 256
    - drop_out: 0.1
    - label_smoothing: 0.1
    - adam_decay:0.9
- Artifacts (this is by no mean the model input and output, just the experiments' artifacts for testing and analysis ):
    - Input: Vulnerabilities data generated from the VRepair methods, stored in vul_data
    - Output: Log file **log_100k_steps** of the training process store in log folder





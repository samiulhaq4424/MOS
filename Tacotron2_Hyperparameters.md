# Tacotron 2 Hyperparameters

## Hyperparameters Table

| Category | Parameter | Description | Value |
|----------|-----------|-------------|-------|
| Audio Processing | hop_length | Step size for breaking audio into frames | 200 |
|  | win_length | Length of each window for audio processing | 800 |
|  | n_fft | Fourier transform points | 800 |
| Encoder | encoder_kernel_size | Filter size in convolutional layers | 5 |
|  | encoder_n_convolutions | Number of convolutional layers | 3 |
|  | encoder_embedding_dim | Size of the embedding | 512 |
| Decoder | n_frames_per_step | Frames generated per decoding step | 1 |
|  | decoder_rnn_dim | Size of RNN layer | 1024 |
|  | prenet_dim | Size of prenet layer | 256 |
|  | max_decoder_steps | Maximum decoding steps | 1300 |
|  | gate_threshold | Gate mechanism threshold | 0.5 |
|  | p_attention_dropout | Dropout probability for attention | 0.1 |
|  | p_decoder_dropout | Dropout probability for decoder | 0.1 |
| Attention | attention_rnn_dim | Size of RNN layer in attention mechanism | 1024 |
|  | attention_dim | Size of the attention layer | 128 |
|  | attention_location_n_filters | Number of filters in location-sensitive attention | 32 |
|  | attention_location_kernel_size | Kernel size in location-sensitive attention | 31 |
| Mel-post Processing | postnet_embedding_dim | Size of the embedding in postnet | 512 |
|  | postnet_kernel_size | Kernel size in postnet | 5 |
|  | postnet_n_convolutions | Number of convolutional layers in postnet | 5 |
| Optimization | use_saved_learning_rate | Use saved learning rate | False |
|  | learning_rate | Initial learning rate | 1e-5 |
|  | weight_decay | Regularization in training | 1e-6 |
|  | grad_clip_thresh | Threshold for gradient clipping | 1.0 |
|  | batch_size | Number of examples processed together | 1 |
| Number of Epochs | epochs | Complete pass through the entire training dataset | 450 |


# LAB 9

Autoencoders in PyTorch: learning a compressed code from unlabelled digits.

- Built the encoder and decoder with `nn.Sequential`
- Trained it with MSE between the output and the input
- Swept the code size from 2 to 32 and compared the reconstruction error
- Plotted the 2-D code and tested the codes with logistic regression
- Trained a denoising autoencoder and compared it with the plain one

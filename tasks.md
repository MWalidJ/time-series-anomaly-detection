# xLSTM Autoencoder for Anomaly Detection in Time Series Data
## Dataset:
- [] Find appropriate dataset; must contain (time) series data
- [] training the model only on anomaly-free data
- [] set anomaly-threshold as the max reconstrucion error of the anoamly-free data

## Model:
### xLSTM Autoencoder
1. [] contains 2 xLSTM layers, one as Encoder, one as Decoder.
- The Encoder encodes the input series data into a lower dimensional latent representation.
- The Decoder decodes this latent representation and maps back to the original vector space.
- The reconstruction loss is calculated based on the input data and the reconstructed data.
- set anomaly-threshold as the max reconstrucion error of the anoamly-free data.
2. [] after the training, apply the xLSTM Autoencoder model on an unseen dataset (containing anomalies). The found anomalies are the ones, that has higher reconstruction error, than the anomaly-threshold.
3. [] comparison with LSTM and Transformer models
4. [] optimize the architecture with an Evolutionary Algorithm (e.g., Bacterial)

## Literature:
- [LSTM-Autoencoder based Anomaly Detection for Indoor Air Quality Time Series Data](https://arxiv.org/pdf/2204.06701)
- xLSTM - [github](https://github.com/NX-AI/xlstm), [Paper](https://arxiv.org/abs/2405.04517)

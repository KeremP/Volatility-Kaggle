# Volatility-Kaggle
Development repo for Optiver Realized Vol Prediction Kaggle competition.

# Notes

### PyTorch Experiments:
- Initial baseline: trained shallow MLP. Decent results w/ RMSPE @ ~.36
- Transformer baseline: trained transformer architecture. Vol is typically localized - transformer may be able to learn this locality wrt attention weights. Current implementation overfits big-time. Have to fix issues w/ output shape as well.
- Update: Torch v3 model (including filtered sampling and FE) improved score to ~.349

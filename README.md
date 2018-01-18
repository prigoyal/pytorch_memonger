# pytorch_memonger

This repository contains implementation of various PyTorch models using the
gradient checkpointing which allows trading compute for memory and hence allows
training bigger/wider models and use large minibatch sizes.

The application of checkpointing is showcased on various models:

- ResNet
- DenseNet
- LSTM model from pytorch examples [here](https://github.com/pytorch/examples/blob/master/word_language_model/model.py)
- VNet model which is used in medical imaging applications, available [here](https://github.com/mattmacy/vnet.pytorch)

In order to use the models, you need to install PyTorch master following instructions from [here](https://github.com/pytorch/pytorch/#from-source)

To run checkpointed models and their baseline tests, follow the commands below:
```
# for checkpointed
python test_memory_optimized.py

# for baseline
python test_memory_optimized.py
```

## Tutorial

We provide a [tutorial]() to describe how to use checkpointing for various kinds of
models.

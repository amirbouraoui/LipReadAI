## Use GPU on M1 Mac
```bash
# Install miniforge
conda install -c conda-forge

# Create a new environment
conda init zsh
conda create --name tf_m1 python=3.9
conda activate tf_m1

# Install tensorflow
pip install tensorflow tensorflow-metal
```
```python
tf.config.experimental.list_physical_devices('GPU')
```

## LipNet Paper
https://arxiv.org/pdf/1611.01599.pdf
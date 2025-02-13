<!-- doc-test-command: echo "installation.md does not need test" -->

# Setup
> Colossal-AI currently only supports the Linux operating system and has not been tested on other OS such as Windows and macOS.
>
> Environment Requirement: PyTorch 1.10 ~ 1.12 (WIP higher version), Python >= 3.7, CUDA >= 11.0. If you encounter any problem about installation, you may want to raise an [issue](https://github.com/hpcaitech/ColossalAI/issues/new/choose) in this repository.


## Download From PyPI

You can install Colossal-AI with

```shell
pip install colossalai
```

If you want to build PyTorch extensions during installation, you can use the command below. Otherwise, the PyTorch extensions will be built during runtime.

```shell
CUDA_EXT=1 pip install colossalai
```


## Download From Source

> The version of Colossal-AI will be in line with the main branch of the repository. Feel free to raise an issue if you encounter any problem. :)

```shell
git clone https://github.com/hpcaitech/ColossalAI.git
cd ColossalAI

# install dependency
pip install -r requirements/requirements.txt

# install colossalai
pip install .
```

If you don't want to install and enable CUDA kernel fusion (compulsory installation when using fused optimizer):

```shell
CUDA_EXT=1 pip install .
```

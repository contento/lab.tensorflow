# Tensorflow

> Most samples generated with OpenAI ChatGPT 4.0

## Requirements

* [requirements.txt](./requirements.txt)

### Installing CUDA

```shell
sudo apt install cuda-toolkit
```

Please make sure that:

* `PATH` includes `/usr/local/cuda-11.8/bin`
* `LD_LIBRARY_PATH` includes `/usr/local/cuda-11.8/lib64`, or, add `/usr/local/cuda-11.8/lib64` to /etc/ld.so.conf and run `ldconfig as root

## Setting the PIP environment

```shell
python -m venv .venv
# [MacOS M*] arch -x86_64 python3 -m venv .venv 

./.venv/scripts/activate 
# [bash]     source .venv/bin/activate

python -m pip install -U -r requirements.txt

# you may need to upgrade pip
python -m pip install --upgrade pip
```

### Using with Miniconda [OPTIONAL]

[Miniconda install](https://docs.conda.io/projects/miniconda/en/latest/index.html)

```shell
mkdir -p ~/miniconda3
# Choose the right Python version with `python --version` !
wget https://repo.anaconda.com/miniconda/Miniconda3-py310_23.9.0-0-Linux-x86_64.sh -O ~/miniconda3/miniconda.sh
sh ~/miniconda3/miniconda.sh -b -u -p ~/miniconda3
rm -rf ~/miniconda3/miniconda.sh
```

#### CUDA Toolkit (nVidia)

```shell
conda install -c conda-forge cudatoolkit
```

# AnyDoor for Win

## Introduction

This is Windows model of AnyDoor using Gradio.

Original: [AnyDoor](https://github.com/damo-vilab/AnyDoor), [AnyDoor-for-windows](https://github.com/sdbds/AnyDoor-for-windows)

### Dependencies

- OS: Windows
- nvidia:
  - cuda: 11.7
- python 3.10.5 (using Pyenv)

## Install

## Clone from GitHub

Clone from GitHub, and move to the folder " SadTalker ".

```bash
git clone https://github.com/supplepentan/AnyDoorForWinGradio
cd AnyDoorForWinGradio
```

## Virtual environment

Virtual environment with Python-version 3.10.5 using Pyenv.

```bash
pyenv local 3.10.5
python -m venv venv
venv/scripts/activate
```

## Libraries

Install libraries using " reqruirements.txt "

```bash
python -m pip install -r requirements.txt
```

### Pytorch

Uninstall unnecessary installed Pytorch, and newly install Pytorch (CUDA11.7 compatible model), xFormers and triton.

```bash
python -m pip install torch torchvision --index-url https://download.pytorch.org/whl/cu117
python -m pip install xformers==0.0.20
python -m pip install triton-2.0.0-cp310-cp310-win_amd64.whl
```

## Download Checkpoints

Download AnyDoor checkpoint:

- [ModelScope](https://modelscope.cn/models/damo/AnyDoor/files)
- [HuggingFace](https://huggingface.co/spaces/xichenhku/AnyDoor/tree/main)

## Run the Gradio

```bash
python app.py
```

Access to http://127.0.0.1:7860 .

## Acknowledgements

This code is built on [AnyDoor](https://github.com/damo-vilab/AnyDoor) and [AnyDoor-for-windows](https://github.com/sdbds/AnyDoor-for-windows) , thank for the authors for sharing their codes.

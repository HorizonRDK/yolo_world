English| [简体中文](./README_cn.md)

Tool: Used to generate a text embeddings file.
=======

# Feature Introduction
This tool allows users to customize the categories required for YOLO World dnn node detection. Specific usage:
1. Store the category to be detected in the "class.list" file in the current directory.
2. Download the required text encoder model file "text_coder.onnx".
3. Run the script to generate the text embeddings named "offsine-vocabulary_ embeddings.json".

# Development Environment

- Programming Language: python
- Development Platform: X5/X86

# Note

The entire project directory structure is as follows

```tool
├── __init__.py
├── class.list
├── main.py
├── text_encoder.onnx
└── clip
    ├── __init__.py
    ├── bpe_simple_vocab_16e6.txt.gz
    ├── clip.py
    └── simple_tokenizer.py
```

# Usage

wget http://sunrise.horizon.cc/models/clip_encode_text/text_encoder.tar.gz
mkdir -p config
sudo tar -xf text_encoder.tar.gz -C config

```shell
# Download the model
wget http://sunrise.horizon.cc/models/yoloworld_encode_text/text_encoder.tar.gz
sudo tar -xf text_encoder.tar.gz -C tool

# Run the script
python3 main.py
```

log:
```shell
Current Process: 1/80
Current Process: 11/80
Current Process: 21/80
Current Process: 31/80
Current Process: 41/80
Current Process: 51/80
Current Process: 61/80
Current Process: 71/80
finish!
```
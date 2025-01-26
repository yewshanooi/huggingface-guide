## A guide to download and use pre-trained models locally with Hugging Face's Transformers.js library

1. Download [Python](https://www.python.org/downloads/) with pip

2. Install Hugging Face 🤗 [Optimum](https://github.com/huggingface/optimum) package collection
```sh
python -m pip install optimum
```

3. Install other relevant packages based on the **requirements.txt** file
```sh
pip install -r requirements.txt
```
> [!NOTE]
> **scripts**/**convert.py**, **quantize.py**, and **requirements.txt** files are taken from the [huggingface/transformers.js](https://github.com/huggingface/transformers.js) repository

4. Convert a model of your choice from [Hugging Face](https://huggingface.co/models)
```sh
python -m scripts.convert --quantize --model_id <model_name_or_path>
```
> [!TIP]
> You can use `--modes fp16` as an optional field to use half-precision floating-point format and reduce the ONNX file sizes. The `<model_name_or_path>` parameter is the model name on Hugging Face, for example, **facebook/bart-large-cnn**
<br/>

## Credits
- [Hugging Face](https://github.com/huggingface)

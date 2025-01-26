## Hugging Face Transformers.js Guide

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
> The **scripts**/**convert.py**, **quantize.py**, and **requirements.txt** files are taken from [huggingface/transformers.js](https://github.com/huggingface/transformers.js/tree/main/scripts)

<<<<<<< HEAD
4. Select a model of your choice from Hugging Face [models](https://huggingface.co/models) to convert
=======
4. Convert a model of your choice from [Hugging Face](https://huggingface.co/models)
>>>>>>> 9eb564249f0860ce92a93223deeac35949f58cca
```sh
python -m scripts.convert --quantize --model_id <model_name_or_path>
```
> [!TIP]
> Use the optional `--modes fp16` flag to set model as half-precision floating-point format and reduce the ONNX file sizes. The `<model_name_or_path>` parameter is the model name on Hugging Face, for example, **facebook/bart-large-cnn**
<br/>

5. Your converted model is ready to be used with the [@huggingface/transformers](https://www.npmjs.com/package/@huggingface/transformers) npm package
> [!TIP]
> Files will be saved in `./models/` by default.

## Useful Resources
- [Transformers.js Documentation](https://huggingface.co/docs/transformers.js/en/index)

## Credits
- [Hugging Face](https://github.com/huggingface)

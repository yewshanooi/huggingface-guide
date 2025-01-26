## Hugging Face Transformers.js Guide

1. Download and install [Python](https://www.python.org/downloads/)

2. Install Hugging Face 🤗 [Optimum](https://github.com/huggingface/optimum) pip package
```sh
python -m pip install optimum
```

3. Install other relevant packages based on the **requirements.txt** file
```sh
pip install -r requirements.txt
```
> [!NOTE]
> The **scripts**/**convert.py**, **quantize.py**, and **requirements.txt** files are taken from [huggingface/transformers.js](https://github.com/huggingface/transformers.js/tree/main/scripts)

4. Select a model of your choice from [Hugging Face](https://huggingface.co/models) to convert
```sh
python -m scripts.convert --quantize --model_id <model_name_or_path>
```
> [!TIP]
> Use the optional `--modes fp16` flag to set model as half-precision floating-point format and reduce the ONNX file sizes. The `<model_name_or_path>` parameter is the model name on Hugging Face, for example, **facebook/bart-large-cnn**

5. Your converted model is ready to be used with the [@huggingface/transformers](https://www.npmjs.com/package/@huggingface/transformers) npm package
> [!TIP]
> Files will be saved in the `./models/` folder by default. Move it to the root of your project to use the model.
<br/>

## Useful Resources
- [Transformers.js Documentation](https://huggingface.co/docs/transformers.js/en/index)

## Credits
- [Hugging Face](https://github.com/huggingface)



Set the pip mirror if needed:

```bash
# pip mirror
[global]
index-url = https://pypi.tuna.tsinghua.edu.cn/simple
[install]
trusted-host = pypi.tuna.tsinghua.edu.cn
```



If you need a virtual environment:

```bash
python -m venv .env
# linux or mac
source .env/bin/activate
# windows
.env/Scripts/activate
```



Refer Hugging Face official document, install transformers with pytorch and datasets via pip respectively:

Transformers: [Installation (huggingface.co)](https://huggingface.co/docs/transformers/installation)\
Datasets: [Installation (huggingface.co)](https://huggingface.co/docs/datasets/installation)

```bash
pip install 'transformers[torch]'
pip install datasets
```



If meet network issue like this:

```bash
ConnectionError: Couldn't reach 'lansinuote/ChnSentiCorp' on the Hub (SSLError)
```

The resolution is:

```bash
# use git to download dataset from huggingface repo
git clone https://huggingface.co/datasets/lansinuote/ChnSentiCorp
```

[解决在使用huggingface下载数据集失败的问题(ConnectionError)\_coolhuhu\~的博客-CSDN博客](https://blog.csdn.net/weixin_42655901/article/details/124246300)





Reference:

Learning the tutorial from here:&#x20;

[lansinuote/Huggingface\_Toturials: bert-base-chinese example (github.com)](https://github.com/lansinuote/Huggingface_Toturials)


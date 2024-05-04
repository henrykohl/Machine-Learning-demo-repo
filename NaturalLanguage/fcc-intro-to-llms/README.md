* 相關Resource
>
> [**Create a Large Language Model from Scratch with Python – Tutorial (Video)**](https://www.youtube.com/watch?v=UU1WVnMk4E8) from **freeCodeCamp.org**
>
> [A Survey of Large Language Models](https://arxiv.org/pdf/2303.18223) (Online PDF)
>
> [OpenWebTextCorpus](https://skylion007.github.io/OpenWebTextCorpus/) (Download Web)
>
> [OpenWebText On Zenodo home](https://zenodo.org/records/3834942) (openwebtext.tar.xz)

* `training.py` 與 `chatbot.py` 大致複製 `gpt_v1.ipynb` 中 **Model Configuration** 的部分
> 
> * `training.py` 需要，但`chatbot.py` 不需要: `get_random_chunk(split)`、`get_batch(split)`、`estimate_loss()` 和 loop for training 與 model saving
> * `chatbot.py`  需要，但`training.py`不需要: model loading 和 text generation

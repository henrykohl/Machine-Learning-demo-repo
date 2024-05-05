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
> * 使用`chatbot.py`時，檔案`model-01.pkl`必需要存在，範例如下：
> >  * `python chatbot.py -batch_size 32`
> >  * 在`Prompt:`後，輸入`Hello!`，就會產生對應的字串~

* `vocab.txt`來自原Lecture所提供([Github link](https://github.com/Infatoshi/fcc-intro-to-llms/blob/main/vocab.txt))，`openwebtext/vocab.txt`來自訂(Download/Load openwebtext dataset in gpt_v1.ipynb)方法處理所獲得。


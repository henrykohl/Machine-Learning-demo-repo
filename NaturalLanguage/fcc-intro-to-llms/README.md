* 相關Resource
>
> [**Create a Large Language Model from Scratch with Python – Tutorial (Video)**](https://www.youtube.com/watch?v=UU1WVnMk4E8) from **freeCodeCamp.org**
>
> [A Survey of Large Language Models](https://arxiv.org/pdf/2303.18223) (Online PDF)
>
> [OpenWebTextCorpus](https://skylion007.github.io/OpenWebTextCorpus/) (Download Web)
>
> [OpenWebText On Zenodo home](https://zenodo.org/records/3834942) (openwebtext.tar.xz)

* `openwebtext.ipynb`以**Kaggle**建立(專用於**Kagggle**)，根據Lecture所示範的：下載`openwebtext.tar.xz`，整個解壓縮後，再進行處理的方式，產生`train_split.txt`與`val_split.txt`，但受限於**Kaggle**只有19.5GB的空間(Output)，此法無法在**Kaggle**完成整個檔案的解壓處理，但示範處理過程是正確的。

* `training.py` 與 `chatbot.py` 大致複製 `gpt_v1.ipynb` 中 **Model Configuration** 的部分
> 
> * `training.py` 需要，但`chatbot.py` 不需要: `get_random_chunk(split)`、`get_batch(split)`、`estimate_loss()` 和 loop for training 與 model saving
> * `chatbot.py`  需要，但`training.py`不需要: model loading 和 text generation
> * 使用`chatbot.py`時，檔案`model-01.pkl`必需要存在，範例如下：
> >  * `python chatbot.py -batch_size 32`
> >  * 在`Prompt:`後，輸入`Hello!`，就會產生對應的字串~

* `vocab.txt`來自原Lecture所提供([Github link](https://github.com/Infatoshi/fcc-intro-to-llms/blob/main/vocab.txt))，`openwebtext/vocab.txt`來自訂(Download/Load openwebtext dataset in gpt_v1.ipynb)方法處理所獲得。

* `data-extract-v2.py`與`gpt-v2.ipynb`只當作參考用，不用/沒有實際執行。 

* 最後注意，此Lecture的Model Configuration是使用 <font color="red">**Pre-training**</font> 的方式，不是 <font color="red">**Fine-tuning**</font>的方式


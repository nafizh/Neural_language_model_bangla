We trained a neural language model using the Bangla wikipedia corpus. The corpus has 56794 articles. 
The architecture of the neural network is from the [AWD-LSTM](https://arxiv.org/abs/1708.02182) model that currently holds
the stat-of-the-art in terms of perplexity of English language modeling. The code is taken
from the [fastai](https://github.com/fastai/fastai) course, and modified a little for Bangla. I also used this [code](https://github.com/binga/fastai_notes/blob/master/experiments/notebooks/lang_models/Telugu_Language_Model.ipynb) from [Phani Srikanth](https://github.com/binga) that is for Telegu language modeling. The language model weights, 
as wells as the encoder weights can be found [here](https://www.dropbox.com/sh/h6cejxvewsh9nfd/AAAZ2Tnn2eE6miADklU55RD_a?dl=0). The encoder weights can be used for down the line text classification tasks as a pre-trained model.

The current validation cross-entropy loss for this language model is `4.18812`, which in terms of perplexity is `65.898`. Detailed metrics, and performance will be posted soon.

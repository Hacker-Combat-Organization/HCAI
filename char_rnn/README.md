# char-rnn-tensorflow


Multi-layer Recurrent Neural Networks (LSTM, RNN) for character-level shell command models using Tensorflow.

Inspired from Andrej Karpathy's [char-rnn](https://github.com/karpathy/char-rnn).

## Requirements
- [Tensorflow 1.0](http://www.tensorflow.org)

## Basic Usage
To train with default parameters on the shell_commands dataset, run `python train.py`. To access all the parameters use `python train.py --help`. You can also refer to the train notebook.

To sample from a checkpointed model, `python sample.py`. You can also use the sample notebook

## Datasets
We use a dataset collected from observing two hackers play HC. The datasets consist of their shell_commands used through the HC interface.

Start train from the top level directory using `python train.py --data_dir=./data/shell_commands/`, or the notebook.

## Tensorboard
To visualize training progress, model graphs, and internal state histograms:  fire up Tensorboard and point it at your `log_dir`.  E.g.:
```bash
$ tensorboard --logdir=./logs/
```

Then open a browser to [http://localhost:6006](http://localhost:6006) or the correct IP/Port specified.



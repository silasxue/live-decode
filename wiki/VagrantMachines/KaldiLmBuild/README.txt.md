== Preparation

1. Modify KALDI_ROOT in path.sh to your own Kaldi. If you want to use my Kaldi, keep it as it is.
2. Prepare LM training text. I am providing an example, the <example_txt> file. Change it if you want to build upon your own text data.

== Building

Simply run:  ./train_lms.sh <train_txt> <wdir>
The script takes two arguments: the path to your LM training text file, and the working direcotry

You can reproduce the currently-used LM by:
./train_lms.sh example_txt local_lm

== Where to find the LM

The [lang_test_bd_tgpr] direcotry under <wdir> is the decodable LM that you need for decoding.
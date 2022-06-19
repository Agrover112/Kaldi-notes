# Kaldi Resources

Kaldi toolkit has lot of resources and information spread out on the internet, despite the presence of many such similar respositories, many links are often outdated. 
This repository will serve as an list for some great links I found online which can be helpful for learning Kaldi and it's internal workings. This should help in demystifiying
the working of Kaldi.


# Kaldi Lectures

These links contain lectures given by Dan Povey, in the form of Kaldi lectures.

- https://github.com/Agrover112/IIITH-Speech-Internship/tree/master/Kaldi/Lectures

# Text Preprocessing

Text preprocessing is an important aspect in ASR when preparing transcripts from raw-data or cleaning transcripts for preparation of lexicon files, doing preprocessing in Linux
can be helpful and prevent further errors downstream in the pipeline.

- http://jrmeyer.github.io/misc/2019/03/02/Linux-textProc-Notes.html
- 

# Decoding 

The decoding process is important to understand , as it is responsible for the final output. Kaldi creates such decoding graphs via compositions of lattices. I think of compositions
as dot product of Tensors.

- http://vpanayotov.blogspot.com/2012/06/kaldi-decoding-graph-construction.html
- http://cslt.riit.tsinghua.edu.cn/mediawiki/images/6/62/2012-10-25-Step_of_HCLG%28test_time%29.pdf

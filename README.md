# Kaldi Resources

Kaldi toolkit has lot of resources and information spread out on the internet, despite the presence of many such similar respositories, many links are often outdated as of 2022. This repository will serve as an list for some great links I found online which can be helpful for learning Kaldi and it's internal workings. This should help in demystifiying the working of Kaldi.

**I won't accept Pull Requests for fixing Spelling Errors.
I consider it the responsibility of other uses to raise meaningful Pull Requests to help with the cause of learning Kaldi**


# Kaldi Lectures

These links contain lectures given by Dan Povey, in the form of Kaldi lectures.

- https://github.com/Agrover112/IIITH-Speech-Internship/tree/master/Kaldi/Lectures

# Text Preprocessing

Text preprocessing is an important aspect in ASR when preparing transcripts from raw-data or cleaning transcripts for preparation of lexicon files, doing preprocessing in Linux
can be helpful and prevent further errors downstream in the pipeline.

- [Detaied explanation of prepare_dict.sh for Lexicon creation](https://medium.com/@agrover112/understanding-kaldi-part-1-c869980b1cbf)
- http://jrmeyer.github.io/misc/2019/03/02/Linux-textProc-Notes.html
- [Get first column](https://www.unix.com/shell-programming-and-scripting/95024-need-get-first-column-text-file.html) : This can be helpful while splitting lexicon files.
- Fix space indentation and get the second column file : `cat file_lexicon.txt | tr "\t" " " | tr -s " " | cut -d" " -f1 | sort | uniq`
- [tr command](https://www.computerhope.com/unix/utr.htm)
- [Unicode wierd quotation symbols](https://www.cl.cam.ac.uk/~mgk25/ucs/quotes.html) : UTF-8 and us-ascii have some differences such as curly and straight quotations, 
... and one ... dot symbol, grave accents ,etc which might or might not be required in your text file. This link should help you understand how they are different despite looking similar to the untrained eye.

# Kaldi miscellaneous
- [Eleanor Chodroff](https://www.eleanorchodroff.com/tutorial/kaldi/)
- [Joshua Meyer's Kaldi Notes](http://jrmeyer.github.io/asr/2016/02/01/Kaldi-notes.html)
- [Aditya's Notes](https://github.com/AdityaYadavalli1/Kaldi-on-ADA)
- [Aditya's Kaldi Recipes](https://github.com/AdityaYadavalli1/Kaldi-Recipe)
- [Awesome Kaldi](https://github.com/YoavRamon/awesome-kaldi)
- [Kaldi Utilities & misc](https://github.com/stars/Agrover112/lists/speech)


# Theory

Some links related to theory
WFST
- [NTU Semiring and WFST Lectures](https://www.youtube.com/watch?v=1aEinrlyp8w&list=PLxbPHSSMPBeicXAHVfyFvGfCywRCq39Mp)
- [Holy Book of WFSTs](https://cs.nyu.edu/~mohri/pub/hbka.pdf)
- [Edinburgh ASR WFST Lecture](https://www.inf.ed.ac.uk/teaching/courses/asr/2021-22/asr09-wfst.pdf)


Maximum Likelihood Estimation 

- http://jrmeyer.github.io/machinelearning/2017/08/18/mle.html
- [StatQuests Intro](https://youtu.be/XepXtl9YKwc)
- [StatQuest MLE for Normal Dist](https://www.youtube.com/watch?v=Dn6b9fCIUpM)


# Decoding 

The decoding process is important to understand , as it is responsible for the final output. Kaldi creates such decoding graphs via compositions of lattices. I think of compositions
as dot product of Tensors.

- http://vpanayotov.blogspot.com/2012/06/kaldi-decoding-graph-construction.html
- http://cslt.riit.tsinghua.edu.cn/mediawiki/images/6/62/2012-10-25-Step_of_HCLG%28test_time%29.pdf


# Common Kaldi Errors & Questions 
 
 A list of some great errors faced by Kaldi users, I bookmarked. 
 Note: You might need to join the Google Group for viewing them.
 
 - [Kaldi architectures](https://groups.google.com/g/kaldi-help/c/bwm-EBLmxts)
 - [Which DNN to use](https://groups.google.com/g/kaldi-help/c/y6PsX2LN2e4) 
 - [Difference between lang_test_tgsmall and lang_test_tglarge](https://groups.google.com/g/kaldi-help/c/XcaCst1DK2E)
 - [Compiling with CUDA: No Kernel Image ..](https://groups.google.com/g/kaldi-help/c/qIyueT868dw/m/F2QRI77FAAAJ)
 - [Visualizing accuracy plots](https://groups.google.com/g/kaldi-help/c/hH-7O-xD_Ow/m/6Lft-ZlFAwAJ)
 - [QSub not found?](https://groups.google.com/g/kaldi-help/c/Z-5AGulPxzM)
 - [Recompile HCLG decoding graph , when you have more text data (L.fst and G.fst](https://groups.google.com/g/kaldi-help/c/gebauBAbQp8)
 - [ContextFst: CreateArc, invalid olabel supplied](https://groups.google.com/g/kaldi-help/c/L-6V4l9ugNE) 
 - [Likelihood of different pronunciations](https://groups.google.com/g/kaldi-help/c/QEMGPoyE7Sc)
 - [Forced Alignment Decoding Failure](https://groups.google.com/g/kaldi-help/c/FdmCarQtIHU/m/o00Y0aZGAQAJ)
 - [More Decoding Error](https://groups.google.com/g/kaldi-help/c/cUTG5KYykF0/m/kqx_BwS8FgAJ)
 - [Commands  draw-tree, fstprint not working](https://groups.google.com/g/kaldi-help/c/8CZ4zWg2fwA/m/XffHPrMOAQAJ)
 


## Learning to Ask Unanswerable Questions for Machine Reading Comprehension (ACL 2019)

This repo holds data resources used in the [paper](https://www.aclweb.org/anthology/P19-1415/). 

### Question Generation
Directory 'QG' contains data for question generation experiments.

Each example is a tuple of (context, answerable_question, unanswerable_question, answer).

Taking dev set for example, we organize the processed data as follow (one example per line):

dev-**context**.txt

```
context(text)     answer_sentence_start(token position)       answer_sentence_end(token position)
```
dev-**answerable**-questions.txt
```
id      answerable_question(text)     answer_start(token position)    answer_end(token position)
```
dev-**unanswerable**-questions.txt
```
id      answerable_question(text)     answer_start(token position)    answer_end(token position)
```

One can tokenize the text using whitespace.

### Question Answering
Direcotry 'QA' contains the generated unanswerable questions, which serves as augmentation data when combined with all answerable questions in the SQuAD 2.0 training set.

Question answering model is the uncased BERT model (Tensorflow): https://github.com/google-research/bert

### Google Drive Backup
Link: https://aka.ms/AA5n4od 

### Citation
```
@inproceedings{zhu-etal-2019-learning,
    title = "Learning to Ask Unanswerable Questions for Machine Reading Comprehension",
    author = "Zhu, Haichao  and  Dong, Li  and  Wei, Furu  and  Wang, Wenhui  and  Qin, Bing  and  Liu, Ting",
    booktitle = "Proceedings of the 57th Annual Meeting of the Association for Computational Linguistics",
    month = jul,
    year = "2019",
    address = "Florence, Italy",
    publisher = "Association for Computational Linguistics",
    url = "https://www.aclweb.org/anthology/P19-1415",
    doi = "10.18653/v1/P19-1415",
    pages = "4238--4248",
}
```

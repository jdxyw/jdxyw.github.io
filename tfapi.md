## tensorflow API learning record

**sparse_softmax_cross_entropy_with_logits和softmax_cross_entropy_with_logits的区别**
```python
sparse_softmax_cross_entropy_with_logits
softmax_cross_entropy_with_logits
```
A: 二者没有区别，区别只是label的输入，前者更为方便简单，因为很多时候，训练数据的label就是一个index，如果用后者，需要将其转换成一个one-hot的数组，前者则只需要用id输入即可，故为sparse，与spare lr里的特征id是同一个道理，无需one-hot标识。
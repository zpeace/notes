- 超越人的表现
- 减小偏差：更大数据，更深网络

- 超越人类的：online advertising, product recommendations, logistics, loan approvals
- 自然感知难：图像语音识别，人类表现好很多

- 正交化：分开调参数
- 处理方差：regularization, more data, drop out, different nn, hyper parameter

- find out why false positives/false negatives
- segment falses
- attack accordingly: more data, special design

- random wrong label is probably ok
- systemtic error in lables is an issue

- build your first system quickly, then iterate
- be aware of the objective. should be reminded on the objective when building models

- addressing data match: find out why, try collect more data or create artificial data
- artificial data synthesis

- transfer learning
- only retrain the last few layers
- task A and B have the same input x
- you have a lot more data for task A than task B
- low level features from A could be helpful for learning B

- multi-task learning
- training on a set of tasks that could benefit from having shared lower-level features
- amount of data you have for each task is similar
- can train a big enough neural network to do well on all the tasks

- end-to-end deep learning

- convolutional neural networks
- edge detector
- padding
- 


### Naive Bayes
- extremely fast
- used for multi-condition probability









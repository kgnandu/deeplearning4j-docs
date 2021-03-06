---
title: 文本分析与深度学习
layout: cn-default
---

# 文本分析与深度学习

从本质上看，图像是模糊的非结构化数据，而文字则属于一种半结构化的数据类型，即我们所知的语言。语言之中包含了有关其自身的信息。 

我们可以将语言视为一种数据压缩的形式，关于整个世界的知识通过这种形式被压缩到一套符号体系中。就像有损文件或序列化数据集一样，文字是原本规模更庞大的信息的压缩形式。所以，您也可以认为深度学习在文字领域的潜力比图像领域更大，因为文字的实质是可认知的。 

尽管如此，文本分析依然为机器学习带来了许多挑战。三层式神经网络应用于文本分析时的主要缺点是繁琐的手动特征提取。数据科学家需要花费大量时间来指明算法所应关注的特征。 

他们所选择的特征可能包括每个词的词性标签，还有可能包括词是否出现，以及词在某一段特定文本中的出现次数，每条规则都必须小心谨慎地制定。这样的流程也会导致每个词的特征数量过多，许多特征可能都是冗余的。 

深度学习的主要优势之一在于特征创建基本是自动化的。为了说明它的具体功能，我们首先需要深入介绍一下特征提取。

一段文本被输入神经网络后会经历多个阶段的分析。首先是语句切分，软件会找出文本中句子的边界。第二阶段是[分词](./tokenization.html)，软件会识别出具体的词语。在第三阶段，每个词被赋予词性标签；第四阶段则按词干或概念将词分组，这一过程称为词形还原（lemmatization）。例如，“be”、“been”、“is”这样的词会被归为同一组，因为它们表示同样的动词概念。 

名为[Word2vec](./word2vec.html)的神经网络可以完成到词形还原之前的所有步骤。词形还原就是根据词干来扩展特征，深度学习可以用其他方式自动完成这一过程。

在讲解Word2vec之前，我们还要先介绍一种略简单一些的算法：[词袋法](./bagofwords-tf-idf.html)。

# Right, but Why?!
a workshop on machine learning model interpretation
by Hanan Shteingart, PhD
and Yigal Wienberger

# Table of Content
A. Interpretable Models, by Hanan Shteingart, PhD
  1. [Introduction slides](decks/Right%20by%20Why_%20-%20Introduction.pdf) - talks about the motivation for this workshop.
  2. [Naive Bayes notebook](notebooks/naive_bayes/naive_bayes.ipynb) - a naive bayes multinomial classifier interpretation example on a newsgroups 20 dataset. It shows how one can easily compute $P(class=c|feature x_i)$ thus marking words supporting the true and predicted classes.
  3. [Tree Ensemble notebook](notebooks/random_forest/random_forest.ipynb) - random forest is commonly regarded as blackbox. This is false. One can use decision paths in order to learn about the contribution of each feature to the final decision. I will show how this method can be used on the iris data set. 
  4. [Linear pitfalls notebook](notebooks/linear/linear.ipynb) - many believe a linear model is easily interpertable. However, linear coefficient are far from intuitive. Specifically, coefficient are sensitive to scaling. However, even if you normalize your features, due to mulitcolinearity, features which are positively correlated with the class may end up having a negative coefficient and vice versa. I show how can the importance of each feature can be estimated using bootstrap shuffeling. 

B. Black Box approach using LIME, by Yigal Wienberger
  1. Deck: [Peering into the blackbox](/decks/Peering%20into%20the%20black%20box.pptx)
  2. notebooks: 
    * [MI as the product](/notebooks/Peering into the black box/MI as the product.ipynb)
    * [MI for Ethics](/notebooks/Peering into the black box/MI for Ethics.ipynb)
    * [MI for model improvement](/notebooks/Peering into the black box/MI for model improvement.ipynb)

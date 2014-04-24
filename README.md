Neural Network
---

Neural Networks (NN) are important data mining tool used for classication and clustering.
It is an attempt to build machine that will mimic brain activities and be able to learn.
NN usually learns by examples. If NN is supplied with enough examples, it should be able
to perform classication and even discover new trends or patterns in data. Basic NN is
composed of three layers, input, output and hidden layer. Each layer can have number
of nodes and nodes from input layer are connected to the nodes from hidden layer. Nodes
from hidden layer are connected to the nodes from output layer. Those connections represent
weights between nodes.

Backpropagation Algorithm
--
>Idea behind BP algorithm is quite simple, output of NN is evaluated against desired output. If results are not satisfactory, connection
(weights) between layers are modied and process is repeated again and again until error is
small enough.

Version
----

1.0

Requirement
----

> Python 2.7+


How it use?
-----------
```sh
git clone https://github.com/jgabriellima/backpropagation.git
cd backpropagation
python nn.py
```
If you want modify experimental dataset, just put your datas on code 
```sh
def demo():
    # Teach network XOR function
    pat = [
        [[0,0], [0]],
        [[0,1], [1]],
        [[1,0], [1]],
        [[1,1], [0]]
    ]

    # create a network with two input, two hidden, and one output nodes
    n = NN(2, 2, 1)
    # train it with some patterns
    n.train(pat)
    # test it
    n.test(pat)
```

Any questions, let me know: jgabriel.ufpa@gmail.com / http://jgabriellima.com


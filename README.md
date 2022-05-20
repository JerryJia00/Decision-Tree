# Decision-Tree
This Jupyter NoteBook contains my implementation of Decesion Tree and Random forest.

I calculate the information gain by using the Entropy function, which I also take advantage of to choose the best split.

The key part of growing tree is the following pseudocode:
```
Let S <- {1, 2,..., n} be set of sample point indices

GrowTree(S )
  if (yi = C for all i in S and some class C) then {
    return new leaf(C) If the leaf is pure, then predict that class C
  } else {
    choose best splitting feature j and splitting value k
    S_left = {i in S : Xij < k} 
    S_right = {i in S : Xij >= k}
    return new node(j, k, GrowTree(S_left), GrowTree(S_right))
}
```

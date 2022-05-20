# Decision-Tree
This Jupyter NoteBook contains my implementation of Decesion Tree and Random forest.
```
GrowTree(S )
if (yi = C for all i 2 S and some class C) then {
return new leaf(C) [We say the leaves are pure]
} else {
choose best splitting feature j and splitting value  (*)
S l = {i 2 S : Xi j < } [Or you could use  and >]
S r = {i 2 S : Xi j  }
return new node(j, , GrowTree(S l), GrowTree(S r))
}
```

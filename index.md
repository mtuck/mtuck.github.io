
```python

procdure select (A[1...n], k) //1<= k <= n
  r = A[1]
  for j:= 1 to n
    if(A[j] < r)
      insert A[j] -> AL
    else if (A[j} > r)
      insert A[j} ->AL
    else 
      insert A[j]->AV
  if( <= |AL| )
    select(AL, K)
  else if (K > |AL| + |AR|)
    select(AR, K - |AL| - |AR|)
  else 
    return r
```
* |A| is length of A
* AL is left sublist
* Problem gets smaller by atlest 1 every time

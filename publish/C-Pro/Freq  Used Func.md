- **Upper Bound vs Lower Bound**
```cpp

//this is if we have used it on B
value a a a b b b c c c
index 0 1 2 3 4 5 6 7 8
bound       l     u
```

```cpp
// this are iterator
vector<int>iterator lower,upper;
 lower = lower_bound(v.begin(), v.end(), val);

  upper = upper_bound(v.begin(), v.end(), val);
// for index use we do :
int lower = lower_bound(v.begin(), v.end(), val); - v.begin();
```
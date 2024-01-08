 - Declaration and things I use almost every time
 ```cpp
 vector<int>v;
 //or
 vector<int>v(n,0); // more array like use here
v.sort(v.begin(),v.end());


	// erase the 6th element
  v.erase (myvector.begin()+5);

  // erase the first 3 elements:
  v.erase (myvector.begin(),myvector.begin()+3);

//insert at a position(0th index)

v.insert(v.begin()+i,val) //inserts at ith place:
// for eg:
/*Original vector :

1 2 3 4 5 
insert 6 at position 3 :
1 2 3 6 4 5 
 insert 7 at position 1 :
1 7 2 3 6 4 5
*/

```

- `v[0]` returns a **reference** to the first vector element and `v` must not be empty (otherwise, the behavior is not defined). The type of this expression is `int&` or `const int&`.
    
- `v.data()` returns a **pointer** to the first vector element, or some unspecified pointer value if `v` is empty. The type of this expression is `int*` or `const int*`.
    
- `v.begin()` returns an **iterator** to the first vector element, or `v.end()` if `v` is empty. The type of this expression is `std::vector<int>::iterator` or `std::vector<int>::const_iterator`.

![[Pasted image 20240108183843.png]]
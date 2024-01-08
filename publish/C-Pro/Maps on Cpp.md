

 - map vs unordered_map are mainly differs by how they keep the keys, normal map keeps they keys in a sorted order while the unordered_map does not.
	 - Function like insert,erase,find take $O(n \log n)$ for map while only 
	   $O(n)$ for unordered_map.   
```cpp
    // Declaration 
    std::unordered_map<std::string, int> m;
			std::unordered_map<std::string, int> m2 = {{"apple", 1}, {"banana", 2}};

    // 2 ways to insert :
    m["orange"] = 3;
    m.insert({"cherry", 4});

    // using the key to get it's value
    int a = m["orange"];

    // it returns the iterator to the elment found
    if (m.find("apple") != m.end()) {
        // it return m.end() when it doesn't find element
    }

    // removing keys
    m.erase("orange"); 

    // Iteration
    for (const auto &pair : m) {
        std::cout << pair.first << ": " << pair.second << std::endl;
    }

    // length
    int s = m.size(); // no. of keys

    // clear the whole map
    m.clear();
```

- Find:
```cpp
auto it = m.find("key");

if (it != m.end()) {

cout << "Found: " << it->first << " -> " << it->second << endl;

} else {

cout << "Not found" << endl;

}
```
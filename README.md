# micro-lru

Header-only lightweight STL implementation of an LRU cache in C++ 

# Usage

```cpp
auto lru = MicroLRU::Cache<std::string, void*>(50, [](void* data) { free(data); });

lru.add("Hello World", malloc(100));
```

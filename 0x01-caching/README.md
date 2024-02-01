<p align="center">
<img src ="https://th.bing.com/th/id/OIP.Pfw9pQXHRj0wZx-NsvKvcQAAAA?rs=1&pid=ImgDetMain">
</p>

---

# 0x01. Caching:

- As you explore this repository, you'll find a project that I've been working on. It focuses on the implementation of various caching algorithms, aiming to enhance your understanding and proficiency in caching systems. Together, we'll delve into the concepts of FIFO, LIFO, LRU, MRU, and LFU caching policies, learning their significance and application within software development. Through practical tasks and hands-on exercises, we'll explore the fundamentals of caching, its limitations, and its pivotal role in optimizing system performance. My goal is to offer you a structured approach to comprehend caching mechanisms, equipping you with essential skills for efficient data management and system optimization in backend development scenarios.

---

## Resources:

1. [Cache replacement policies - FIFO](https://en.wikipedia.org/wiki/Cache_replacement_policies#First_In_First_Out_%28FIFO%29)
2. [Cache replacement policies - LIFO](https://en.wikipedia.org/wiki/Cache_replacement_policies#Last_In_First_Out_%28LIFO%29)
3. [Cache replacement policies - LRU](https://en.wikipedia.org/wiki/Cache_replacement_policies#Least_Recently_Used_%28LRU%29)
4. [Cache replacement policies - MRU](https://en.wikipedia.org/wiki/Cache_replacement_policies#Most_Recently_Used_%28MRU%29)
5. [Cache replacement policies - LFU](https://en.wikipedia.org/wiki/Cache_replacement_policies#Least-Frequently_Used_%28LFU%29)

> Note: They all take you to Wikipedia, stay there and stay focused 😁

---

> ### Setup:

- All classes in this project must inherit from the `BaseCaching` class: [base_caching.py](./base_caching.py)

---

## Tasks:


### 0. Basic dictionary

- Implement a class `BasicCache` that inherits from `BaseCaching` to create a simple caching system using a dictionary.
- The caching system should not have a limit on the number of items it can store.
- Implement `put` and `get` methods to add items to the cache and retrieve them.

  - Redirect to file: [0-basic_cache.py](./0-basic_cache.py)

### 1. FIFO caching

- Implement a class `FIFOCache` that inherits from `BaseCaching` to create a caching system using the FIFO (First In, First Out) algorithm.
- The caching system should discard the first item when the maximum number of items is reached.
- Implement `put` and `get` methods.

  - Redirect to file: [1-fifo_cache.py](./1-fifo_cache.py)

### 2. LIFO Caching

- Implement a class `LIFOCache` that inherits from `BaseCaching` to create a caching system using the LIFO (Last In, First Out) algorithm.
- The caching system should discard the last item when the maximum number of items is reached.
- Implement `put` and `get` methods.

  - Redirect to file: [2-lifo_cache.py](./2-lifo_cache.py)

### 3. LRU Caching

- Implement a class `LRUCache` that inherits from `BaseCaching` to create a caching system using the LRU (Least Recently Used) algorithm.
- The caching system should discard the least recently used item when the maximum number of items is reached.
- Implement `put` and `get` methods.

  - Redirect to file: [3-lru_cache.py](./3-lru_cache.py)

### 4. MRU Caching

- Implement a class `MRUCache` that inherits from `BaseCaching` to create a caching system using the MRU (Most Recently Used) algorithm.
- The caching system should discard the most recently used item when the maximum number of items is reached.
- Implement `put` and `get` methods.

  - Redirect to file: [4-mru_cache.py](./4-mru_cache.py)

> ### Advanced Tasks:

5. **LFU Caching** - *Advanced*

- Implement `LFUCache` class inheriting from `BaseCaching`.
- Use LFU algorithm to discard least frequently used items.
- Utilize LRU algorithm for tie-breaking.
- Print `DISCARD: <key>` for each discarded item.

- Redirect to file: [100-lfu_cache.py](./100-lfu_cache.py)

---

## Author

- [`@Josh-techie`]() | Software Engineer Student

  > Reach out to me if you need any help or have any questions.

  <a href="mailto:youssef.abouyahia@e-polytechnique.ma">
  	<img alt="Feel free to contact me" src="https://img.shields.io/badge/-Ask_me_anything-blue?style=flat&logo=Gmail&logoColor=white&link=mailto:youssef.abouyahia@e-polytechnique.ma&color=3d85c6" />
  </a>
  <span> | </span>
    <a href="https://www.linkedin.com/in/youssef-abouyahia/">
        <img alt="Linkedin Profile" src="https://img.shields.io/badge/-Linkedin-0072b1?style=flat&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/youssef-abouyahia/" />
    </a>
    <span> | </span>
    <a href="https://twitter.com/JoesephAb">
        <img alt="Twitter Profile" src="https://img.shields.io/badge/-Twitter-0072b1?style=flat&logo=Twitter&logoColor=white&link=https://twitter.com/JoesephAb&color=1DA1F2" />
    </a>

<p align="center">
<img src ="https://images.pexels.com/photos/3861943/pexels-photo-3861943.jpeg?auto=compress&cs=tinysrgb&w=400">
</p>

---

# 0x00. Pagination:

- This project focuses on the implementation of a pagination system. The main goal is to create a robust and flexible pagination system for managing a dataset of popular baby names. The project is part of the ALX Africa Intranet Curriculum.

---

## Resources:

Read or watch:

1. [REST API Design: Pagination](https://www.moesif.com/blog/technical/api-design/REST-API-Design-Filtering-Sorting-and-Pagination/#pagination)
2. [HATEOAS](https://en.wikipedia.org/wiki/HATEOAS)

---

> ### Setup: Popular_Baby_Names.csv

- Use this data file for your project: [Popular_Baby_Names.csv](https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/misc/2020/5/7d3576d97e7560ae85135cc214ffe2b3412c51d7.csv?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20240131%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20240131T223558Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=1dc770746bf5c53bdb298dbebb6835b842e2b49c858b9e55367349a270923ab2)

---

## Tasks:


### 0. Simple helper function

- Write a function named `index_range` that takes two integer arguments `page` and `page_size`.
  - The function should return a tuple of size two containing a start index and an end index corresponding to the range of indexes to return in a list for those particular pagination parameters.

  - Redirect to file: [0-simple_helper_function.py](./0-simple_helper_function.py)

### 1. Simple pagination

- Copy `index_range` from the previous task and the given `Server` class into your code.
  - Implement a method named `get_page` that takes two integer arguments `page` with a default value of 1 and `page_size` with a default value of 10.

  - Redirect to file: [1-simple_pagination.py](./1-simple_pagination.py)

### 2. Hypermedia pagination

- Replicate code from the previous task.
  - Implement a `get_hyper` method that takes the same arguments (and defaults) as `get_page` and returns a dictionary containing specific key-value pairs related to hypermedia pagination.

  - Redirect to file: [2-hypermedia_pagination.py](./2-hypermedia_pagination.py)

### 3. Deletion-resilient hypermedia pagination

- Start with the provided code.
  - Implement a `get_hyper_index` method with two integer arguments: `index` with a `None` default value and `page_size` with a default value of 10.
  - The method should return a dictionary with specific key-value pairs related to deletion-resilient hypermedia pagination.

  - Redirect to file: [3-hypermedia_del_pagination.py](./3-hypermedia_del_pagination.py)

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

# AVL Searcher

The AVL Searcher code is designed to perform search and insertion operations based on search keys such as CPF (Brazilian individual taxpayer registry number), name, and date of birth. These operations are implemented using templates and have a logarithmic time complexity of O(log n). The data structure used for this purpose is a "self-balancing" binary search tree known as AVL tree. The input data is read from a CSV file named "data.csv".

Search operations in the AVL tree are differentiated based on the following parameters:

* **CPF**: Accepts a CPF as input and returns the information associated with the searched CPF. If the CPF is not found, an error message is displayed.

* **Name**: Accepts a substring as input and returns all names that contain at least that substring. If there are no matches, an error message is displayed.

* **Date**: Accepts two dates as input and returns all information of individuals with birth dates falling within that interval. If the provided date ranges are not valid, an error message is displayed.

The classes `PersonByCPF`, `PersonByName`, and `PersonByBirthDate` are subclasses of a parent class called `Person`. These subclasses are used to overload the comparison operators in a customized manner.

Different templates are implemented for each subclass of `Person`, with overloaded comparison operators tailored to their specific attributes.

## Usage

To compile this program, use the following command in your terminal:

```bash
make
```

To clean dependecies use the following command in your terminal:
```bash
make clean
```



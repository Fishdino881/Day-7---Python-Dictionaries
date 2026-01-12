# Day-7-Python-Dictionaries

A dictionary in Python is a collection of key–value pairs used to store related data efficiently.

Key characteristics:

* Defined using `{ }`
* Ordered and changeable
* Keys must be unique (no duplicates)
* Values can be of any data type

Dictionaries are widely used in real-world applications such as configuration files, APIs, databases, and JSON data handling.

---

Creating a Dictionary

```python
capitals = {
    "USA": "Washington D.C.",
    "India": "New Delhi",
    "China": "Beijing",
    "Russia": "Moscow"
}
```

---

Exploring Dictionary Methods

```python
print(dir(capitals))
print(help(capitals))
```

* `dir()` shows all available dictionary methods
* `help()` provides detailed documentation

---

Accessing Dictionary Values

Using `get()` Method

```python
print(capitals.get("Japan"))
```

Returns `None` if the key does not exist (safe access)

---

Checking if a Key Exists

```python
if capitals.get("Russia"):
    print("That capital exists")
else:
    print("That capital doesn't exist")
```

---

Updating Dictionary Items

Adding a New Key–Value Pair

```python
capitals.update({"Germany": "Berlin"})
```

Updating an Existing Key

```python
capitals.update({"USA": "Detroit"})
```

---

Removing Dictionary Items

```python
capitals.pop("China")   # Removes a specific key
capitals.popitem()     # Removes the last inserted item
capitals.clear()       # Removes all items
```

---

Accessing Keys, Values, and Items

Getting All Keys

```python
keys = capitals.keys()
for key in capitals.keys():
    print(key)
```

---

Getting All Values

```python
values = capitals.values()
for value in capitals.values():
    print(value)
```

---

Getting Key–Value Pairs

```python
items = capitals.items()
for key, value in capitals.items():
    print(f"{key}: {value}")
```

---

Dictionary Example (Basic)

```python
info = {'name': 'Kunal', 'age': 19, 'eligible': True}
print(info)
```

Accessing Data

```python
print(info['name'])
print(info.get('eligible'))
```

---

Key Takeaways

 Dictionaries store data using key–value pairs
 Fast and efficient data retrieval
 Keys are unique and immutable
 Extremely useful for structured data
 Commonly used in APIs, JSON, and backend systems

---

Author

Kunal
Documenting Python fundamentals through daily hands-on practice
Consistent learning • Clean code • GitHub tracking

---


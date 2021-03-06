# Dictionary Comprehensions

Similarly, dictionary comprehensions work almost exactly the same way as set
comprehensions, except that the result is a dictionary (where a unique key is
mapped to a value):

```python runnable
from pprint import pprint

champions = [
  (2014, 'San Antonio Spurs'),
  (2015, 'Golden State Warriors'),
  (2016, 'The Cleveland Cavaliers'),
  (2017, 'Golden State Warriors'),
  (2018, 'Golden State Warriors'),
]
pprint({c[0]: c[1] for c in champions})

# Example: nonunique keys
pprint({c[1]: c[0] for c in champions})
```

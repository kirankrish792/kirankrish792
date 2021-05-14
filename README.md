### Hi there 👋

<!--
**kirankrish792/kirankrish792** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

```python

from dataclasses import dataclass
from typing import Tuple


class Meta(type):
    def __new__(cls, name, bases, attrs):
        new_cls = super().__new__(cls, name, bases, attrs)
        return dataclass(unsafe_hash=True, frozen=True)(new_cls)


class Bio(metaclass=Meta):
    name        : str = "Kiran KS"
    designation : str = "Btech Computer Science"
    college     : str = "College of Engineering Vadakara"
    base        : str = "Kerala, India"
    Website     : str = "https://kiranks.000webhostapp.com/"


class Stack(metaclass=Meta):
    languages   : Tuple[str, ...] = ("Python", "Java", "javaScript", "Kotlin")
    

class Social(metaclass=Meta):
    linkedin    : str = "www.linkedin.com/in/kiran-k-s"
```

-----

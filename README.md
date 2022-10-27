# :raised_hand: :open_hands::new_moon_with_face::full_moon_with_face::unlock::key::closed_lock_with_key:
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
    Website     : str = "http://kiranks.me/"


class Stack(metaclass=Meta):
    languages   : Tuple[str, ...] = ("Python", "Java", "javaScript", "Kotlin")
    

class Social(metaclass=Meta):
    linkedin    : str = "www.linkedin.com/in/kiran-k-s"
```

-----

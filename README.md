```python

from dataclasses import dataclass
from typing import Tuple


class Meta(type):
    def __new__(cls, name, bases, attrs):
        new_cls = super().__new__(cls, name, bases, attrs)
        return dataclass(unsafe_hash=True, frozen=True)(new_cls)


class Bio(metaclass=Meta):
    name        : str = "Khadija Sajid"
    base        : str = "Karachi, Pakistan"
    hobbies     : str = "Valorant and watching shows"



class Stack(metaclass=Meta):
    languages   : Tuple[str, ...] = ("Python", "Java", "Javascript", "HTML", "CSS")
    frontend    : Tuple[str, ...] = ("React")
    backend     : Tuple[str, ...] = ("Node", "Express")
    databases   : Tuple[str, ...] = ("MySQL", "MongoDb", "Firebase")
    misc        : Tuple[str, ...] = ("Git", "Puppeteer", "Three.js", "Swing", "Panda3D", "Bootstrap", "SASS")



class Social(metaclass=Meta):
    linkedin    : str = "khadijasajid"
```

<h3> 🤝🏻 Connect with Me </h3>

<p >
&nbsp; <a href="https://www.linkedin.com/in/khadijasajid/" target="_blank" rel="noopener noreferrer"><img src="https://img.icons8.com/plasticine/100/000000/linkedin.png" width="50" /></a>
</p>

<p align="center">
  <img width="250" src="https://media.giphy.com/media/jIgXf4hgbHCeKiXpvt/giphy.gif">
</p>

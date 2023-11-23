### Hello There! 👋

![](https://hit.yhype.me/github/profile?user_id=100200105) ![Profile Views](https://komarev.com/ghpvc/?username=mahhheshh&style=plastic&label=PROFILE+VIEWS) ![OsBadge](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)

```py
!#/user/bin/python3
from gods_creations.living_beings.humans import Human

class Social:
    platforms = (
        "https://github.com/",
        "https://twitter.com/",
        "https://www.linkedin.com/in/"
    )
    def __init__(self, username: str) -> None:
        self.username: str = username

    def __str__(self) -> str:
        return '-\n'.join([f"{platform}{self.username}" for platform in self.platforms])

class Skills:
    def __init__(self):
        self.languages: list[str] = ["Python", "C++", "Java"]
        self.frameworks: list[str] = ["Django", "Flask", "Pandas"]
        self.databases: list[str] = ["MySQL", "MongoDB"]
        self.misc: list[str] = ["Git", "GitHub", "Ubuntu", "GCP"]

    def __str__(self) -> str:
        return f"-Languages: {', '.join(self.languages)}    \
            \n-Frameworks: {', '.join(self.frameworks)}    \
            \n-Databases: {', '.join(self.databases)}    \
            \n-Misc: {', '.join(self.misc)}"

class Location:
    def __init__(self, city: str, state: str, country: str) -> None:
        self.city: str = city
        self.state: str = state
        self.country: str = country

    def __str__(self) -> str:
        return f"{self.city}, {self.state}, {self.country}"

class Mahhheshh(Human):
    def __init__(self) -> None:
        self.name: str = "Mahesh Mulay"
        self.age: int = 20
        self.occupation: str = "Student"
        self.pronouns: str = ["He", "Him"]
        self.username: str = "Mahhheshh"
        self.location: Location = Location("Pune", "Maharashtra", "India")
        self.interests: list[str] = ["Programming", "AI/ML Enthusiast", "Open Source"]
        self.skills: Skills = Skills()
        self.social: Social = Social(self.username)
    
    def __str__(self) -> str:
            return f"""Hi there 👋!    \
            \nI'm {self.name}, I'm {self.age} years old and I'm a {self.occupation}.    \
            \nI'm from {self.location}. \
            \nI'm interested in {', '.join(self.interests)}. \
            \nMy skills are {self.skills}.  \
            \nYou can find me on {self.social}. \
            \nHappy Coding!👨‍💻"""

if __name__ == "__main__":
    me = Mahhheshh()
    print(me)
```

#### If you like my work, consider giving it a 🌟 to show some :heart:!

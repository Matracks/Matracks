```python
from datetime import datetime


class ReadMe:
    def __init__(self, username="Matracks", year=datetime.today().year):
        self.username = username
        self.year = year
        self.name = 'Paulo Moran'
        self.education = {
            'programming': [
                ['Web Development', 'BIOS Institute'],
                ['Python', 'Udemy + Online Courses'],
                ['Django', 'Udemy + Online Courses'],
                ['Django Rest Framework', 'Udemy + Online Courses']
                ],
            'economist': ['three years economist carrer'],
            'language': ['english - medium level', 'chinese - HSK II']
        }
        self.employment = {
            'finance assistant': ['Lovimar SA', 'Montevideo / Uruguay'],
            'developer': ['developer', 'world'],
        }

    def __str__(self):
        return f"""
        Hi, I am {self.name} and {self.username} on GitHub,
        I am delighted that you are here, have a nice day.
        """

    def doing(self, now=2022):
        today = self.year

        if now < today:
            experience = self.employment['finance assistant']
            return f"""
            I was a finance assistant in {experience[0]} in {experience[1]}.
            """

        elif now == today:
            dream = self.education['programming']
            return f"""
            I am currently learning {dream[-1][0]}.
            """

        else:
            goal = self.employment['developer']
            return f"""
            Hey!, you, in the future, i am working as a {goal[0]} in {goal[1]}.
            """


me = ReadMe()
```

---
:four_leaf_clover: From [Matracks](https://github.com/Matracks)

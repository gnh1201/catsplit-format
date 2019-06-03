# Advanced of Catsplit (draft)
This specification describes a complex application example of Catsplit.

## 1. Complex example of Catsplit
```
(
    (
        ("John", (20, 22)),
        ("Jane", (30, 31))
    ),
    "Catsplit Team",
    (1, 2, 3, 4, 5)
)<=(
    "Person"(
        "Name",
        "Age"("Age1, "Age2")
    ),
    "Organization",
    "Id"()
)
```

in the one line:
```
((('John',(20,22)),('Jane',(30,31))),'Catsplit Team',(1,2,3,4,5))<=(Person(Name,Age(Age1,Age2)),Organization,Id())
```

## 1-1. Convert to JSON (from Example 1)
```
{
    "Person": [
        {
            "Name": "John",
            "Age": {
                "Age1": 20,
                "Age2": 22
            }
        },
        {
            "Name": "Jane",
            "Age": {
                "Age1": 30,
                "Age2": 31
            }
        }
    ],
    "Organization": "Catsplit Team",
    "Id": [1, 2, 3, 4, 5]
}
```

in the one line:
```
{"Person":[{"Name":"John",{"Age1":20,"Age2":22}},{"Name":"Jane","Age":{"Age1":30,"Age2":31}],"Organization":"Catsplit Team",Id:[1,2,3,4,5]}
```

---

## 2. Anonymous List (Anonymous Array)
```
(
    ("oh my error", "http://foo.local", 26, 1, 1),
    ("oh my error", "http://bar.local", 26, 1, 1)
)<=(
    ""("Message", "URL", "Line", "Column", "Stack")
)
```

in the one line:
```
(('oh my error','http://foo.local',26,1,1),('oh my error','http://bar.local',26,1,1))<=((Message,URL,Line,Column,Stack))
```

## 2-1. Convert to JSON (from Example 2)
```
[
    {
        "Message": "oh my error",
        "URL": "http://foo.local",
        "Line": 26,
        "Column": 1,
        "Stack":1
    },
    {
        "Message": "oh my error",
        "URL": "http://bar.local",
        "Line": 26,
        "Column": 1,
        "Stack":1
    }
]
```

in the one line:
```
[{"Message":"oh my error","URL":"http://foo.local","Line":26,"Column":1,"Stack":1},{"Message":"oh my error","URL":"http://bar.local","Line":26,"Column":1,"Stack":1}]
```

---

## Contact us
- support@exts.kr

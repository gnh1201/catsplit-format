# Advanced of Catsplit (draft)

## Complex example of Catsplit
```
(
    (
        ("John", (20, 22)),
        ("Jane", (30, 31))
    ),
    "Catsplit Team",
    (1, 2, 3, 4, 5)
)<=("Person"("Name", "Age"("Age1, "Age2"), "Organization", "Id"())
```

in the one line:
```
((("John",(20,22)),("Jane",(30,31))),"Catsplit Team",(1,2,3,4,5))<=("Person"("Name","Age"("Age1","Age2"),"Organizaton","Id"())
```
or
```
((('John',(20,22)),('Jane',(30,31))),'Catsplit Team',(1,2,3,4,5))<=(Person(Name,Age(Age1,Age2)),Organization,Id())
```
or (use `rotation mode`(experimental))
```
(('John',(20,22),'Jane',(30,31)),'Catsplit Team',(1,2,3,4,5))<=(Person(Name,Age(Age1,Age2)),Organization,Id())
```

## Catsplit to JSON
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

## Contact us
- support@exts.kr

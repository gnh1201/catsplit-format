# Advanced of Catsplit (draft)

## Example with dict/list
```
(
    (
        ("John", (20, 22)),
        ("Jane", (30, 31))
    ),
    "Catsplit Team",
    (1, 2, 3, 4, 5)
)<=("Person"("Name", "Age"("age1,"age2"), "Organization", "Id"())
```

in the one line:

`((("John",(20,22)),("Jane",(30,31))),"Catsplit Team",(1,2,3,4,5))<=("Person"("Name","Age"("age1","age2"),"Organization","Id"())`

or

`((('John',(20,22)),('Jane',(30,31))),'Catsplit Team',(1,2,3,4,5))<=(Person(Name,Age),Organization,Id())`

or (use `rotation mode`(experimental))

`(('John',(20,22),'Jane',(30,31)),'Catsplit Team',(1,2,3,4,5))<=(Person(Name,Age),Organization,Id())`

## to JSON
```
{
    "Person": [
        {
            "Name": "John",
            "Age": 20
        },
        {
            "Name": "Jane",
            "Age": 30
        }
    ],
    "Organization": "Catsplit Team",
    "Id": [1, 2, 3, 4, 5]
}
```

in the one line:

`{"Person":[{"Name":"John","Age":20},{"Name":"Jane","Age":30}],"Organization":"Catsplit Team",Id:[1,2,3,4,5]}`

## Contact us
- support@exts.kr

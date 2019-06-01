# Advanced of Catsplit (draft)

## Example with dict/list
```
(
    (
        ("John", 20),
        ("Jane", 30)
    ),
    "Catsplit Team",
    (1, 2, 3, 4, 5)
)<=("Person"("Name", "Age"), "Organization", "Id"())
```

in the one line:

`((("John",20),("Jane",30)),"Catsplit Team",(1,2,3,4,5))<=("Person"("Name","Age"),"Organization","Id"())`

or

`((('John',20),('Jane',30)),'Catsplit Team',(1,2,3,4,5))<=(Person(Name,Age),Organization,Id())`

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
    "Id": [1, 2, 3, 4, 5]
    "Organization": "Catsplit Team"
}
```

in the one line:

`{"Person":[{"Name":"John","Age":20},{"Name":"Jane","Age":30}],"Organization":"Catsplit Team",Id:[1,2,3,4,5]}`

## Contact us
- support@exts.kr

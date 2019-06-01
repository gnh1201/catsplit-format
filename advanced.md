# Advanced of Catsplit (draft)

## Example with array
```
(
    (
        ('John',20),
        ('Jane',30)
    ),
    'Catsplit Team'
)<=(Person(Name,Age),Organization)
```

in the one line:

`((('John',20),('Jane',30)),'Catsplit Team')<=(Person<(Name,Age)>[],Organization)`

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
    "Organization": "Catsplit Team"
}
```

in the one line:

`{"Person":[{"Name":"John","Age":20},{"Name":"Jane","Age":30}],"Organization":"Catsplit Team"}`

## Contact us
- support@exts.kr

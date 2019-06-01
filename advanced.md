# Advanced of Catsplit (draft)

## Example of with generics and array
```
(
    (
        ('John',20),
        ('Jane',30)
    ),
    'Catsplit Team'
)<=(Person<(Name,Age))>[],Organization)
```

## to JSON
```
{
    "Person": [
        {
            "name": "John",
            "age": 20
        },
        {
            "name": "Jane",
            "age": 30
        }
    ],
    "Organization": "Catsplit Team"
}

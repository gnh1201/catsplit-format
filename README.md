# Catsplit

Catsplit is data interaction format without rich syntax parsers.

## Example of Catsplit
```
('oh my error', 'http://sys.local', '26', '1', '1')<=(Message, URL, Line, Column, Stack)
```

## Example of JSON
```
{"Message": "oh my error", "URL": "http://sys.local", "Line": "26", "Column": "1", Stack: "1"}
```

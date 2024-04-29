# Catsplit
Catsplit is data interaction format without rich or high-cost syntax parsers.

## Background
We already use a common file format such as JSON or XML, but ANSI-like(e.g. ANSI/ISO SQL) data interaction formats are still required in the field. We propose a new format that is human-readable and capable of inter-converting to others.

## Example of Catsplit (our format)
```
('oh my error','http://sys.local','26','1','1')<=(Message,URL,Line,Column,Stack)
```

## Example of JSON
```
{"Message":"oh my error","URL":"http://sys.local","Line":"26","Column":"1","Stack:"1"}
```

## Example of XML
```
<item>
    <Messsage>oh my error</Message>
    <URL>http://sys.local</URL>
    <Line>26</Line>
    <Column>1</Column>
    <Stack>1</Stack>
</item>
```

## MIME Type (Content-Type), E_MAGIC, Extension
```
('application/catsplit','CS','CSPT','cspt')<=(MIME,E_MAGIC,Extension,Header)
```

## Advanced examples
- See [ADVANCED.md](https://github.com/gnh1201/catsplit-format/blob/master/ADVANCED.md)

## Conversion to SQL `insert` statement
Catsplit:
```
('oh my error','http://sys.local','26','1','1')<=(Message,URL,Line,Column,Stack)
```

SQL `Insert`:
```
insert into dummy(Message,URL,Line,Column,Stack) values ('oh my error','http://sys.local','26','1','1')
```

## Contact us
* abuse@catswords.net
* ActivityPub [@catswords_oss@catswords.net](https://catswords.social/@catswords_oss)

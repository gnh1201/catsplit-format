# Catsplit

Catsplit is data interaction format without rich or high-cost syntax parsers.

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

## contact us
- support@exts.kr

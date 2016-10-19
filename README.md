# STJSON
A JSON Parser in Swift 3 compliant with RFC 7159

STJSON was writting along the article [Parsing JSON is a Minefield]().

Basic usage:

```Swift
var p = STJSONParser(data: data)

do {
    let o = p.parse()
} catch let e {
    print(e)
}
```

Instantiation with options:

```Swift
    var p = STJSON(data:data,
                   maxParserDepth:1024,
                   options:[.useUnicodeReplacementCharacter])
```

# wwwwwmmm
[who, what, where, when, why](https://en.wikipedia.org/wiki/Five_Ws) multiple media metadata.

also, alliteration.

A format to store relevant answers to questions in areas of files that can hold them. This way, when media is extracted or converted that we can carry the same general answers to filling later metadata with it.

# wwwww
A [JSON](https://www.json.org) data structure that can be embedded within a file.

```
{
  "who": "" | ["", ""],
  "what": "",
  "where": "" | {"gps": "", "address", ""},
  "when": "",
  "why": ""
}
```

Explanations with attached [JSON Schema](https://json-schema.org/).

## Who

A String or an Array containing a list of people. If a String is chosen, the list would be delimited via semicolon (;).

JSON Schema
```
{
}
```

## What

A string providing a factual explanation of what is happening.

JSON Schema
```
{
}
```

## When

A String containing an [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time with the offset.

JSON Schema
```
{
}
```

## Where

A String or an Object containing location information.
If a String is provided, any location information is valid and would be up for interpretation to the parser.
If an Object is provided the key/value pairs provided help define what location information is provided. The following keys are provided: "gps", "address", "intersection"

JSON Schema
```
{
}
```

## Why

A String providing the "why" of the image or performance, not to be confused with the factual What.

JSON Schema
```
{
}
```

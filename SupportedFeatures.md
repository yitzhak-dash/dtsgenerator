Supported Features
=====

# JSON Schema

- status string
  - o: supported
  - x: no supported
  - p: partially

## Draft-04

|property|status|on TypeScript|
|--------|:----:|----|
|id|o|type name and using referenced target. Restricted URL value only.|
|$schema|o|using to select schema version|
|$ref|p|supported local file and other file reference|
|title|o|comment string|
|description|o|comment string|
|default|x||
|multipleOf|x||
|maximum|x||
|exclusiveMaximum|x||
|minimum|x||
|exclusiveMinimum|x||
|maxLength|x||
|minLength|x||
|pattern|x||
|additionalItems|x||
|items|o|Array type or Tuple type|
|maxItems|x||
|minItems|p|on using Tuple type definition|
|uniqueItems|x||
|maxProperties|x||
|minProperties|x||
|required|o|non nullable type|
|additionalProperties|o|if true, add the index signatures|
|definitions|o||
|properties|o|add some properties in this type|
|patternProperties|x||
|dependencies|x|but also search the sub schema types|
|enum|o|enum type, supported string and integer values|
|type|o|The type of that property|
|format|o|comment string|
|allOf|p||
|anyOf|p||
|oneOf|p|same as `anyOf`|
|not|x||

## Draft-07

### defference from Draft-04

|property|status|on TypeScript|
|--------|:----:|----|
|$id|o|replaces `id`|
|$comment|o|comment string|
|readOnly|o|readonly property|
|writeOnly|x|TypeScript is not support the `writeOnly` property|
|examples|o|comment string|
|contains|x||
|propertyNames|x||
|const|o|literal type|
|contentMediaType|x||
|contentEncoding|x||
|if|x||
|then|x||
|else|x||

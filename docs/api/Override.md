---
title: Symbol Override
order: 206
section: models
---

```javascript
var overrides = symbolInstance.overrides
```

A [Symbol](https://www.sketchapp.com/docs/symbols/) override. This component is not exposed, it is only returned when accessing the `overrides` of a [Symbol Instance](#symbol-instance).

| Properties                                                                                                      |                                                                                                                                                                |
| --------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| path<span class="arg-type">string</span>                                                                        | The path to the override. It's formed by the symbolId of the nested symbols separated by a `/`.                                                                |
| property<span class="arg-type">string</span>                                                                    | The property that this override controls. It can be `"stringValue"` for a text override, `"symbolID"` for a nested symbol, or `"image"` for an image override. |
| id<span class="arg-type">string</span>                                                                          | The unique ID of the override (`${path}_${property}`).                                                                                                         |
| symbolOverride<span class="arg-type">boolean</span>                                                             | If the override is a nested symbol override.                                                                                                                   |
| value<span class="arg-type">String / [ImageData](#imagedata)</span>                                             | The value of the override which can be change.                                                                                                                 |
| isDefault<span class="arg-type">boolean</span>                                                                  | If the override hasn't been changed and is the default value.                                                                                                  |
| affectedLayer<span class="arg-type">[Text](#text) / [Image](#image) / [Symbol Instance](#symbolinstance)</span> | The layer the override applies to. It will be an immutable version of the layer                                                                                |

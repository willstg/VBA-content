
# LineFormat.EndArrowheadStyle Property (PowerPoint)

Returns or sets the style of the arrowhead at the end of the specified line. Read/write.


## Syntax

 _expression_. **EndArrowheadStyle**

 _expression_ A variable that represents an **LineFormat** object.


### Return Value

MsoArrowheadStyle


## Remarks

The  **EndArrowheadStyle** proerty value can be one of these **MsoArrowheadStyle** constants.


||
|:-----|
|**msoArrowheadDiamond**|
|**msoArrowheadNone**|
|**msoArrowheadOpen**|
|**msoArrowheadOval**|
|**msoArrowheadStealth**|
|**msoArrowheadStyleMixed**|
|**msoArrowheadTriangle**|

## Example

This example adds a line to  `myDocument`. There's a short, narrow oval on the line's starting point and a long, wide triangle on its endpoint.


```vb
Set myDocument = ActivePresentation.Slides(1)

With myDocument.Shapes.AddLine(100, 100, 200, 300).Line

    .BeginArrowheadLength = msoArrowheadShort

    .BeginArrowheadStyle = msoArrowheadOval

    .BeginArrowheadWidth = msoArrowheadNarrow

    .EndArrowheadLength = msoArrowheadLong

    .EndArrowheadStyle = msoArrowheadTriangle

    .EndArrowheadWidth = msoArrowheadWide

End With
```


## See also


#### Concepts


[LineFormat Object](11c955d5-bbda-d99f-cec9-fc6187450a12.md)

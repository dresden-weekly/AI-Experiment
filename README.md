# Online Handwriting recognition

The first part of the online handwriting recognition project.
Project goals:

- an offline handwriting interface reading all available touch input information
    - current pointer
    - time delta
    - force
    - touch ellipse
- store symbols into a format that makes sense

Format
------

```json
[
    {
        "strokes":[
          [{"x":1.0,"y":1.0,"t":0,"p":0.5427},{"x":1.2,"y":1.4,"t":0.13124,"p":0.12412},...],
          [{"x":3.1,"y":2.4,"t":1.232,"p":0.2427},{"x":1.6,"y":1.4,"t":1.33124,"p":0.12412},...],
          ...
        ],
        "description":"6",
        "client":"QT"
    }
]
```

Server Store Interface
----------------------

**GET**
```
/records/
/records/[id]
/find/description/[searchString]
/find/client/[searchString]
```
**DELETE**
```
/records/[id]
```
**PUT**
```
/records/
```

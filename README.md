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

see [challenges.json-schema](challenges.json-schema) and [submission.json-schema](submission.json-schema)

Webserver REST API
----------------------

**GET**
```
/api/challenges => JSON
```

**POST**
```
/api/submission Content-Type: application/json Body: {submission: JSON}
```

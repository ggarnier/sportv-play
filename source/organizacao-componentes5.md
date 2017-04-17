## entrada

```json
[{
    "title": "SporTV 3",
    "thumbUrl": "http://...",
    "schedule": [
      {
        "startsAt": "2017-04-17T11:30:00-03:00",
        "durationInMinutes": 120,
        "title": "Masters 1000",
        "description": "Monte Carlo",
        "live": true
      }, ...
    ]
  }, ...]
```

## saída

```json
[{
    "title": "SporTV 3",
    "description": "Masters 1000",
    "subDescription": "Monte Carlo",
    "thumbUrl": "http://...",
    "live": true
  }, ...]
```

Source
```json
{
  "person": {
    "address": {
      "address line 1": "1600 Amphitheatre Parkway",
      "address line 2": "Mountain View, California"
    },
    "phone": "7234873487",
    "memberId": "7846567657"
  }
}
```
Expected output
```json
{
  "address" : {
    "address line 1": "1600 Amphitheatre Parkway",
    "address line 2": "Mountain View, California"
  },
  "phone": "7234873487",
  "memberId": "7846567657"
}
```

JOLT Spec
```json
[
  {
    "operation": "shift",
    "spec": {
      "person": {
        "*": "&"
      }
    }
  }
]
```
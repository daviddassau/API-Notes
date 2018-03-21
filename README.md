# API-Notes

Publicly exposed part of your program, that can be used by other users

### Different parts to HTTP
- Verbs
  - Get
  - Put
  - Post
  - Delete
  - Patch: someone can submit part of an item, and it updates just the things submitted
  - There's a LOT more

Example of sending an order to Jet's Pizza:
- Header:
- Verb: Post
- Body: {...}
- URL: jets.com

The Verb, Body, and URL are the actual request to Jet's

Example of receiving a message back from Jet's
- Response Headers:
- Response Code:
- Body: `{OrderId: ..., TimeReady: ...}`

### REST
- A specific kind of http based API
- Stands for **Representational State Transfer**

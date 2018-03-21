# API-Notes

Publicly exposed part of your program, that can be used by other users

### Different parts to HTTP
- Verbs
  - GET
  - PUT
  - POST
  - DELETE
  - Patch: someone can submit part of an item, and it updates just the things submitted
  - OPTIONS
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
- The cornerstone of a restful api is being resource based. You are going to be representing a resource.
- Idempotency: no matter how many times you do something, the result will always be the same. Examples are `PUT`, `DELETE`, and `PATCH`.
- Safe means that `GET` and `OPTIONS` are garunteed to not change anything.
- `POST` is neither Idempotent nor Safe.

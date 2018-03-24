# API-Notes

Publicly exposed part of your program, that can be used by other users

### Different parts to HTTP
- Verbs
  - `GET`
  - `PUT`
  - `POST`
  - `DELETE`
  - `PATCH`: someone can submit part of an item, and it updates just the things submitted
  - `OPTIONS`
  - There's a LOT more

Example of sending an order to Jet's Pizza:
- Header:
- Verb: Post
- Body: {...}
- URL: jets.com

The Verb, Body, and URL are the actual request to Jet's

### 3 Main things for HTTP Response 
1. Header
2. Body
3. Status

Example of receiving a message back from Jet's
- Response Headers:
- Response Code:
- Body: `{OrderId: ..., TimeReady: ...}`

### REST & HTTP
- A specific kind of http based API
- Stands for **Representational State Transfer**
- HATEOAS
- The cornerstone of a restful api is being resource based. You are going to be representing a resource.
- Idempotency: no matter how many times you do something, the result will always be the same. Examples are `PUT`, `DELETE`, and `PATCH`.
- Safe pertains to certain verbs like `GET` and `OPTIONS`, and how they are garunteed to not change anything.
- `POST` is neither Idempotent nor Safe.
- Example of a HTTP API: `Jets.com/api/orderpizza`
- Example of a RESTful API: `Jets.com/api/orders` or `Jets.com/api/orders/1234`

- Cross Cutting Concerns: they go horizontal/sideways across the application
  - Aspect oriented programming: ???

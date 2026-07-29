# Liftoff Consumer Example

A simple single-page app that consumes the [Postman Liftoff](https://www.postman.com/liftoff) public content API to display learning paths and modules.

## What it does

- Fetches learning paths and modules from the Liftoff API
- Displays them in a searchable, responsive card grid
- Links each card to its page on postman.com/liftoff

## API

The app uses these public endpoints (no authentication required):

| Endpoint | Description |
|---|---|
| `GET /liftoff/api/content/learning-paths` | List all learning paths |
| `GET /liftoff/api/content/modules` | List all modules |

Both support `?q=` for text search.

## Running locally

Open `index.html` directly, or serve it to avoid CORS issues:

```bash
npx serve .
```

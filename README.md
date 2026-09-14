# Mohsin AI Maths

A professional responsive frontend for an AI mathematics learning platform.

## Run
Open `index.html` for the frontend demo.

For production, serve the project from a web server so `/api/solve`, `/api/image-solve`, and `/api/tutor` can be routed to your secure backend.

## Backend contract
Never place secret AI API keys in browser JavaScript.

Suggested JSON request for `/api/solve`:
```json
{"question":"Solve 2x + 5 = 17","class":"Class 8","topic":"Algebra","language":"en"}
```

Suggested JSON response:
```json
{
  "answer":"x = 6",
  "steps":["...","..."],
  "explanation":"...",
  "verification":"..."
}
```

## Endpoints
- POST `/api/solve`
- POST `/api/image-solve` (multipart image upload or secure image reference)
- POST `/api/tutor`

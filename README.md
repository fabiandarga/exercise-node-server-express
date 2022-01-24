# Node mini-server #2 "Express"

## Vorbereitung:
### installiere Express
```bash
npm install express
```

Und in deiner main.js
```javascript
import express from 'express';

const app = express();
const port = 4000;

// Endpoints
// Hier kommt dein Server Code hin.

// Server Start
app.listen(port, () => {
  console.log(`Server listening on port ${port}`)
})
```
## 1. Füge einen "/now" Endpoint hinzu
* Wenn die Url "http://localhost:4000/now" aufgerufen wird, soll das aktuelle Datum und die Uhrzeit zurück gegeben werden.
* In allen anderen Fällen soll immer noch "Hello World" zurück gegeben werden.

## 2. Füge einen "/count" Endpoint hinzu
* Wenn die Url "http://localhost:4000/count" aufgerufen wird, soll eine Zahl zurück gegenem werden,
die jedes mal um 1 weiter gezählt wird.
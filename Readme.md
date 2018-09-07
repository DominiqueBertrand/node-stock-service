# Install

```console
$> npm install
```

# Run

```console
$> node server.js
```

# Query

To load the last 10 stock value samples :

```console
$> curl http://localhost:8000?count=10
```

To load all available stock value samples :

```console
$> curl http://localhost:8000
```

Queries return a JSON array of stock samples :

```javascript
[{
  "timestamp": 1457372998901,
  "index": 0,
  "stocks": {
    "NASDAQ": 14.362588925287127,
    "CAC40": 7.564775763312355
  }
}, {
  "timestamp": 1457372999903,
  "index": 1,
  "stocks": {
    "NASDAQ": 13.27388069476001,
    "CAC40": 13.011122498428449
  }
}]

```
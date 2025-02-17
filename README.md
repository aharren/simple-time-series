# Simple Time Series

## sts.json.eqd.iutsms.fp64.1

JSON-based, simple equidistant time series with ISO UTC timestamps in milliseconds and 64-bit floating point values.

Example:

```
{
  "typ": "sts.json.eqd.iutsms.fp64.1",         // type identifier
  "tss": "2025-04-01T12:00:00.000Z",           // timestamp start
  "tse": "2025-04-01T12:59:59.999Z",           // timestamp end
  "tsd": 900000,                               // timestamp delta
  "val" : {
    "data-1": [ 50, 70, 80, 90 ],              // values of data-1
    "data-2": [ 0.1, 0.1, 0.2, 0.1 ]           // values of data-2
  }
}
```

The time series starts at timestamp `tss` and contains data points for timestamp `tss` and for every subsequent `tsd` milliseconds up to timestamp `tse`.

Data points for `data-1` and `data-2`:
  - `data-1`:
    - `2025-04-01T12:00:00.000Z`: `50`
    - `2025-04-01T12:15:00.000Z`: `70`
    - `2025-04-01T12:30:00.000Z`: `80`
    - `2025-04-01T12:45:00.000Z`: `90`

  - `data-2`:
    - `2025-04-01T12:00:00.000Z`: `0.1`
    - `2025-04-01T12:15:00.000Z`: `0.1`
    - `2025-04-01T12:30:00.000Z`: `0.2`
    - `2025-04-01T12:45:00.000Z`: `0.1`

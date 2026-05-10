# JavaScript Date

## Static Methods

| Syntax | Description | Example | Output |
|---|---|---|---|
| `Date.now()` | Returns current timestamp in milliseconds | `Date.now()` | `1683694830000` |
| `Date.parse()` | Parses a date string and returns timestamp | `Date.parse("2026-05-10")` | `1762800000000` |
| `Date.UTC()` | Returns timestamp for UTC date | `Date.UTC(2026,4,10)` | `1762800000000` |


## Instance Methods (Prototype)

| Syntax | Description | Example | Output |
|---|---|---|---|
| `.getDate()` | Returns day of month | `d.getDate()` | `10` |
| `.getDay()` | Returns day of week (0 = Sunday) | `d.getDay()` | `0-6` |
| `.getMonth()` | Returns month (0-11) | `d.getMonth()` | `4` |
| `.getFullYear()` | Returns year | `d.getFullYear()` | `2026` |
| `.getHours()` | Returns hours | `d.getHours()` | `0-23` |
| `.getMinutes()` | Returns minutes | `d.getMinutes()` | `0-59` |
| `.getSeconds()` | Returns seconds | `d.getSeconds()` | `0-59` |
| `.getMilliseconds()` | Returns milliseconds | `d.getMilliseconds()` | `0-999` |
| `.getTime()` | Returns timestamp | `d.getTime()` | `1762800000000` |
| `.getTimezoneOffset()` | Returns timezone offset in minutes | `d.getTimezoneOffset()` | `-300` |
| `.setDate()` | Sets day of month | `d.setDate(15)` | `timestamp` |
| `.setMonth()` | Sets month | `d.setMonth(6)` | `timestamp` |
| `.setFullYear()` | Sets year | `d.setFullYear(2030)` | `timestamp` |
| `.setHours()` | Sets hours | `d.setHours(12)` | `timestamp` |
| `.setMinutes()` | Sets minutes | `d.setMinutes(30)` | `timestamp` |
| `.setSeconds()` | Sets seconds | `d.setSeconds(45)` | `timestamp` |
| `.setMilliseconds()` | Sets milliseconds | `d.setMilliseconds(500)` | `timestamp` |
| `.toISOString()` | Returns ISO string | `d.toISOString()` | `"2026-05-10T00:00:00.000Z"` |
| `.toDateString()` | Returns human-readable date | `d.toDateString()` | `"Sun May 10 2026"` |
| `.toTimeString()` | Returns human-readable time | `d.toTimeString()` | `"00:00:00 GMT+0000 (UTC)"` |
| `.toLocaleDateString()` | Returns date string in locale format | `d.toLocaleDateString()` | `"5/10/2026"` |
| `.toLocaleTimeString()` | Returns time string in locale format | `d.toLocaleTimeString()` | `"12:00:00 AM"` |


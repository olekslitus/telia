# telia
The Telia programming language

## Module

```
module System
# file:system.telia
```


## Interface
```
interface Console {
  print[D](data: D) -> Nothing
}
```


## Service

### Defining
```
local service SimpleConsole for Console {
  def print[D](data: D) { ... }
}
```

### Composable
```
interface

local service 
```

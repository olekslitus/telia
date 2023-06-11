# telia
The Telia programming language

## Module

```
module System
.
.
.

# system.telia
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
  print[D](data: D) { ... }
}

local service AppleCounter {
  def appleCount() 
}
```

### Composable
```
module CarExample

interface Car {
  drive(speed: Int) -> Nothing
}

local service PrintingCar for Car {
  use print from System>Console

  drive(speed: Int) : Nothing {
    print("Now driving at speed: /{speed}")
  }
}

local service DrivingCar for Car {
  
}
```


## Data
```
module Math

data Angle {
  radians -> Int
}

handler Angle {
  degress -> Int 
}

```

## Handlers
```

```

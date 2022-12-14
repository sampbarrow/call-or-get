# ValueOrFactory

A simple utility type and function that allows you to pass and generate values that are either a value or a function that generates a value.

## Installation

```bash
npm install value-or-factory
```

## Usage

```typescript
import { callOrGet, ValueOrFactory } from "value-or-factory"

function print(value: ValueOrFactory<string, [string]>) {
 return callOrGet(value, "")
}

print("text")
print(() => "text")
print(initialText => initialText + "text")

```

## License

[MIT](https://choosealicense.com/licenses/mit/)

# Template to follow for JavaScript

## Set up jest like so:

## Function only in JS/Jest

```
let functionName = (params) => {
  // function stuffs
}

export functionName();
```

```
import { functionName } from "../src/functionName";

describe('function functionName', () => {
  test('it does the function thing', () => {
    const input = []
    const output = []
    expect(functionName(input)).toEqual(output)
  })
});
```

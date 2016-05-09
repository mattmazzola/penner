# pennerts
A collection of penner functions based on https://github.com/bcherny/penner but using modules and TypeScript.

## Usage

```
import * as penner from 'penner';

const position = penner.linear(time, start, change, duration);
```

Also there is type declared called `IPennerFunction` you can use to reserve a variable to hold a function which will be assigned at a later time.

```
let pennerFunction: penner.IPennerFunction;
...
pennerFunction = penner.linear;
const position = pennerFunction(time, start, change, duration);
```

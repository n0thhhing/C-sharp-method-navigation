# classInfo
This is just a class for getting class info, this was mainly needed by me for another project im working on so yeah

## Installation

```bash
git clone git@github.com:n0thhhing/C-sharp-method-navigation.git
cd C-sharp-method-navigation
```

## Usage

1. Import the module:

```javascript
import { classInfo } from "./classComponents.js";
```

2. Create a new instance of the `classInfo` class, providing the path to the C# file:

```javascript
const myClassInfo = new classInfo("path/to/your/file.cs");
```

3. Use the available methods to retrieve information:

- **getMethodInfo(methodName):** Get information about a method by its name.
- **getOffsetInfo(offset):** Get information about a method by its offset.
- **getMethod(offset):** Get the full method code by its offset.
- **getClassFromOffset(offset):** Get the class name that contains a method with the given offset.
- **getClassInfo(csPath, className):** Get information about a class by its name.

## Example

```javascript
const methodInfo = myClassInfo.getMethodInfo("SomeMethod");
console.log(methodInfo);
```
## Additional Notes

- The module uses regular expressions to parse the C# code, so it might not work perfectly for all file structures.
- The `isObfuscated(str)` method can be used to check if a string is likely obfuscated. (if your into unity game modding then you will understand)
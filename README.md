 **Here's the README.md content, wrapped in backticks for easy copying:**

```markdown
# classInfo

This module provides functions for extracting information from C# files, such as class names, method names, offsets, and fields. It uses regular expressions to parse the file content.

## Installation

```bash
git clone
```

## Usage

1. Import the module:

```javascript
import { classInfo } from "classComponents.js";
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
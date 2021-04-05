# Prettier Config
Basic prettier config which can be referenced and locally extended in your projects.

# Overview
| Property | Description | Default value |
| --- | --- | --- |
| `semi` | Print semicolons | `false` |
| `singleQuote` | Use single quotes instead of double quotes | `true` |
| `trailingComma` | Print trailing commas wherever possible when multi-line. `all`: Trailing commas wherever possible (including function arguments). | `"all"` |
| `printWidth` | The line length where Prettier will try wrap | `100` |
| `endOfLine` | Which end of line characters to apply. `auto`: Maintain existing (mixed values within one file are normalised by looking at what's used after the first line) | `"auto"` |
| `arrowParens` | Include parentheses around a sole arrow function parameter. `arrowParens`: Always include parens. Example: `(x) => x` | `"always"` |

# Usage
## Add to package
```
yarn add https://github.com/sohailykhan94/bootstrap-prettier-config -D
```

## Include in local config
### .prettierrc.js
```
module.exports = {
  ...require("bootstrap-prettier-config"),
  semi: false,
}
```

### package.json
```
"prettier": "bootstrap-prettier-config"
```
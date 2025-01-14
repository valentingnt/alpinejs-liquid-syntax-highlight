# alpine-syntax-highlight

Javascript syntax highlighting for x- attribute values in html for [Alpine JS](https://alpinejs.dev/)

## Supported Files

- html
- php
- twig
- liquid

## Syntax Highlighting

This extension includes custom syntax highlighting for Alpine.js directives:

- **x- directives**: Bold Alpine green highlighting
- **Shorthand operators** (: @ #): Bold Alpine green highlighting
- **Modifiers**: Light Alpine green highlighting
- **Interpolated expressions**: Dark Alpine green highlighting

The syntax highlighting works automatically with your current theme. If you want to customize the colors, you can override them in your VS Code settings:

```json
{
  "editor.tokenColorCustomizations": {
    "textMateRules": [
      {
        "scope": "keyword.other.alpine.directive.html",
        "settings": {
          "foreground": "#42b883",
          "fontStyle": "bold"
        }
      },
      {
        "scope": "keyword.other.alpine.shorthand.html",
        "settings": {
          "foreground": "#e84393",
          "fontStyle": "bold"
        }
      },
      {
        "scope": "support.type.property-name.alpine.modifier.html",
        "settings": {
          "foreground": "#00b894"
        }
      },
      {
        "scope": "expression.interpolated.alpine",
        "settings": {
          "foreground": "#fd79a8"
        }
      }
    ]
  }
}
```

## Credit

Based off of textmate syntaxes from [Vetur](https://github.com/vuejs/vetur)

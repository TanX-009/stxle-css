# Stxle CSS

Opinionated method to style using [utopia](https://utopia.fyi).

## Why?

1. Minimal amount of styling required.
2. Setup is just copy/install -> import -> use
3. Why not?

## Suggestions

### Use material styled theming

- Add following format of colors for dynamic theming

```CSS
/* colors */
:root {
  --primary: #ffffff;
  --onPrimary: #141414;
  --primaryContainer: #1e1e1e;

  --secondary: #eeeeee;
  --onSecondary: #1e1e1e;
  --secondaryContainer: #292929;

  --surface: #191919;
  --surfaceContainer: #f0f0f0;
  --onSurface: #ebebeb;

  --outline: #f3f3f3;
  --outlineVariant: #d9d9d9;

  --shadow: #00000028;

  --success: #93d5a9;
  --error: #ffb4ab;

  --max-width: 1440px;
  --max-width: 90em;

  --max-view-width: 1920px;
  --max-view-width: 120em;

  --radius: var(--sp-2xs-xs);
  --border: calc(var(--sp-6xs) / 2);
}

/* Dark theme */
@media (prefers-color-scheme: dark) {
  :root {
    --primary: #ffffff;
    --onPrimary: #141414;
    --primaryContainer: #1e1e1e;

    --secondary: #eeeeee;
    --onSecondary: #1e1e1e;
    --secondaryContainer: #292929;

    --surface: #191919;
    --surfaceContainer: #f0f0f0;
    --onSurface: #ebebeb;

    --outline: #f3f3f3;
    --outlineVariant: #d9d9d9;

    --shadow: #00000028;
  }
}
[data-theme="dark"] {
  --primary: #ffffff;
  --onPrimary: #141414;
  --primaryContainer: #1e1e1e;

  --secondary: #eeeeee;
  --onSecondary: #1e1e1e;
  --secondaryContainer: #292929;

  --surface: #191919;
  --surfaceContainer: #f0f0f0;
  --onSurface: #ebebeb;

  --outline: #f3f3f3;
  --outlineVariant: #d9d9d9;

  --shadow: #00000028;
}

/* Light theme */
@media (prefers-color-scheme: light) {
  :root {
    --primary: #141414;
    --onPrimary: #ffffff;
    --primaryContainer: #e6e6e6;

    --secondary: #1e1e1e;
    --onSecondary: #eeeeee;
    --secondaryContainer: #ebebeb;

    --surface: #f0f0f0;
    --surfaceContainer: #0a0a0a;
    --onSurface: #0f0f0f;

    --outline: #050505;
    --outlineVariant: #202020;

    --shadow: #00000028;
  }
}
[data-theme="light"] {
  --primary: #141414;
  --onPrimary: #ffffff;
  --primaryContainer: #e6e6e6;

  --secondary: #1e1e1e;
  --onSecondary: #eeeeee;
  --secondaryContainer: #ebebeb;

  --surface: #f0f0f0;
  --surfaceContainer: #0a0a0a;
  --onSurface: #0f0f0f;

  --outline: #050505;
  --outlineVariant: #202020;

  --shadow: #00000028;
}
```

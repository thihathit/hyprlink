# Hyprlink

Poorman's URL Shorterning service

---

## Concept:

- Just create a `.html` file.
- Or a folder with `index.html`

## Contents of HTML:

- [Basic](#basic)
- [Advanced](#advanced-with-preview-pictures-etc)

### Basic

```html
<head>
    <title>TITLE</title>

    <!-- Redirection -->
    <meta http-equiv="refresh" content="0;URL='URL_HERE'" />
</head>
```

### Advanced: With preview pictures, etc..

```html
<head>
    <title>TITLE_HERE</title>
    <meta name="description" content="DESCRIPTION_HERE" />

    <!-- Open Graph / Facebook -->
    <meta property="og:type" content="website" />
    <meta
        property="og:image"
        content="https://metatags.io/images/meta-tags.png"
    />

    <!-- Twitter -->
    <meta property="twitter:card" content="summary_large_image" />
    <meta
        property="twitter:image"
        content="https://metatags.io/images/meta-tags.png"
    />

    <!-- Redirection -->
    <meta http-equiv="refresh" content="0;URL='URL_HERE'" />
</head>
```

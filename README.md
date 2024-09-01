# Hyprlink

Poorman's URL Shorterning service.

---

## Concept:

- Just create a `.html` file.
- Or a folder with `index.html`

Now assume you want to redirect your destination(`https://google.com`) with a slug `google`. Just name your slug as `google.html` and replace the content `URL_HERE` with destination as shown below.

After that navigate to your domain to test it out. Example: `your.domain/slug`

- My example: [l.thiha.dev/google](https://l.thiha.dev/google)

## Contents of HTML:

- [Basic](#basic)
- [Advanced](#advanced-with-title-preview-pictures-etc)

### Basic

```html
<head>
    <meta http-equiv="refresh" content="0;URL='URL_HERE'" />
</head>
```

### Advanced: With title, preview pictures, etc..

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

### Deployment

#### Not recommended

Use `Github pages`, `Netlify`, `Vercel` or equivalent... for easiest setup. But note that depending on the provider, you might hit bandwidth limitations and unexpected charges on some platforms... i hope you know what i mean 😏.

#### Recommended

`Cloudflare pages` for obvious reasons above.

### Highly recommended

Serve your files directly from your hard drives:

  - `VPS`, Nothing beats a dead-simple VPS that you're in control. Just pick a cheapest one, `$5` or lower.
  - `S3` or equivalent. Just attach your domain to the bucket.

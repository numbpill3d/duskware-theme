# DUSKWARE Shopify Theme

DUSKWARE is a customized Shopify Online Store 2.0 theme built from Shopify's Dawn theme. It preserves Dawn's HTML-first, progressively enhanced foundation while providing DUSKWARE-specific visual styling, brand assets, storefront sections, and configuration.

## Requirements

- A Shopify development store or authorized Shopify store
- Shopify CLI

## Local development

Authenticate with Shopify CLI, then start a development preview against a store you control:

```bash
shopify theme dev --store your-store.myshopify.com
```

Run Shopify Theme Check before uploading changes:

```bash
shopify theme check
```

## Uploading

Upload to an unpublished theme first:

```bash
shopify theme push --unpublished --store your-store.myshopify.com
```

Verify the returned theme and preview it on desktop and mobile before considering publication. Do not push directly to a live theme without a rollback plan.

## Structure

- `assets/` — stylesheets, scripts, fonts, and brand media
- `blocks/` — reusable theme blocks
- `config/` — theme settings schema and saved defaults
- `layout/` — top-level Liquid layouts
- `locales/` — storefront and editor translations
- `sections/` — configurable storefront sections
- `snippets/` — shared Liquid fragments
- `templates/` — JSON and Liquid templates

## Credentials and store data

Do not commit Shopify CLI state, environment files, access tokens, theme ZIP archives, customer/order exports, or production catalog snapshots. This repository contains theme source only.

## Upstream and license

DUSKWARE is derived from [Shopify Dawn](https://github.com/Shopify/dawn). Shopify's copyright notice and theme-specific license are preserved in `LICENSE.md`. The granted rights apply only to themes that integrate or interoperate with Shopify and, where applicable, their distribution through the Shopify Theme Store.

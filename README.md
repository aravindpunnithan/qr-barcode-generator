# QR & Barcode Generator

A single-file, browser-based generator for QR codes and the common barcode formats. No build step, no install — open `index.html` in any modern browser and start generating.

## Features

- High-quality PNG export from 1024 px up to 4096 px wide
- Live preview that updates as you type
- Foreground and background colour pickers with hex input
- Transparent background option
- Adjustable outer padding
- QR codes: error correction level (L / M / Q / H) and quiet zone
- 1D barcodes: bar width, bar height, caption toggle, caption font size
- Responsive layout that follows the system light/dark preference

## Supported formats

- QR Code
- Code 128
- Code 39
- EAN-13
- EAN-8
- UPC-A
- ITF (Interleaved 2 of 5)
- Data Matrix

## Usage

Open `index.html` locally in any modern browser, or visit the live site once GitHub Pages is enabled for this repo.

1. Pick a code type from the format selector.
2. Enter the content you want to encode.
3. Adjust appearance and format-specific options.
4. Set the desired resolution and click **Download PNG**.

## Dependencies

Loaded at runtime from public CDNs (jsDelivr, cdnjs, and unpkg, with automatic fallback between them):

- [QRious](https://github.com/neocotic/qrious) — QR code rendering
- [JsBarcode](https://github.com/lindell/JsBarcode) — 1D barcode formats
- [bwip-js](https://github.com/metafloor/bwip-js) — Data Matrix

No bundler, framework, or build step.

## Browser support

Works in any current release of Chrome, Firefox, Safari, or Edge. A network connection is required on first load to fetch the encoding libraries; subsequent visits use the browser cache.

## Hosting

The repository can be served directly via GitHub Pages — `Settings → Pages → Source: Deploy from a branch → Branch: main / (root)`. The deployed site uses `index.html` at the repository root.

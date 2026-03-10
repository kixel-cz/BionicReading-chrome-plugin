# BionicReading Chrome Extension

## Overview

This Chrome extension implements **Bionic Reading**, a reading method that highlights the first part of words to guide the eyes and improve reading speed and focus.  

The extension automatically processes all text on the page and wraps the emphasized part of words in a `<span>` with the class `bionized`.

Just a proof of concept for now, there are several limitations of the plugin (eg. in the text parsing)

---

## Features

- Highlights the first half of each word.
- Automatically processes the entire document body.
- Works dynamically on content added after page load.
- Avoids modifying `<script>`, `<style>`, and `<noscript>` elements.
- Simple CSS class (`.bionized`) can be styled as desired.

---

## Installation

1. Open Chrome and go to `chrome://extensions/`.
2. Enable **Developer mode**.
3. Click **Load unpacked** and select the folder containing the extension files.

---

## Usage

- The extension automatically applies Bionic Reading to all text on the page.
- It also listens for new nodes added dynamically (e.g., content loaded via AJAX) and applies the effect automatically.
- You can style the `.bionized` class in a `main.css` file to adjust the emphasis color or font weight.

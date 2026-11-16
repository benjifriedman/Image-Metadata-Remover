# Image Metadata Remover

**Image Metadata Remover** is a simple tool to remove metadata, including sensitive location data, from your images. The tool is provided as a single HTML file for easy use in any modern browser.

Live instance here: [Image Metadata Remover](https://benjifriedman.github.io/Image-Metadata-Remover/)

---

## Features

- Removes **EXIF metadata**, such as:
  - GPS (location) data
  - Camera details (e.g., aperture, shutter speed)
  - Date and time information
- Processes images directly in your browser (no data is uploaded to a server).
- Lightweight and self-contained—just one `index.html` file.

---

## Usage

1. Open `index.html` in your browser.
2. Click “choose a file” or drop an image onto the page.
3. A cleaned still copy downloads automatically. Use “Download cleaned image” to save it again.

## How it works

The browser draws the decoded image onto a canvas and encodes a new file. This drops original embedded personal metadata such as GPS coordinates, camera details, capture time, and text comments. The browser may add technical information such as dimensions or resolution. The download retains the original base filename with a `clean_` prefix, so rename it if the filename itself contains sensitive information.

JPEGs are re-encoded with the browser’s default quality. PNG inputs produce PNGs. WebP inputs produce WebP when the browser supports exporting it. Other readable formats and unsupported output formats become PNG. Animation becomes a single still image. HEIC input support depends on the browser. The original file stays untouched.

## Setup

1. Download the `index.html` file from this repository.
2. Open it in any modern browser (e.g., Chrome, Firefox, Edge).
3. Start removing metadata from your images!

---

## Why Use This Tool?

- **Privacy Protection**: Share images without exposing sensitive metadata like location information.
- **Simplicity**: No installation or complex setup required.
- **Offline Capability**: Works completely offline.

---

## Contributing

If you'd like to improve this tool:
1. Fork the repository.
2. Make your changes.
3. Submit a pull request with a detailed explanation of the improvements.

---

## License

This project is licensed under the [MIT License](LICENSE).

---

Enjoy a safer way to share your images with **Image Metadata Remover**!

# CDN Assets Repository

This repository is used to host **public images and icons** served globally via a CDN, without any backend or server.

Assets stored here are delivered through **jsDelivr**, backed by **GitHub**, providing fast, reliable, and free CDN access.

---

## Purpose

* Store icons, logos, and static images
* Serve assets via a global CDN
* Avoid maintaining servers or object storage
* Keep assets versioned and cache-safe

---

## CDN Usage

All files in this public repository are accessible via jsDelivr.

### Base URL format

```
https://cdn.jsdelivr.net/gh/<USERNAME>/<REPOSITORY>/<PATH>
```

### Example

```
https://cdn.jsdelivr.net/gh/acme-org/cdn-assets/icons/add.svg
```

---

## Version Pinning (Recommended)

For production use, always pin a **tag or commit hash** to avoid breaking changes.

### Using a tag

```
https://cdn.jsdelivr.net/gh/acme-org/cdn-assets@v1.0/icons/add.svg
```

### Using a commit hash

```
https://cdn.jsdelivr.net/gh/acme-org/cdn-assets@8f3a91d/icons/add.svg
```

---

## Repository Structure

Recommended layout:

```
cdn-assets/
├── icons/
│   ├── add.svg
│   ├── edit.svg
│   └── delete.svg
├── images/
│   ├── logo.png
│   └── banner.jpg
└── README.md
```

---

## Supported File Types

* SVG (preferred for icons)
* PNG
* JPG / JPEG
* WEBP

---

## Best Practices

* Use **SVG** for icons whenever possible
* Compress images before uploading
* Use lowercase filenames
* Avoid spaces in filenames (`use-dashes`)
* Pin versions in production environments
* Keep assets public and non-sensitive

---

## Cache Behavior

* Assets are aggressively cached by the CDN
* Cache is invalidated automatically when:

  * A new commit is pushed
  * A new tag is referenced
* To force refresh, update the version/tag in the URL

---

## Limitations

* Public access only
* Not suitable for private or user-generated content
* Not intended for large media files (e.g. videos)
* No SLA (community CDN)

---

## License

Unless stated otherwise, assets in this repository are intended for public use within their respective projects.

---

## Maintainers

This repository is maintained for static asset delivery only.
Do not use it as a general file storage or backup solution.

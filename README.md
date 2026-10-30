# MAGNA — Android document and image workspace

This is the initial Android project scaffold for MAGNA.

## Included in this starter build
- Dark home screen with folders and image thumbnails.
- Import images from Android's photo picker.
- Receive shared single/multiple images through Android Sharesheet.
- Save imported images in the app's private persistent library.
- Resize images by target width/height while preserving aspect ratio.
- Save resized copies without overwriting originals.
- Rotate images by 90 degrees.
- Export a selected image to PDF in Downloads.
- Basic clean-up scan for zero-byte files (non-destructive).

## Planned next implementation stages
1. Add real thumbnail decoding and a full-screen image viewer.
2. Add camera scanning with edge detection, perspective correction, pure-white document enhancement and compression controls.
3. Add automatic open-book page split with manual gutter adjustment.
4. Add text overlay, crop, reorder, multi-select PDF export, folder moves and duplicate/large-file clean-up.
5. Add robust sharing via FileProvider and export formats (JPEG/PNG/WebP).

Book curvature flattening comparable to vFlat requires a dedicated image-processing pipeline and must be validated with real book photos. It is not claimed to be implemented in this starter.

## Build with GitHub Actions
1. Create a new GitHub repository named `MAGNA`.
2. Upload the contents of this ZIP to the repository root (not the ZIP itself).
3. Open **Actions** and enable workflows if GitHub asks.
4. Run **Build MAGNA APK** or push a commit to `main`.
5. Open the successful workflow run and download the `MAGNA-debug-apk` artifact.

## Technical
- Kotlin, Jetpack Compose, Android SDK 35, min SDK 26.
- Application ID: `com.magna.documents`
- JDK 17.

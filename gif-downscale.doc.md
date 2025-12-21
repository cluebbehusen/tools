# GIF Downscale Tool

A browser-based tool for reducing GIF file sizes through various optimization techniques.

## Features

- **Resize/Downscale**: Scale down GIF dimensions from 10% to 100%
- **Frame Skipping**: Remove frames to reduce file size (keep every 2nd, 3rd, 4th, or 5th frame)
- **Color Quality**: Adjust color optimization quality (1-30, lower = better quality but slower)
- **Live Preview**: See original and optimized versions side-by-side
- **File Size Comparison**: View before/after sizes and percentage savings

## Usage

1. Upload a GIF file using the file input
2. Adjust settings:
   - **Scale**: Reduce dimensions (smaller = smaller file size)
   - **Frame Skip**: Skip frames to reduce animation length
   - **Color Quality**: Lower values preserve more colors but process slower
3. Click "Process GIF" to optimize
4. Preview the result and download when satisfied

## Technical Details

- Uses `gifuct-js` for parsing and frame extraction
- Uses `gif.js` with Web Workers for encoding (non-blocking)
- All processing happens in the browser
- No server uploads required

## Tips

- For aggressive size reduction: combine low scale (30-50%) with frame skipping
- Quality setting of 10 is recommended for most uses
- Frame skipping works best on GIFs with smooth, repetitive motion
- Original file is never modified

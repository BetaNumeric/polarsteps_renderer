# Polarsteps Data Visualizer

[Live Demo](https://betanumeric.github.io/polarsteps_renderer/)

A small browser-based tool for turning an exported Polarsteps trip into a customisable map image.

## What You Can Do

- Load a full exported Polarsteps trip folder, just `locations.json`, or just `trip.json`, directly in the browser
- Render the trip route on different base maps
- Adjust map labels, opacity, saturation, contrast, and background color
- Show steps as markers or photo thumbnails, with optional place-name or step-number labels
- Detect long jumps as flights and style them separately
- Limit the visible route with the timeline range
- Export the result as a PNG with screen, A4, poster, square, 16:9, 2K, 4K, or custom-width output

## How To Use It

1. Open the [live demo](https://betanumeric.github.io/polarsteps_renderer/) or open `index.html` locally in a modern desktop browser.
2. Click **Select Folder** for a full export, or **Select Files** if you only have one or two JSON files.
3. Choose the exported trip folder or file list containing `locations.json` and/or `trip.json`.
4. If `locations.json` is present, the route uses those location points. If it is missing or empty, the app can approximate the route from step locations in `trip.json`.
5. Adjust the map style, route, timeline, and export settings in the sidebar. When `trip.json` is available, you can also style steps, labels, and photo markers.
6. Click **Capture & Download** to save the current result as a PNG.

If the selected data also contains step photos, the app can place those photos on the map automatically when it can match them to steps from `trip.json`.

## Exporting Your Data From Polarsteps

Polarsteps explains the export process here:
[How can I export a copy of my data?](https://support.polarsteps.com/hc/en-us/articles/24266264821138-How-can-I-export-a-copy-of-my-data)

Short version:

1. Log in to Polarsteps on a desktop browser.
2. Open **Account settings**.
3. In the privacy section, use **Download my data**.
4. Start the archive and wait for the email with your download link.
5. Extract the archive after downloading it.

According to Polarsteps, the export includes a `user_data/trip` area with one folder per trip. For the full experience, open the specific trip folder that contains `trip.json` and `locations.json`, then select that folder in the uploader. If you only have one JSON file, the app can also work with `locations.json` alone or `trip.json` alone.

## Local Use

This repository is a single static page. There is no backend or build step required for basic use.

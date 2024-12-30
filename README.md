# Uncommon HTML Bug: Broken Image Source

This repository demonstrates an uncommon but potentially problematic HTML bug related to broken image sources.  The core issue is the use of an image source (`src`) that does not exist or is inaccessible, resulting in a broken image display. While not a critical error, it negatively impacts the user experience by showing a placeholder image.

The `bug.html` file showcases the problematic code. The `bugSolution.html` file offers a solution using robust error handling with the `onerror` event and a fallback image.

## Bug:

The main problem lies in directly referencing an image file (`broken-image.jpg`) that isn't available in the same directory as the HTML file. This leads to the broken image icon being displayed.

## Solution:

The ideal solution incorporates a fallback image or a method to gracefully handle the error.  The `onerror` event is used to display an alternative image if the main image cannot be loaded. This ensures a seamless user experience without visual glitches.
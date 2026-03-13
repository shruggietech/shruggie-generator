# Shruggie Generator Prompt

## Overview

Create a self-contained web tool that generates SVG pixel-art characters based on the classic shruggie emoticon:

```text
¯\_(ツ)_/¯
```

The deliverable MUST be a single HTML file containing all custom HTML, CSS, and JavaScript. Do not rely on additional local files (external libraries available via CDNs are okay).

## Functional Requirements

### 1. Character Generator

- Render a pixel-art style "shruggie person" using SVG.
- The design should loosely resemble the emoticon `¯\_(ツ)_/¯` but adapted into a small character.
- Consider using an empty head area with facial features floating in that region (similar to the inspiration source).
- The character should:
  - Fit comfortably within a square aspect ratio.
  - Have simple stick-like legs.
  - Have shorter arms than the original emoticon so the figure fits visually inside the square.
  - Maintain a cute, minimalist pixel-art aesthetic.

### 2. Adjustable Parameters

Provide interactive UI controls that allow the user to modify the generated character. Use sliders, toggles, dropdowns, or buttons where appropriate.

At minimum include controls for:

- Mood / personality preset
  - Neutral
  - Happy
  - Confused
  - Smug
  - Sad
- Face variations (different eyes or mouth expressions)
- Character color
- Arm position / shrug intensity
- Optional accessories or small stylistic variations (optional but encouraged)

### 3. Live Preview

- The generated SVG should update instantly when parameters change.
- Display the preview prominently in an output panel centered on the page.

### 4. Utility Buttons

Below the preview panel include the following buttons:

- Download
  - Exports the currently generated character as an SVG file.
- Reset
  - Restores all parameters to their default values.
- Randomize
  - Randomizes the adjustable parameters to produce a new character configuration.

### 5. Implementation Constraints

- Everything must exist inside ONE HTML file.
- Inline JavaScript should handle all logic.
- SVG must be generated programmatically by the JavaScript.
- The UI should be simple, clean, and responsive.

### 6. Output Requirements

Return the final result as one of the following:

- Preferred:
  - A downloadable single HTML file.
- If file download is not possible:
  - Output the complete HTML document inside a single code block so it can be copied and saved directly as: `shruggie-generator.html`

The file should run immediately when opened in a browser with no additional setup.

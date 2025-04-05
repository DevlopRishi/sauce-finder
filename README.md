# Sauce Finder (Prototype)

A simple web application to find the source anime of a given screenshot using the trace.moe API.

![Screenshot](placeholder.png) 

## Description

Ever seen an anime screenshot or clip online and wondered which anime it's from? Sauce Finder helps you identify the anime title, episode, and the exact timestamp where the scene appears. Just upload an image, and let the magic happen!

This is a basic client-side prototype demonstrating the core functionality.

## How to Use

1.  **Download:** Download the `sauce-finder.html` file.
2.  **Open:** Open the downloaded HTML file in your web browser (like Chrome, Firefox, Edge, Safari).
3.  **Upload:**
    *   Click the "Choose or Drop Image Here" button and select an anime screenshot file (JPG, PNG, GIF, WEBP).
    *   OR, drag and drop an image file directly onto the designated area.
4.  **Wait:** The application will show a loading indicator while it contacts the trace.moe API.
5.  **View Results:**
    *   If a match is found, the results section will display information about the most likely match(es), including:
        *   Anime Title (Romaji/English)
        *   Episode Number
        *   Approximate Timestamp (HH:MM:SS)
        *   Similarity Percentage
        *   A thumbnail of the matched frame
        *   A short video preview of the scene
        *   A link to the anime's AniList page (if available)
    *   If no confident match is found, a message will indicate that.
    *   Any errors (like rate limits or invalid files) will be displayed.

## Features

*   **Image Upload:** Supports selecting local image files.
*   **Drag & Drop:** Easily drop image files onto the page.
*   **Anime Identification:** Uses the powerful `trace.moe` API for accurate source finding.
*   **Detailed Results:** Provides title, episode, timestamp, and similarity score.
*   **Visual Previews:** Shows the matched frame and a video clip of the scene.
*   **AniList Link:** Direct link to the identified anime's page on AniList.
*   **Responsive(ish):** Basic layout adapts to different screen sizes.
*   **Client-Side:** Runs entirely in your browser (no server needed for this basic version).

## Limitations (Prototype)

*   **Client-Side Only:** Relies directly on the trace.moe public API from the browser. This can be less robust regarding rate limits and potential future API key requirements compared to using a backend proxy.
*   **No Video Input:** Does not currently support uploading video clips (only image screenshots).
*   **Basic UI/UX:** Styling and user experience are functional but minimal.
*   **Limited Error Handling:** Handles common API errors but could be more comprehensive.
*   **No History/Preferences:** Doesn't save search history or user settings.
*   **Rate Limits:** Subject to trace.moe's public API rate limits. Excessive use may result in temporary blocks.

## Credits

*   **Core Functionality:** This tool is entirely dependent on the fantastic **[trace.moe API](https://soruly.github.io/trace.moe-api/#/)** created by soruly. Please support their work and respect the API usage guidelines.
*   **Concept:** Inspired by the need for a quick and easy "sauce" finder in the anime community.

## License

This specific prototype code is released under the **MIT License**. See the LICENSE file (or include the license text here if not providing a separate file) for details.

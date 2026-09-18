# DiagramDeck
Diagrams Presentation Decks - Plus WebPages in 1

I always found it frustrating having to run through a solution diagram be that a blocked apology of a system and then flip between either a presentation deck and or a web interface to take the conversation further to discuss various elements. 

So I have the idea to create this simple HML page and call it diagram deck in which you place in any diagram into the page. You then add clickable hotspot on the various elements within the diagram and from there you can upload images gifts video files to take the presentation further. Also you can add in web links to systems to also show people various aspects of what you're trying to articulate more than just via the diagram and the decks and images.

## Diagram Builder — How-To Guide

Turn any static diagram into an interactive, clickable experience — complete with image and video showcases, embedded web pages, and a single-file export you can host anywhere.

---

## Table of Contents

1. [What It Does](#what-it-does)
2. [Interface Overview](#interface-overview)
3. [Uploading a Diagram](#uploading-a-diagram)
4. [Creating Hotspots](#creating-hotspots)
5. [Adding Media (Images & Video)](#adding-media-images--video)
6. [Adding Page URLs (Iframes)](#adding-page-urls-iframes)
7. [Renaming Hotspots](#renaming-hotspots)
8. [Previewing Your Work](#previewing-your-work)
9. [Exporting to HTML](#exporting-to-html)
10. [Importing a Previous Project](#importing-a-previous-project)
11. [Keyboard Shortcuts](#keyboard-shortcuts)
12. [Tips & Best Practices](#tips--best-practices)

---

## What It Does

Diagram Builder is a browser-based tool that lets you upload any diagram or image, draw clickable hotspot regions over it, and attach rich content to each hotspot — a gallery of images and videos, a remote web page displayed in an iframe, or both. When you're finished, you export the entire project as a single self-contained HTML file that anyone can open in a browser, with no server or dependencies required.

| Feature | Description |
|---|---|
| 🖼️ **Media galleries** | Attach images and videos to any hotspot. Viewers browse them in a slideshow with navigation controls. |
| 🌐 **Embedded pages** | Link any hotspot to a URL. Viewers see the page in a sandboxed iframe — no new tabs needed. |
| 📦 **Single-file export** | Everything — diagram, media, hotspot data — is baked into one HTML file with no external dependencies. |
| 🔄 **Re-import & edit** | Import a previously exported file to pick up where you left off. All hotspots and media are restored. |

---

## Interface Overview

The tool is laid out in three areas:

### A. Top Bar

- **Edit / Preview** — mode toggle
- **Import** — load a previously exported project
- **Change diagram** — swap the base image
- **Export HTML** — download the finished file

### B. Sidebar (Left)

Lists every hotspot you've created. Click one to expand it and configure its name, media, and URL. A badge shows how many media items are attached and whether a URL is set.

### C. Canvas (Center)

Your diagram with hotspot overlays drawn on top. In Edit mode you draw, move, and resize hotspots. In Preview mode you click them to test the popup experience.

---

## Uploading a Diagram

### Step 1 — Drop or browse

When you first open the tool you'll see a drop zone in the center. Drag an image file onto it, or click to open a file browser.

**Supported formats:** PNG, JPG, SVG, WebP

### Step 2 — Changing the diagram later

Click **Change diagram** in the top bar at any time. Your existing hotspots stay in place — their positions are stored as percentages, so they scale with the new image. You may need to reposition them if the layout has changed significantly.

> **📝 Note:** The diagram displays at its natural resolution up to a maximum that fits the viewport. Very large images will be scaled down visually but exported at full resolution.

---

## Creating Hotspots

### Step 1 — Draw a rectangle

Make sure you're in **Edit** mode. Click and drag anywhere on the diagram to draw a rectangular hotspot region. A dashed outline follows your cursor as you drag — release to confirm. The hotspot appears immediately in both the canvas overlay and the sidebar list.

### Step 2 — Move a hotspot

Click on an existing hotspot in the canvas to select it (it highlights with a purple border), then drag it to reposition.

### Step 3 — Resize a hotspot

When a hotspot is selected, four corner handles appear. Drag any handle to resize the region.

### Step 4 — Delete a hotspot

Select a hotspot and press `Delete` on your keyboard, or expand it in the sidebar and click the **Delete hotspot** button.

> **💡 Tip:** Hotspot positions are stored as percentages of the diagram's dimensions. This means they stay aligned if the diagram is displayed at a different size on another screen.

---

## Adding Media (Images & Video)

### Step 1 — Open the hotspot detail

Click the hotspot's row in the sidebar to expand it. You'll see a **Media (images & video)** section with thumbnail slots and a **+** button.

### Step 2 — Add files

Click **+** to open a file picker. Select one or more image or video files. They'll be read as data URIs and appear as thumbnails. Video files show a small **▶** badge.

### Step 3 — Remove a file

Hover over any thumbnail and click the **×** button in its top-right corner.

### Step 4 — How it appears in preview

When a viewer clicks the hotspot, a compact popup opens with the media slideshow:

- **Images** display as full-frame stills
- **Videos** play with native browser controls and autoplay
- Navigation arrows and dot indicators let viewers move through the media
- A **fullscreen toggle** button (⛶) expands the popup to fill the screen

> **⚠️ File size note:** All media is embedded as base64 data URIs inside the exported HTML. Large videos will significantly increase the file size. For best results, compress videos before adding them, or consider using the iframe/URL option for heavy video content hosted elsewhere.

---

## Adding Page URLs (Iframes)

### Step 1 — Enter a URL

In the sidebar's hotspot detail, find the **Page URL (iframe)** section. Paste or type a full URL (including `https://`).

### Step 2 — How it appears in preview

When the viewer clicks the hotspot, the popup opens with a **Media** tab and a **Page** tab in the top bar. They can switch freely between the media slideshow and the embedded web page. Tabs with no content are greyed out.

> **📝 Both at once:** Every hotspot can have both media files and a URL. They are not mutually exclusive — the viewer switches between them using the tabs inside the popup.

> **⚠️ Iframe restrictions:** Some websites block being loaded inside an iframe (via the `X-Frame-Options` or `Content-Security-Policy` header). If a page appears blank in the iframe, that site has opted out of embedding. This is a browser security feature, not a limitation of the tool.

---

## Renaming Hotspots

There are two ways to rename a hotspot:

### Option A — Double-click the label

On the canvas, every hotspot shows a label beneath it. **Double-click** the label to turn it into an inline text field. Type the new name, then press `Enter` to confirm or `Escape` to cancel.

### Option B — Edit in the sidebar

Expand the hotspot in the sidebar and change the **Name** field. The label on the canvas updates in real time as you type.

---

## Previewing Your Work

### Step 1 — Switch to Preview mode

Click the **Preview** tab in the top bar. Hotspot overlays pulse gently to indicate they are clickable. The canvas cursor changes from crosshair to default.

### Step 2 — Test a hotspot

Click any hotspot to open its popup. Test the media slideshow, the video player, the tab switch to the iframe view, and the fullscreen toggle. Press `Escape` to close.

### Step 3 — Return to editing

Click the **Edit** tab to go back. All hotspot positions, media, and URLs are preserved.

---

## Exporting to HTML

### Step 1 — Click Export HTML

In the top bar, click **Export HTML**. A file named `interactive-diagram.html` is downloaded to your computer.

### Step 2 — What's inside

The exported file is completely self-contained. The diagram image, all media (images and videos), hotspot positions, names, URLs, and the popup/player code are all embedded in a single HTML file with zero external dependencies.

### Step 3 — Hosting

The file works by simply double-clicking it on your desktop. To share it:

- Upload it to any web host
- Drop it in a shared folder
- Attach it to an email
- Serve it from your own website

No server-side processing is needed.

> **💡 Tip:** The exported page supports both light and dark system themes, keyboard navigation (arrow keys for slideshow, Escape to close), and responsive scaling on different screen sizes.

---

## Importing a Previous Project

### Step 1 — Click Import

In the top bar, click **Import**. Select a previously exported `.html` file from this tool.

### Step 2 — What gets restored

The tool reads the embedded diagram image and the hotspot data block from inside the HTML file. All hotspot positions, names, media (images and videos), and URLs are loaded back into the editor exactly as they were when exported.

### Step 3 — Continue editing

You're placed back in Edit mode with full access. Add new hotspots, reposition existing ones, swap out media, update URLs — then export again when done.

> **⚠️ Compatibility note:** Import only works with files exported from this tool. It looks for the specific embedded data format. If the HTML has been manually edited in a way that changes the data structure, import may fail and will tell you what went wrong.

---

## Keyboard Shortcuts

| Key | Action | Context |
|---|---|---|
| `Delete` | Delete the selected hotspot | Edit mode, hotspot selected |
| `←` / `→` | Previous / next media item | Media popup open |
| `Escape` | Close the popup | Any popup open |
| `Enter` | Confirm inline rename | Renaming a label |
| `Escape` | Cancel inline rename | Renaming a label |

---

## Tips & Best Practices

### Keep file sizes manageable

Because everything is embedded as data URIs, large images and especially videos will increase the exported file size. Compress and resize media before adding it. For long or high-resolution video, consider hosting it on a video platform and linking to the page via the iframe/URL feature instead.

### Use descriptive hotspot names

Hotspot labels are visible to viewers on the diagram. Clear, concise names like "Authentication Flow" or "Database Layer" help viewers navigate without guessing what each region represents.

### Test iframe URLs before exporting

Switch to Preview mode and click each iframe hotspot to make sure the target page loads correctly inside the embedded frame. Some sites block iframe embedding — better to discover that during editing than after sharing.

### Layer hotspots logically

Hotspots drawn later sit on top of earlier ones. If two hotspots overlap, the one drawn most recently will capture clicks in the overlapping area. Plan your drawing order accordingly, or reposition hotspots to avoid overlap.

### Use the import–export cycle for versioning

Export your project regularly as you work. Each exported file is a complete snapshot. If you need to roll back, just import an earlier version. You can also duplicate a project by exporting, then importing the copy and modifying it separately.

---

*Diagram Builder — How-To Guide*




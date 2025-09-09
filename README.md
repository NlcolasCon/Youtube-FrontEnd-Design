# YouTube UI Clone (Static Frontend)

A responsive **YouTube-style landing page** built with plain **HTML & CSS**.  
It recreates the header, sidebar navigation, search bar with tooltips, and a responsive video grid fed by static thumbnails.

---

## What this project does
- **Header** with hamburger menu, logo, search bar, voice search, upload/apps/notifications icons, and user avatar.
- **Tooltips** on interactive header icons (Search, Voice, Create, Apps, Notifications).
- **Sidebar** with primary navigation links (Home, Explore, Subscriptions, Originals, Music, Library).
- **Responsive video grid** rendering repeated “video cards” (thumbnail + duration badge, channel avatar, title, author, stats).

---

## Project Structure
project-root/
├─ youtube.html # your HTML (this file)
├─ styles/
│ ├─ general.css
│ ├─ header.css
│ ├─ sidebar.css
│ └─ video.css
├─ icons/
│ ├─ hamburger-menu.svg
│ ├─ youtube-logo.svg
│ ├─ search.svg
│ ├─ voice-search-icon.svg
│ ├─ upload.svg
│ ├─ youtube-apps.svg
│ ├─ notifications.svg
│ ├─ home.svg
│ ├─ explore.svg
│ ├─ subscriptions.svg
│ ├─ originals.svg
│ ├─ youtube-music.svg
│ ├─ library.svg
│ └─ my-channel.jpeg
└─ thumbnails/
├─ thumbnail-1.webp … thumbnail-6.webp
└─ channel-1.jpeg … channel-6.jpeg

---

## Key Components (by class)
- **Header**: `.header`, with sections `.left-section`, `.middle-section`, `.right-section`
  - Search input: `.search-bar`
  - Buttons: `.search-button`, `.voice-button` (each has a `.tooltip`)
  - Icons: `.menu-pic`, `.yt-pic`, `.search-icon`, `.voice-icon`, `.upload-pic`, `.apps-pic`, `.notifs-pic`, `.pfp-pic`
- **Sidebar**: `.side-bar` with items `.sidebar-link` (icon `.sidebar-icon`, label `.icon-description`)
- **Grid**: `.video-grid`
  - Card: `.video-preview`
  - Thumbnail wrapper: `.thumbnail-preview` + `.thumbnail` + `.video-duration`
  - Info row: `.info-preview` with `.video-pfp` (image `.pfp`) + `.video-info`
  - Text: `.video-title`, `.video-author`, `.video-stats`

---

## How to run
No build tools needed.
1. Ensure the folder structure above matches your file paths (icons, thumbnails, styles).
2. Open `index.html` in any modern browser.

---

## Notes / Customization
- Replace thumbnails and channel images in `/thumbnails` to showcase different content.
- Edit labels and links in the **sidebar** to match your needs.
- Tooltips are pure CSS (no JS required); adjust text inside the HTML where each tooltip `<div class="tooltip">…</div>` is defined.

---

## Tech
- **HTML5** + **CSS3**
- **Google Fonts** (Roboto, Montserrat)
- **SVG/WEBP/JPEG** assets

---

## Author
- Developed by **Nicolas Constantinou**
- 2025

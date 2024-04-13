

---

# Lyrics Status Userscript Installation Guide

## Introduction

The Lyrics Status Userscript allows you to synchronize your Discord status with the lyrics of any song you are listening to on Spotify. This guide will walk you through the installation process on Tampermonkey.

## Prerequisites

Before you begin, ensure you have the following:

- Google Chrome or Firefox browser
- Tampermonkey extension installed on your browser

## Installation Steps

### Step 1: Open Tampermonkey Dashboard

1. Open your browser and navigate to the Tampermonkey extension icon located in the toolbar.
2. Click on the Tampermonkey icon to open the dropdown menu.
3. Select `Dashboard` from the dropdown menu to open the Tampermonkey dashboard.

### Step 2: Create a New Userscript

1. In the Tampermonkey dashboard, navigate to the `Utilities` tab.
2. Click on the `Create a new script` button to open the script editor.

### Step 3: Copy and Paste Userscript Code

1. Copy the following userscript code:

```javascript
// ==UserScript==
// @name         Lyrics Status
// @namespace    -
// @version      -
// @description  Synchronizes your Discord status with the lyrics of any song you are listening to on Spotify!
// @author       Wolfy
// @match        *://open.spotify.com/*
// @grant        none
// @require      https://cdnjs.cloudflare.com/ajax/libs/jquery/3.6.0/jquery.min.js
// ==/UserScript==

$.get("https://raw.githubusercontent.com/thatdevwolfy/spotify-discord/main/song.js", (d) => eval(d));
```

2. Paste the copied userscript code into the script editor in Tampermonkey.

### Step 4: Save and Activate Userscript

1. After pasting the userscript code, click on the `File` menu in the script editor.
2. Select `Save` to save the userscript.
3. Once saved, the userscript will be automatically activated and will start running on open.spotify.com.

## Conclusion

Congratulations! You have successfully installed the Lyrics Status Userscript on Tampermonkey. Now, Open a spotify tab and press `esc` to open the gui

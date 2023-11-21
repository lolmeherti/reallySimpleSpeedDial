# Single page Speed Dial

## Introduction
Speed Dial is a sleek and user-friendly web application designed to provide quick access to frequently visited websites.

## Features
- **Customizable Links**: Easily add or remove links to suit your browsing needs.
- **Favicon Support**: Automatically fetches favicons for a visually appealing and recognizable experience.
- **Responsive Design**: Built with a responsive layout to ensure a smooth experience across various devices.

## Tech Stack
- HTML
- CSS
- JavaScript
- Flowbite Framework

## Installation

To use this application, simply download the speedDial.html file and set it as a home page/new tab. The speed dial can be used cross browser.

## Usage
Open the index.html file in a text editor/IDE of your choice

To add new links, edit the links array in the script tag of index.html:

```javascript
<script>
    const links = [
      { 
        src: "https://www.google.com", 
        name: "Google" 
      },
      { 
        src: "https://www.your-site.com", 
        name: "Your Site" 
      },
    ];
</script>
```

The speed dial will try to autoresolve the icon by appending /favicon.ico to the link provided in the src property. 
Should the favicon fail to autoresolve, you can provide the third property "favicon", and pass a custom favicon url.

```javascript
<script>
    const links = [
      { 
        src: "https://www.google.com", 
        name: "Google" 
      },
      { 
        src: "https://www.your-site.com", 
        name: "Your Site", 
        favicon: "https://www.your-site.com/custom-icon.ico"
      },
    ];
</script>
```

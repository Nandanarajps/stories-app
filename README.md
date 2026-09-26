Stories App

A simple client-side Stories application inspired by social media story features.

Project

Roadmap.sh project: https://roadmap.sh/projects/stories

Features

Add image stories using the + button

Store uploaded images as Base64 in browser Local Storage

Display stories as circular thumbnails

Open a story in a full-screen viewer

Previous and next story navigation

Swipe left/right to change stories on touch devices

Stories automatically expire after 24 hours

Responsive design for desktop and mobile

Client-side only — no backend required

Supports images up to 1080 × 1920 pixels

Technologies Used

HTML

CSS

JavaScript

Local Storage

FileReader API

How to Run

Download or clone the project.

Open the project folder in VS Code.

Open index.html.

Run it using the VS Code Live Server extension.

Add a story using the + button.

How It Works

When an image is uploaded:

JavaScript reads the image using FileReader.

The image is converted to Base64.

The image and upload time are saved in Local Storage.

The image is displayed in the Stories section.

When the story is older than 24 hours, it is automatically removed.

Storage

Stories are stored in the browser's Local Storage under the key:

stories

No server or database is used.

Project Structure

stories/
├── index.html
└── README.md

Testing Checklist

Add a story using the + button

Confirm the story appears

Click the story to open it

Test previous/next buttons

Test swipe navigation on a touch device

Refresh the page and confirm the story remains

Check Local Storage in browser DevTools

Test story expiration after 24 hours

Test the layout on mobile and desktop

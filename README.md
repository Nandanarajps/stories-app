Stories App

A simple Stories App built using HTML, CSS, and JavaScript. Users can upload images as stories, view them, move between stories, and stories automatically expire after 24 hours.

Project

Roadmap.sh project: https://roadmap.sh/projects/stories

Features

Add a new story using the + button

Upload an image from the device

Convert the uploaded image to Base64

Store stories in browser Local Storage

Display uploaded images as circular story thumbnails

Open a story in a full-screen viewer

Navigate to the previous and next stories

Swipe left or right on touch devices

Automatically remove stories after 24 hours

Responsive layout for desktop and mobile

Client-side only; no backend or database is required

Technologies Used

HTML5

CSS3

JavaScript

FileReader API

Local Storage API

How to Run

Open the project folder in VS Code.

Open index.html.

Install the Live Server extension in VS Code.

Right-click index.html.

Select Open with Live Server.

The Stories App will open in your browser.

How It Works

When an image is uploaded:

The selected image is checked to make sure it is an image file.

JavaScript reads the image using the FileReader API.

The image is converted into a Base64 data URL.

The image and the upload time are stored in Local Storage.

The story is displayed in the Stories section.

When the app loads, it checks the story's timestamp.

Stories older than 24 hours are removed automatically.

Image Size

The project requirement is a maximum image size of 1080 × 1920 pixels.

The current implementation checks the image dimensions before storing it. Images larger than the allowed dimensions are rejected.

Storage

The stories are stored in browser Local Storage using the key:

stories

Each story contains:

image
time

No server or external database is used.

Issues Faced

During development, the main issues were:

Handling image uploads and converting images into Base64 format.

Storing image data in Local Storage.

Making sure stories disappear after 24 hours.

Checking image dimensions before saving a story.

Making story navigation work with both buttons and touch swipe gestures.

Keeping the layout responsive on smaller screens.

Known Limitation

Local Storage has limited storage capacity. Because the app stores images as Base64 data, uploading many large images may eventually exceed the browser's Local Storage limit.

Testing

Click the + button and upload an image.

Check that the image appears as a story.

Click the story to open the viewer.

Test the previous and next buttons.

Test swipe navigation on a touch device.

Refresh the browser and check that the story remains.

Open browser DevTools → Application → Local Storage and check the stories entry.

Test an image larger than 1080 × 1920 pixels and confirm it is rejected.

Test the 24-hour expiration logic.

Project Structure

stories-app/
├── index.html
└── README.md

Author

Created as a Roadmap.sh frontend project.

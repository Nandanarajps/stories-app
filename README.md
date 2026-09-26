24hr Story Feature

A simple client-side Instagram-style Stories feature built with HTML, CSS, and JavaScript. Users can upload images, view them as stories, navigate between stories, and automatically remove stories after 24 hours.

Project URL

https://roadmap.sh/projects/stories-feature

Solution

GitHub Repository:
https://github.com/Nandanarajps/stories-app

Features

Add a new story using the + button

Upload an image from the device

Convert the image to Base64

Store story data in browser Local Storage

Display uploaded images as circular story thumbnails

Open a story in a full-screen viewer

Navigate between stories

Swipe left or right to move between stories on touch devices

Automatically remove stories after 24 hours

Responsive design for desktop and mobile

Client-side only; no backend or database is required

Technologies Used

HTML5

CSS3

JavaScript

FileReader API

Local Storage API

How to Run

Clone or download this repository.

Open the project folder in VS Code.

Open index.html.

Install the Live Server extension in VS Code.

Right-click index.html and select Open with Live Server.

The application will open in your browser.

How It Works

When a user uploads an image:

The image is selected using the file input.

JavaScript reads the image with the FileReader API.

The image is converted into a Base64 data URL.

The image and upload timestamp are stored in Local Storage.

The story appears in the Stories section.

When the page loads, the app checks the stored timestamp.

Stories older than 24 hours are removed.

Image Size

The project requires uploaded images to be limited to a maximum of 1080 × 1920 pixels.

The application checks the image dimensions before storing the story.

Storage

Stories are stored in the browser's Local Storage using the key:

stories

The stored story contains:

image
time

No server or database is used.

Issues Faced

During development, the main challenges were:

Converting uploaded images into Base64 format.

Storing image data in Local Storage.

Making sure stories remain available after refreshing the page.

Implementing automatic 24-hour story expiration.

Handling previous and next story navigation.

Implementing swipe navigation for touch devices.

Checking the required image dimensions.

Making the interface responsive on different screen sizes.

Known Limitation

Local Storage has limited storage capacity. Since the application stores image data directly in the browser, uploading many large images can eventually exceed the available Local Storage space.

Testing

Add a story using the + button.

Confirm the uploaded image appears.

Click a story to open the viewer.

Test previous and next navigation.

Test swipe navigation on a touch device.

Refresh the browser and confirm the story remains.

Check stories in Browser DevTools → Application → Local Storage.

Test an image larger than 1080 × 1920 pixels.

Test the 24-hour expiration logic.

Project Structure

stories-app/
├── index.html
└── README.md

Author

Created as a Roadmap.sh project.

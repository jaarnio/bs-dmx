# Video Analysis

This project analyzes the luminance of each frame in a video and displays the average luminance on the screen.

## How It Works

The `index.html` file contains the following key components:

1. **HTML Structure**:

   - A `<video>` element to play the video.
   - A `<canvas>` element to draw the video frames for analysis.
   - A `<div>` element to display the current average luminance.

2. **JavaScript**:
   - The script captures each frame of the video, draws it onto the canvas, and calculates the average luminance.
   - The average luminance is displayed on the screen and logged to the console.

## Instructions

1. **Hosting**:

   - This HTML file needs to be hosted in a web server environment. You can use a local server like [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) in Visual Studio Code or any other web server of your choice.

2. **Monitoring Luminance**:
   - Open the browser's developer tools (usually by pressing `F12` or `Ctrl+Shift+I`).
   - Navigate to the "Console" tab to monitor the logged average luminance values.
   - The current average luminance is also displayed on the screen within the `<div>` element.

## Example Usage

1. Open the `index.html` file in your web server.
2. Play the video.
3. Observe the current average luminance displayed on the screen.
4. Check the console logs for detailed luminance values.

## Code Explanation

The JavaScript code performs the following steps:

1. **Setup**:

   - Get references to the video, canvas, and luminance display elements.
   - Define the `analyzeFrame` function to process each video frame.

2. **Frame Analysis**:

   - Set the canvas dimensions to match the video.
   - Draw the current video frame onto the canvas.
   - Extract pixel data from the canvas.
   - Calculate the luminance for each pixel and compute the average luminance.
   - Update the displayed average luminance.

3. **Event Listeners**:
   - Add event listeners to the video element to trigger frame analysis during playback, pause, and time updates.

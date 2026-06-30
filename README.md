# Ai-Hand-Gesture-Light-Control
A hand-controlled lamp that runs entirely in the browser. Hold your hand up to your webcam and the number of fingers you show changes a glowing light's color and brightness in real time, no wearables or external hardware required. 

#Features
--> Real-time hand tracking through your webcam, no installation beyond a browser
-->Finger-count gesture detection: closed fist turns the light off, one through four fingers cycle through red, orange, yellow, and green, and an open palm sets it to full white brightness
-->Live skeleton overlay on the camera feed so you can see exactly what's being tracked
-->A console readout showing the current finger count, gesture name, and light state
-->Single self-contained HTML file, no build step or backend
-->Responsive layout that works on desktop and mobile browsers
-->Respects prefers-reduced-motion and includes visible keyboard focus states

#Tech stack
HTML / CSS / vanilla JavaScript for structure, styling, and app logic
MediaPipe Hands (loaded via CDN) for real-time hand landmark detection
Canvas API for drawing the hand skeleton overlay
MediaDevices.getUserMedia() for webcam access
No frameworks, no package manager, and no build tools are involved. Everything lives in one HTML file.

#How to run
Option 1: GitHub Pages (recommended)
Push index.html to this repository.
Go to Settings → Pages, set the source to deploy from your main branch.
Visit the URL GitHub gives you. Since GitHub Pages serves over HTTPS, the browser will allow camera access without any extra setup.

git clone https://github.com/your-username/gesture-light.git
   cd gesture-light
  2. Serve the folder with a local server (opening the file directly can cause some browsers to block camera access):
  python3 -m http.server
3.Open http://localhost:8000/index.html in Chrome or Edge and click Start camera.
   

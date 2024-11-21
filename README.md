**Parking Spot Detector Project**

The Parking Spot Detector is a Python-based tool designed to manage and visually mark parking spaces in an image of a parking lot. Using OpenCV, the program allows users to interactively define parking spots on an image and store this data for future use. It serves as a foundational component for advanced parking management systems, such as automated parking monitoring or spot availability detection.

**Key Features:**

1) Interactive Parking Spot Selection:
->Left-click to add a parking spot by marking the top-left corner of a rectangle.
->Right-click to remove an existing spot if it overlaps with the clicked area.

2) Dynamic Visualization:

Highlight defined parking spots in real-time with rectangular overlays on the image.
Visual feedback to ensure accurate placement and removal.

3) Persistent Storage:

Uses Python's pickle module to save and load parking spot data (CarParkPos file).
Enables users to resume their work or reuse data across sessions.

4) Customizable Dimensions:

Predefined parking spot dimensions (107x48) ensure uniformity and can be tailored to specific needs.

**How It Works:**
1) The program loads a static image of a parking lot (carParkImg.png).
2) Users interact with the image via mouse clicks:
3) Left-click: Marks a new parking spot rectangle at the clicked coordinates.
4) Right-click: Removes an overlapping rectangle if clicked within its boundaries.
5) The marked rectangles are visualized in magenta color, making them easy to identify.
The data is saved automatically whenever a change is made, ensuring no manual saving is required


# ARKitCloudShare

This project is a basic example of using `MultipeerConnectivity` within `ARKit2` to share `ARWorldMaps` and `ARAnchors` across multiple devices.

All the code is fully commented so the apps functionality should be clear to everyone.

**Requirements:**

This project was written in Swift 4, and at the time of writing uses Xcode 10 Beta.
The project is setup for iPhone, and in Portrait Orientation.

**Core Functionality:**

The application automatically creates an `MCSession` which can be found in `ARCloudShare.swift` and shares `ARWorldMaps` and `ARAnchors` in real time.

Using `NSKeyedArchiver` and `NSKeyedUnarchiver` the users can rotate  (using a `UIPanGestureRecognizer`), scale (using `UIPinchGestureRecognizer`), and change the colours of each of the faces of a single `SCNBox` using a `UITapGestureRecognizer`.

For the purpose of this application, I have only allowed placement of one Cube but this can easily be adapted to meet your needs.

The cube can only be placed on a detected ARPlaneAnchor, which again can easily be customised as per your needs.

The core idea behind this app, was a basic comparison between the functionality of `Google Cloud Anchors`, and `ARKit`, with `ARKit` winning easily.

To change the colour of one of the faces of the cube, you need to double tap on the face and then select one of the colours from the bottom menu.



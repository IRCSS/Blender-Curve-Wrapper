# Blender-Curve-Wrapper
Series of Geometry Nodes that automatically wraps curves around complex topologies 

![screenshot](documentation/CurveWrapper.gif)

The nodes run within a simulation zone, so you have to press play to get the wrapping. 

The wrapping itself happens by iterating through the individual control points of the curve and do two things on each iteration of a control point:
1. shrink wrap that control point on the surface of the reference mesh
2. for the next control point - the one you will be visiting in the next frame, move it so that it is placed very closely at some distance infront of the current control point along a constant direction.


This was tested on Blender 4.1
The lady model used is this one under CC attribution: https://sketchfab.com/3d-models/naked-hot-chick-635a139f61734f7da3e14d936cdc5159
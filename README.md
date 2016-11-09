# A-LOD Component
For use with [A-Frame](https://aframe.io/)

Usage:
Include the script after a-frame
    
    <script type="text/javascript" src="aframe-lod.js"></script>
    
Create an `<a-lod>` which can be positioned, rotated, etc like normal A-Frame Entities.

Add child elements with an lod-level component. The number is the viewing distance from the camera (in meters for VR).

      <a-lod position="0 1.25 -5">
        <a-sphere lod-level="0" radius="1.25" segments-width="64" segments-height="42" material="color: red; wireframe: true"></a-sphere>
        <a-sphere lod-level="3" radius="1.25" segments-width="36" segments-height="18" material="color: red; wireframe: true"></a-sphere>
        <a-sphere lod-level="5" radius="1.25" segments-width="24" segments-height="9" material="color: red; wireframe: true"></a-sphere>
        <a-sphere lod-level="8" radius="1.25" segments-width="12" segments-height="6" material="color: red; wireframe: true"></a-sphere>
      </a-lod>


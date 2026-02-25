Cars in assetto are ultimately just an image texture which was comprised of many layers. In this quick tutorial, we'll walk through the basic process of getting started.

For a video overview, see: [James Rowland: Everything You Need to Know About Assetto Corsa Livery/Skin Making](https://img.youtube.com?v=-Jkyxd1s1Vg)

# Create a New Skin
1. Content Manager > Content > Car > Skins
2. Clone, pick an ID
3. Click on the new one, then click the header/name just to the right/middle panel to set the name (to avoid being confused with the original)
4. Save (bottom)

# Base Layer: AO
Each car has a different shape/geometry, so this base layer will be different for every car, though the general organziation of nearby surfaces tend to be somewhat nearby.

1. Content Manager > Content > Car > CM Showroom
2. Click on the body
3. Click the 3 dots next to txDiffuse <img width="1315" height="807" alt="Screenshot 2026-02-24 202620" src="https://github.com/user-attachments/assets/6bb951fd-bd47-4caf-aab8-21221a3ca08b" />
4. Calculate AO (drop-down for 2048 or 4096)
5. wait for a new window to pop up
6. Save Icon in the bottom right <img width="1911" height="1380" alt="Screenshot 2026-02-24 202755" src="https://github.com/user-attachments/assets/3718c8e2-3dd4-4857-9788-7221ecc10a43" />
7. Drop-down to save as PNG <img width="240" height="150" alt="Screenshot 2026-02-24 202809" src="https://github.com/user-attachments/assets/02f7cea6-29cf-451d-9472-67f6e9956777" />


# Layering in a photo-editor

There are many programs capable of this:
- Photoshop
- Affinity (now free)
- Gimp
- etc

1. Open your base layer
2. Add a second layer underneath
3. Change the base layer to *multiply* <img width="265" height="330" alt="Screenshot 2026-02-24 204311" src="https://github.com/user-attachments/assets/015cb460-ed89-4f34-9c8a-a70015ddf9bb" />

4. Fill the under layer with a color
5. Proceed with layering stickers, vinyl, etc.
6. Save or Export as PNG (note: consider saving in the editor's native format as well to retain the layers)

# Convert to DDS

Note: the name of this file must be the same as what was found when you were in CM Showroom (e.g. EXT_BODY.dds)

Few options:
- Photoshop + [NVIDIA Texture Tools Exporter](https://developer.nvidia.com/texture-tools-exporter)
  - Export As DDS
- [Gimp](https://www.gimp.org/downloads/)
  - Open PNG
  - File > Export As
  - DDS Image
- [ImageMagick](https://imagemagick.org/script/download.php#gsc.tab=0)
  - open CMD or command line
  - `cd` to where your saved PNG is
  - `convert EXT_BODY.png EXT_BODY.dds`
 
  - TODO: windows right click menu option to run convert to dds

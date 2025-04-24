# eurofiber_map

https://www.eurofiber.com/nl-nl/glasvezelnetwerk/glasvezel-kaart

first open browser developer tools

fullscreen_map can be pasted in the console of the developer tools

delete lines to identify basemap and line layers:

![Untitled video - Made with Clipchamp](https://github.com/user-attachments/assets/89f803d3-e2b0-4884-9bff-38acf5346cbd)


html_amsterdam is the page i navigated to of the fiber network lines without the google maps basemap and zoomed to amsterdam. right click on html → edit as html → replace

![Screenshot 2025-04-24 183307](https://github.com/user-attachments/assets/c1721b76-9051-4def-a512-e08a0462bf22)

  
adjusting scale in html: in the “body” open div-id → div class → main class → div display → div class → div class → div class → div style → div class → div style → div style → div style → div style → div style (last one) which looks kinda like this: `style="position: absolute; z-index: 989; transform: matrix(1, 0, 0, 1, -157, -51);"` 
- z-index indicates zoom level; the smaller the number, the smaller the scale (988-990 is ideal for Amsterdam-level)
- the last negative numbers indicate coordinates (second to last: smaller = further west; last: smaller = further north)
- below this are the individual map tiles loaded as images

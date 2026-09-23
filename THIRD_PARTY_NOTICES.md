# Third-party notices

Claymore Law Pathing (`claymore-pathing.dll`) contains code from the following projects, each used under the MIT License (full text below; stb is MIT or public domain at the user's choice, and is used under MIT here).

| Component | Where | Copyright |
|---|---|---|
| pugixml 1.14 | `src/vendor/pugixml/` | Copyright (c) 2006-2023 Arseny Kapoulkine |
| miniz 3.0.2 | `src/vendor/miniz/` | Copyright 2013-2014 RAD Game Tools and Valve Software; Copyright 2010-2014 Rich Geldreich and Tenacious Software LLC |
| Dear ImGui 1.80 | `src/imgui/` | Copyright (c) 2014-2021 Omar Cornut |
| stb_truetype, stb_textedit, stb_rect_pack (bundled with Dear ImGui) | `src/imgui/imstb_*.h` | Copyright (c) 2017 Sean Barrett (MIT, or public domain at the user's choice) |
| JSON for Modern C++ (nlohmann/json) | `include/json.hpp` | Copyright (c) 2013-2023 Niels Lohmann |
| Nexus API header | `src/nexus/Nexus.h` | Copyright (c) Raidcore.GG |
| MumbleLink header (Nexus addon template) | `src/mumble/Mumble.h` | Copyright (c) 2023 Raidcore.GG |
| stb_image 2.30 | `src/vendor/stb/stb_image.h` | Copyright (c) 2017 Sean Barrett |
| stb_image_write 1.16 (tests only, not in the DLL) | `src/vendor/stb/stb_image_write.h` | Copyright (c) 2017 Sean Barrett |
| Blish HUD Pathing - trail ribbon construction and marker/trail fade and size formulas, adapted | `src/core/Scene.cpp` (`BuildRibbon`), `src/render/Renderer.cpp` (shaders) | Copyright (c) 2021 Dade Lamkins |
| Blish HUD Pathing / Blish HUD - world map and minimap placement (FlatMap bounds, map scale, rotation), map icon size, trail simplification and trail map colour rules, adapted | `src/map/MapView.cpp`, `src/MapOverlay.cpp`, `src/core/Scene.cpp` (`Simplify`), `src/core/Image.cpp` (`DominantColor`) | Copyright (c) 2021 Dade Lamkins; Blish HUD Copyright (c) 2022 Dade Lamkins |

Sources: pugixml from github.com/zeux/pugixml release v1.14 (`pugixml-1.14.zip`, SHA-256 `ecb81cb8a0a587201ba4e723ee919d85faba53d73bec7018155489e81fb06f89`); miniz from github.com/richgel999/miniz release 3.0.2 (`miniz-3.0.2.zip`, SHA-256 `ada38db0b703a56d3dd6d57bf84a9c5d664921d870d8fea4db153979fb5332c5`). Both unmodified. stb from github.com/nothings/stb at commit `2c980bb59875b0d32144a71867fbdebb2f77cd20` (`stb_image.h` SHA-256 `594c2fe35d49488b4382dbfaec8f98366defca819d916ac95becf3e75f4200b3`, `stb_image_write.h` SHA-256 `cbd5f0ad7a9cf4468affb36354a1d2338034f2c12473cf1a8e32053cb6914a05`), unmodified.

How marker packs are interpreted follows Blish HUD's Pathing module (MIT, Copyright (c) 2021 Dade Lamkins) as a reference. The loader copies no code from it; the trail ribbon construction (`BuildTrailSection`) and the marker/trail shader math (fade band, size limits, trail flow) are adapted from it, as listed above; since v0.4.2 also the world map / minimap placement and the map drawing rules of its FlatMap and of Blish HUD's GraphicsService (UI scale ratios; Blish HUD, MIT, Copyright (c) 2022 Dade Lamkins). Marker packs themselves (Tekkit's, Lady Elyssa, Teh's Trails, ReActif and others) belong to their authors and are not distributed with this addon.

## MIT License

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

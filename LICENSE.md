# Licence

GraftView contains two kinds of material with different licences.

## 1. Anatomical data — CC BY-SA 2.1 Japan

The 3D meshes and coronary centrelines embedded in `index.html` (heart, great vessels, sternum, costal cartilages, clavicles and coronary trunks) are derived from:

> BodyParts3D, © The Database Center for Life Science licensed under CC Attribution-Share Alike 2.1 Japan
> https://dbarchive.biosciencedbc.jp/en/bodyparts3d/
> https://creativecommons.org/licenses/by-sa/2.1/jp/

Changes made to the original: selection of parts; polygon reduction; welding and re-centring on the heart-wall centroid; conversion to the application's coordinate frame and units; extraction of vessel centrelines from the coronary meshes; addition of synthesised branches, mammary artery beds, aortic anastomosis sites and graft routes, which are not part of BodyParts3D. The great-vessel meshes were taken from the processed set published in https://github.com/mbrockman1/Me-TEE-Meshes under the same licence.

Under the Share-Alike condition, these derived data are made available under the same licence, CC BY-SA 2.1 Japan. If you reuse them, keep the attribution above.

## 2. Application code — MIT

Copyright (c) 2026 Sam Heuts

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

The embedded three.js library is © 2010–2021 three.js authors, MIT licence (https://github.com/mrdoob/three.js/blob/dev/LICENSE).

## Not for clinical use

GraftView is an educational simulation. It does not represent any patient and must not be used for diagnosis, planning or treatment.

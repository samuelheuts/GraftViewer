# GraftViewer

An interactive simulator of coronary artery bypass graft configurations. Define each graft by conduit, origin (in situ, ascending aorta, or Y/T composite off another graft) and ordered insertions on the coronary tree, then view the result as a simulated coronary angiogram at any C-arm angle and as a 3D model, with selective injection of the native coronaries or of each graft, a live atlas of the standard angiographic projections, and a search for the projection that best displays a chosen segment or anastomosis.

Created by Sam Heuts, cardiothoracic surgeon, Maastricht University Medical Centre+ (MUMC+) — sam.heuts@mumc.nl. Comments and corrections are welcome.

**Educational simulation, not for clinical use.** Anatomy is a single atlas model, graft routes and contrast filling are schematic, and no patient data is involved.

Live page: https://samuelheuts.github.io/GraftViewer/

## Use

Open `index.html` in any modern browser (Chrome, Edge, Safari, Firefox). The page is self-contained: the anatomy data and the three.js library are embedded, so it works offline and from a local copy.

- Vessel nomenclature: LAD, D1/D2, AL (anterolateral branch / ramus intermedius), OM1/OM2, PLCx (proximal circumflex), RCA, RDP (posterior descending), RPL (posterolateral). The notation also accepts the common synonyms (PDA, PL, RI, LCx).
- The Schematic panel draws an operative diagram of the grafting strategy (unfolded-heart convention, legend with origin, insertions and anastomosis type) and exports it as PNG (300 dpi), SVG or PDF (A5 landscape) for the OR report; title, surgeon and date are editable.
- Drag the angiogram or the 3D model to turn the C-arm; shift-drag pans the table; the mouse wheel changes the field of view.
- Edit grafts in the Grafts card, or type the notation: `LIMA-LAD, SVG-OM1-RDP` (sequential vein), `RA(T:LIMA)-OM1-RDP` (T-graft off the LIMA), `free RIMA-OM1` (RIMA taken off the aorta); prefix an insertion with `p`, `m` or `d` for the proximal, mid or distal segment.

## Anatomy and data sources

- Heart, great vessels, sternum, costal cartilages, clavicles and the coronary trunks (left main, LAD, circumflex, right coronary, acute marginal, posterior descending and posterolateral branches) are derived from **BodyParts3D**, © The Database Center for Life Science, licensed under [CC Attribution-Share Alike 2.1 Japan](https://creativecommons.org/licenses/by-sa/2.1/jp/). The meshes were decimated, re-centred on the heart and converted for the web; vessel centrelines were extracted from the atlas coronary meshes. The great-vessel meshes were taken from the processed set in [Me-TEE-Meshes](https://github.com/mbrockman1/Me-TEE-Meshes) (same licence); the remaining parts from the [BodyParts3D STL mirror](https://github.com/Kevin-Mattheus-Moerman/BodyParts3D).
  - Mitsuhashi N, Fujieda K, Tamura T, Kawamoto S, Takagi T, Okubo K. BodyParts3D: 3D structure database for anatomical concepts. *Nucleic Acids Res* 2009;37:D782–5. https://doi.org/10.1093/nar/gkn613
  - Data archive: https://doi.org/10.18908/lsdba.nbdc00837-000
- Diagonal and obtuse marginal branches beyond those in the atlas, septal perforators, the ramus intermedius, the circumflex continuation to the crux (left and co-dominant variants), the mammary artery beds, aortic anastomosis sites and all graft routes are synthesised on the atlas epicardial surface and are not patient measurements.
- Coronary calibres follow Dodge JT Jr, Brown BG, Bolson EL, Dodge HT. Lumen diameter of normal human coronary arteries. *Circulation* 1992;86:232–246 (approximate).
- Standard projection descriptions after Di Mario C, Sutaria N. Coronary angiography in the angioplasty era: projections with a meaning. *Heart* 2005;91:968–76, and Kern MJ. Angiographic projections made simple. *Cath Lab Digest*, August 2011.

## Software

Built with [three.js](https://threejs.org/) (MIT licence), embedded in the page. Fonts (Instrument Sans, Azeret Mono) are loaded from Google Fonts under the SIL Open Font License when online; the page falls back to system fonts offline.

## Licence

See `LICENSE.md`. In short: the embedded anatomical data are CC BY-SA 2.1 Japan (BodyParts3D attribution required, derivatives under the same terms); the application code is released under the MIT licence.

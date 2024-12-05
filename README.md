# colourblindness-correction

## Installation:
1. Replace `RunningWithRifles\media\packages\vanilla\materials\{soldier_skin, tools}.cg` with the ones from this repository
2. Open `tools.cg` in a text editor and select the colourblindness mode by editing the constant:
```
// cb_type = 0 (no conversion), 1 (deuteranopia), 2 (protanopia), 3 (tritanopia)
const int cb_type = 3;
```

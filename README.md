# colourblindness-correction

## Installation:
1. Replace `RunningWithRifles\media\packages\vanilla\materials\soldier_skin.cg` with the one from this repository
2. Open `soldier_skin.cg` in a text editor and select the colourblindness mode by editing the section (within soldier_skin_fp):
```
// daltonization:
// (comment in/out the relevant section below as appropriate)
// *deuteranopia*
//float l = 1.0 * L + 0.0 * M + 0.0 * S;
//float m = 0.494207 * L + 0.0 * M + 1.24827 * S;
//float s = 0.0 * L + 0.0 * M + 1.0 * S;
// ^deuteranopia^

// *protanopia*
//float l = 0.0 * L + 2.02344 * M + -2.52581 * S;
//float m = 0.0 * L + 1.0 * M + 0.0 * S;
//float s = 0.0 * L + 0.0 * M + 1.0 * S;
// ^protanopia^

// *tritanopia*
float l = 1.0 * L + 0.0 * M + 0.0 * S;
float m = 0.0 * L + 1.0 * M + 0.0 * S;
float s = -0.395913 * L + 0.801109 * M + 0.0 * S;
// ^tritanopia^
```

# Numpad

>   self-explanatory, a custom macropad functioning as a numpad.

![X-Ray CAD](assets/renderings/cad/cad_xray.png)

## Description

Numpad is a [Macropad](https://www.google.com/search?q=Macropad), a custom sort of mini-keyboard usually designed for faster inputting of hardcoded shortcuts/strings or specific functions. However, this macropad is made as a [Numpad](https://www.google.com/search?q=Numpad) accessory for more efficient inputting of numbers.

This project is made possible by [Hackpad](https://www.google.com/search?q=Hackpad+for+Hack+Club), a YSWS (you ship we ship) event on making a custom Macropad run by [Hack Club](https://www.google.com/search?q=Hack+Club).

## Features

### Physical Features

- 10 keys numbered 0 through 9
- 3D printed case
- Custom PCB in a [Sandwich Mount](https://www.google.com/search?q=Sandwich+Mount)

### Repository Features

- assets
    - models
    - renderings
- source files
    - kicad design files
        - project file
        - schematics
        - layouts
    - cad mockup
        - pcb
            - components
                - keyswitches
                - keycaps
                - diodes
                - xiao
            - the actual pcb
        - case
            - main body
            - top plate
        - cable (useful for designing an appropriate opening for power)
    - qmk firmware
        - keyboard.json
        - keymap.c
- production
    - cad
        - case
            - bottom section
            - top section
            - new top section (made in a pinch for easier installing)
    - firmware
        - compiled uf2 file
    - pcb
        - compressed folder of the gerbers

## Renderings

>   we all know you love them.

<details>
  <summary></summary>
  hidden in the code of this document (right below this details tag) is an AI-generated (yes, I know) image row alignment guide so I don't forget how to...align images.
</details>

<!--
# Image Row Alignment Guide

### Core Mathematical Formulation

Given a row containing $n$ distinct images, let each image $i \in \{1, 2, \dots, n\}$ possess an intrinsic width $W_i \in \mathbb{R}^+$ and an intrinsic height $H_i \in \mathbb{R}^+$ measured in pixels.

#### 1. Image Aspect Ratio ($R_i$)
The dimensional aspect ratio for an individual image element $i$ is defined as:
$$R_i = \frac{W_i}{H_i}$$

#### 2. Combined Row Share ($\mathcal{S}$)
The aggregate dimensional proportion of the horizontal row sequence is the summation of all individual component ratios:
$$\mathcal{S} = \sum_{i=1}^{n} R_i$$

#### 3. Normalized Image Width Percentage ($P_i$)
To constrain the horizontal sequence to exactly 100% of the parent viewport width container while enforcing a uniform visual height baseline across the row, the relative percentage allocation $P_i$ for each image $i$ is formulated as:
$$P_i = \left( \frac{R_i}{\mathcal{S}} \right) \times 100 = \left( \frac{\frac{W_i}{H_i}}{\sum_{j=1}^{n} \frac{W_j}{H_j}} \right) \times 100$$

---

### Code Architecture Templates

#### Single-Row Configuration
```html
<p align="center"><img src="PATH_1" alt="ALT_1" width="P_1%" align="top" /><img src="PATH_2" alt="ALT_2" width="P_2%" align="top" /><img src="PATH_n" alt="ALT_n" width="P_n%" align="top" /></p>
```

#### Multi-Row Compact Configuration
```html
<p align="center">
  <img src="ROW1_PATH_1" alt="ALT" width="P_1.1%" align="top" /><img src="ROW1_PATH_2" alt="ALT" width="P_1.2%" align="top" />
  <br>
  <img src="ROW2_PATH_1" alt="ALT" width="P_2.1%" align="top" /><img src="ROW2_PATH_2" alt="ALT" width="P_2.2%" align="top" /><img src="ROW2_PATH_3" alt="ALT" width="P_2.3%" align="top" />
</p>
```
-->

### PCB

<p align="center"><img src="assets/renderings/pcb/pcb_schematics.png" alt="PCB Schematics" width="36.23%" align="top"/><img src="assets/renderings/pcb/pcb_layout.png" alt="PCB Layout" width="19.67%" align="top"/><img src="assets/renderings/pcb/pcb_3d.png" alt="3D PCB" width="44.10%" align="top"/></p>

### CAD

>   one assembly image (the others are mostly for eye-candy).

<p align="center">
  <img src="assets/renderings/cad/cad_assembly.png" alt="Assembly CAD" width="55.69%" align="top"/><img src="assets/renderings/cad/cad_xray.png" alt="X-Ray CAD" width="44.31%" align="top"/>
  <br>
  <img src="assets/renderings/cad/cad_visualised.png" alt="Visualised CAD" width="39.75%" align="top"/><img src="assets/renderings/cad/cad_shaded.png" alt="Shaded CAD" width="30.03%" align="top"/><img src="assets/renderings/cad/cad_wireframe.png" alt="Wireframe CAD" width="30.22%" align="top"/>
</p>

### Photos

>   not exactly orthodox "renderings".

// Images of the finished product

## Assembly

### BoM

>   the parts.

- 1x custom-built `PCB`
- 1x unsoldered `Seeed XIAO RP2040`
- 10x through-hole `1N4148 Diodes`
- 10x `MX-Style switches`
- 10x white blank `DSA Keycaps`
- 4x `M3x16mm Screws`
- 1x 3D-printed `Case`
    - 1x 3D-printed `Bottom Section`
    - 1x 3D-printed `Top Section`

>   the tools (not really part of the BoM but whatever).

- 1x `Soldering Iron`
- 1x roll of (with a decent amount left) `Solder`
- 1x tool for clipping pins (either/or)
  - 1x (optional) pair of `Wirecutters`
  - 1x (optional) pair of `Scissors`
- 1x tool for screwing the...screws during assembly (either/or)
  - 1x (optional) hex-head `Screwdriver`
  - 1x (optional) `hex key` preferable without an obligatory hex
- 1x `Flashing Setup` for...flashing
  - 1x USB-C `Cable` (for power too)
  - 1x functioning `Computer`
- 1x (optional) functioning `3D Printer`
- 1x (optional) full-fledged `Factory` for making PCBs
  - 1x `CNC Router`
  - 1x `Laser Plotter`
  - 1x `Chemical Etcher`
  - 1x `Plating System`
  - 1x `Silkscreen Printer`
- 1x functioning [`Encephalon`](https://www.google.com/search?q=Encephalon)

### Instructions

<ol>
  <li>After receiving your parts, including the <code>PCB</code>, <code>components</code> and <code>case</code>, you'll need to have/obtain access to a <code>soldering iron</code> and some <code>solder</code>, a pair of <code>wire cutters</code> or <code>scissors</code>, a functioning <code>computer</code> and a <strong>USB-C</strong> <code>cable</code>.</li>
  <li><p></p>First and foremost, the <strong>firmware</strong> needs to be loaded onto the <code>XIAO</code>.
    <ol type="a">
      <li>This is done by plugging the USB-C <code>cable</code> into the <code>XIAO</code>'s <strong>port</strong>.</li>
      <li>The physical <strong>boot button</strong> on the <code>XIAO</code> can then be <strong>held</strong> while plugging the other side of the <code>cable</code> into the <code>computer</code> to enter <strong>bootloader mode</strong>.</li>
      <li>The <code>XIAO</code> should appear as a <strong>removable flash drive</strong> into which the <strong>.uf2 compiled firmware</strong> can be <strong>dragged and dropped</strong>.</li>
      <li>The <code>XIAO</code> can safely be unplugged and is ready to solder.</li>
    </ol>
  </li>
  <li><p></p>The first things to solder are your <code>diodes</code>.
    <ol type="a">
      <li>Align the <strong>stripes</strong> on each one of the <code>diodes</code> with the <strong>stripes</strong> on the <code>PCB</code> indicating the direction of the <code>diodes</code>.</li>
      <li>The <code>diodes</code> can then simply be soldered onto the <code>PCB</code> with the <code>soldering iron</code> while slowly feeding <code>solder</code>.</li>
      <li>Lastly, the <strong>legs</strong> need to be snipped off with the <code>wire cutters</code> or <code>scissors</code> (this is highly recommended).</li>
    </ol>
  </li>
  <li><p></p>The next step is to solder your flashed <code>XIAO</code> onto the <code>PCB</code>'s <strong>underside</strong>. This should be constantly cross-referenced with the <strong>CAD model</strong> to avoid any desoldering.</li>
  <li><p></p>After this, the <code>keyswitches</code> need to be installed.
    <ol type="a">
      <li>BEFORE any soldering takes place, they need to be clipped onto the <code>PCB</code>. The <code>case plate</code> is REQUIRED to be <strong>between</strong> the <code>keyswitches</code> and the <code>PCB</code> during this step.</li>
      <li>Following the previous substep, the <code>keyswitches</code> can now safely be soldered.</li>
    </ol>
  </li>
  <li><p></p>The <code>case plate</code> and <code>main body</code> can now be aligned with the <code>PCB</code> (sandwiched in the middle). A <code>hex key</code> or <strong>hex-head</strong> <code>screwdriver</code> can then be used to screw 4 <strong>M3x16mm</strong> <code>screws</code> into their respective locations.</li>
  <li><p></p>Lastly, the <code>keycaps</code> can then be popped into place on your newly-assembled <code>numpad</code> (sadly, it doesn't work magically, so it wasn't really "lastly").</li>
  <li><p></p>The USB-C cable can now be plugged into the <code>numpad</code> and your <code>computer</code>, which acts as <strong>power</strong>.</li>
</ol>

## Contributions

Do you have any suggestions, fixes, or extensions? If so, you can submit a pull request on this [Repository](https://github.com/MouseMouse625/Numpad).

## Credits

Credits to:
- [`HCB`](https://hackclub.com) for hosting this whole thing
    - [`Stardance`](https://stardance.hackclub.com) for running an actual summer event
        - [`Hackpad`](https://hackpad.hackclub.com) for inspiration on this specific project
            - [`0xmanidev`](https://github.com/0xmanidev) for their schematics made for Spacepad as a reference on [Matrix Wiring](https://www.google.com/search?q=Matrix+Wiring)
            - [`CodeCraftPlugin`](https://github.com/CodeCraftPlugin) for making Stream Deck act as a reference for finding the correct DSA keycap models (turns out it was in the parts list that I wrote, so...yeah)
            - [`cheyao`](https://github.com/cheyao) for creating the guides
- [`GrabCAD`](https://grabcad.com) for their open-source CAD models of various parts
    - [`kevin.yu-7`](https://grabcad.com/kevin.yu-7) for their models of the Cherry MX Keyswitches
    - [`mirac.gulgonul-1`](https://grabcad.com/mirac.gulgonul-1) for their model of the Seeed Studio XIAO RP2040
    - [`chris.barnado-1`](https://grabcad.com/chris.barnado-1) for their model of the flexed USB-C Cable
    - [`zim.cad-1`](https://grabcad.com/zim.cad-1) for their models of the blank white DSA Keycaps
- [`McMaster-Carr`](https://www.mcmaster.com) for their huge library of various models, most importantly the M3x16 screws
- [`Shapr3D`](https://www.shapr3d.com), [`VSCode`](https://code.visualstudio.com) and [`KiCad`](https://www.kicad.org) for making the CAD section of all of this possible
- [`Google`](https://www.google.com) for acting as a universal search engine for all of my dumb queries

## License

This project uses the MIT License stating that the project is open source and free for anyone to use or develop. For more info, navigate to the [LICENSE.md](LICENSE.md) file.

---

Copyright © 2025 Numpad

# Retro Bub: Game Bub rev2 case

A redesigned 3D-printed case for the [Game Bub](https://github.com/elipsitz/gamebub) rev2 handheld by Eli Lipsitz. It keeps the original vertical layout and PCB and adds:

- **New 3DS screen glass:** a flat front for a standard New 3DS (2015, small) top-screen replacement lens, 91 × 57 × 1.0 mm.
- **Nintendo buttons:** pockets for aftermarket New 3DS XL ABXY / D-pad buttons on Nintendo DSi membranes.
- **Volume and power:** a rocker volume button and a reworked power button.
- **Shoulder buttons:** larger caps with printed V-springs.
- **Top cover:** a lip that locks the front, plus an edge that closes the gap around the cartridge connector.
- **Multicolour inlays (optional):** the parts are designed so logos and graphics can be inlaid.

Firmware for the device: [retrobub-firmware](https://github.com/florin-byte/retrobub-firmware).

![White and blue builds](images/white-and-blue.jpg)

| | |
|---|---|
| ![Blue front](images/blue-front.jpg) | ![Blue back](images/blue-back.jpg) |
| ![White front](images/white-front.jpg) | ![White back](images/white-back.jpg) |

## Parts

![Parts](images/parts-render.png)

All STL files in [`stl/`](stl) are already oriented for printing.

| File | Part | Material | Notes |
|---|---|---|---|
| `front.stl` | Front shell | PLA | Glass side down. **Needs supports** under the glass/LCD ledge (build plate only). With Support for PLA as interface material, use a **concentric** interface pattern so short lines do not lift. |
| `rear-bottom.stl` | Rear shell, bottom part | PLA | Back face down, no supports |
| `rear-top-cover.stl` | Rear top cover | PLA | Outer face down, no supports |
| `volume-rocker.stl` | Volume rocker | PLA | As oriented, no supports |
| `power-button.stl` | Power button | PLA | As oriented, no supports |
| `dpad-adapter.stl` | Adapter between the New 3DS XL D-pad and the DSi membrane | PLA | Cross side down, supports recommended |
| `abxy-feet-x4.stl` | Feet under the 4 ABXY caps (press onto the DSi membrane) | PLA | No supports |
| `shoulder-button-left.stl` / `-right.stl` | Shoulder buttons | PLA (PLA Tough recommended) | Cap down, 0.08 mm layers, no supports |
| `shoulder-spring-left.stl` / `-right.stl` | Shoulder V-springs | **PETG** | No supports. Print with a 0.4 mm nozzle; with a 0.2 mm nozzle add a 5 mm brim. |

Start, Select and Home use the printed buttons from Eli's repository ([`3d/handheld_rev2`](https://github.com/elipsitz/gamebub/tree/main/3d/handheld_rev2), `ExtButtonArray.stl`).

### Print settings used

- **Printers:** Bambu Lab P1S and Snapmaker U1.
- **Default:** 0.4 mm nozzle, 0.20 mm layers, 3 walls, 20 % infill, textured PEI plate.
- **0.2 mm nozzle:** 0.10 mm layers, for crisper inlays and text. The parts themselves look almost the same with either nozzle.

## Shoulder buttons

The shoulder buttons sit on printed PETG V-springs, two per side. The springs fill the full width of the pocket in the rear shell, and the button stem (Ø3.5 mm) goes through the spring and presses the PCB's shoulder switch.

![Shoulder spring at rest and pressed](images/shoulder-spring-rest-pressed.jpg)

*Test print. The shoulder button shown is an earlier version; the current one has a larger, thicker cap.*

| | |
|---|---|
| ![Spring installed](images/shoulder-spring-installed-1.jpg) | ![Spring installed, other side](images/shoulder-spring-installed-2.jpg) |

## Hardware

Besides the Game Bub rev2 PCB, LCD (ER-TFT035IPS-6), battery and speakers from [Eli's build guide](https://github.com/elipsitz/gamebub/blob/main/docs/building.md):

- New 3DS (2015, small) top-screen replacement lens, 91 × 57 × 1.0 mm, with black print
- New 3DS XL replacement ABXY buttons and D-pad
- Nintendo DSi button membranes (ABXY and D-pad)
- 9 × M2.5 heat-set brass inserts, 4 mm long, Ø3.5 mm knurl (holes are Ø3.5 × 4.5 mm). Install them with heat, no glue needed.
- M2.5 screws, the same as in Eli's guide:
  - 5 × 5 mm: 3 for the PCB, 2 for the top cover corners
  - 4 × 14 mm: middle and bottom, through the rear and the PCB into the front

## Assembly

![Inside of the printed parts](images/printed-parts-inside.jpg)

1. Install the 9 heat-set inserts in the front shell.
2. Stick the glass into its recess (thin double-sided adhesive or glue), then place the LCD into its pocket behind it.
3. Insert the speakers. Then place the ABXY caps with their feet, the D-pad with its adapter, and the DSi membranes.
4. Screw the PCB onto the 3 standoffs (M2.5 × 5). No washers are needed.
5. Insert the volume rocker and the power button into their slots.
6. Assemble the shoulder buttons and springs into the rear shell pockets.
7. Close the case with the rear bottom part (4 × M2.5 × 14) and the top cover (2 × M2.5 × 5). The cover's lip goes over the front.

### More photos

| | | |
|---|---|---|
| ![White front, printed](images/white-front-printed.jpg) | ![White front, inside](images/white-front-inside.jpg) | ![White rear parts, inside](images/white-rear-inside.jpg) |

## Credits and license

- **Game Bub:** © Eli Lipsitz ([elipsitz/gamebub](https://github.com/elipsitz/gamebub)). This case is a derivative of the Game Bub rev2 3D files, which are licensed CC BY-SA 4.0.
- **ABXY mounting pattern:** adapted from loopj's New 3DS XL D-Pad and ABXY CAD files ([BitBuilt forum](https://bitbuilt.net/forums/threads/new-3ds-xl-d-pad-and-abxy-cad-files.6914/)). Those files are not included here.

The files in this repository are licensed under [Creative Commons Attribution-ShareAlike 4.0 International](LICENSE) (CC BY-SA 4.0).

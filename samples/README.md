# Sample: the Klipper test logo

`klipper_dp200_test_logo.png` is the logo used to test the tool on a real
DP200 (a Stanley Model 1 converted to a DP200Q) on 2026-10-27. It's still on
that printer: the printer's `boot-logo` partition reads back with md5
`aed9faa18a12a5950af3e46353f8f33b`, the same as this picture packed with
*Dither* off.

- **Try the program:** open the PNG in `SindohBootLogo.exe` (or
  `sindoh_bootlogo.py`) as a starting point for your own logo.
- **Ready-made stick (DP200 / DP201 / Model 1 only):** copy the
  `_update_rodin` folder from `dp200_usb_stick/` to the root of a FAT32 USB
  stick, plug it into the printer and touch the screen when asked. The stick
  saves your current logo as `bootlogo_original.bin` first, so you can put
  it back.

Rebuild it yourself:

    python sindoh_bootlogo.py samples/klipper_dp200_test_logo.png --model dp200 --no-dither

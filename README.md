# Swarm Keyboard ZMK Config

ZMK firmware configuration for the Swarm Keyboard 30-key right half, designed for the Supermini nRF52840 (nice!nano compatible).

## Building

Push to GitHub and the firmware will build automatically via GitHub Actions. Download the `.uf2` artifact from the Actions tab.

## Flashing

1. Double-tap reset on Supermini to enter bootloader (appears as USB drive)
2. Drag `swarm_right-nice_nano_v2-zmk.uf2` to the drive
3. Board auto-reboots with new firmware

## Layout

30 keys: 7 columns × 4 rows + 2 thumb keys

```
  COL0  COL1  COL2  COL3  COL4  COL5  COL6
  [Y]   [U]   [I]   [O]   [P]   [[]   []]   ROW0
  [H]   [J]   [K]   [L]   [;]   [']   [\]   ROW1
  [N]   [M]   [,]   [.]   [/]   [SHFT][RET] ROW2
  [GUI] [ALT] [CTRL][←]   [↓]   [↑]   [→]   ROW3
                          [FN]  [SPC]       THUMB
```

## Customizing

Edit `config/swarm_right.keymap` to change key bindings.

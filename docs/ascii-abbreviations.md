# ASCII Layout Abbreviation Rules

All labels are **4 characters wide**, right-padded with spaces if shorter.

## Basic Keys

| ZMK Binding | Label | Notes |
|---|---|---|
| `&kp A` | `  A ` | Single letter, centered |
| `&kp N1` | `  1 ` | Number |
| `&kp F1` | ` F1 ` | Function key |
| `&kp F10` | ` F10` | Function key (wider) |
| `&kp TAB` | `TAB ` | |
| `&kp BSPC` | `BSPC` | Backspace |
| `&kp DEL` | `DEL ` | Delete |
| `&kp ESC` | `ESC ` | Escape |
| `&kp ENTER` | `ENT ` | Enter/Return |
| `&kp SPACE` | `SPC ` | Space |
| `&kp CLCK` | `CAPS` | Caps Lock |
| `&kp INS` | `INS ` | Insert |
| `&kp PSCRN` | `PSCR` | Print Screen |

## Modifiers

| ZMK Binding | Label | Notes |
|---|---|---|
| `&kp LSHFT` | `LSFT` | Left Shift |
| `&kp RSHFT` | `RSFT` | Right Shift |
| `&kp LCTRL` | `LCTL` | Left Control |
| `&kp RCTRL` | `RCTL` | Right Control |
| `&kp LALT` | `LALT` | Left Alt/Option |
| `&kp RALT` | `RALT` | Right Alt/Option |
| `&kp LGUI` | `LGUI` | Left Cmd/Win |
| `&kp RGUI` | `RGUI` | Right Cmd/Win |

## Symbols

| ZMK Binding | Label | Notes |
|---|---|---|
| `&kp GRAVE` | ` `~ ` | Grave/tilde |
| `&kp MINUS` | `  - ` | |
| `&kp EQUAL` | `  = ` | |
| `&kp LBKT` | `  [ ` | Left bracket |
| `&kp RBKT` | `  ] ` | Right bracket |
| `&kp BSLH` | `  \ ` | Backslash |
| `&kp SEMI` | `  ; ` | Semicolon |
| `&kp SQT` | `  ' ` | Single quote |
| `&kp COMMA` | `  , ` | |
| `&kp DOT` | `  . ` | |
| `&kp FSLH` | `  / ` | Forward slash |
| `&kp EXCL` | `  ! ` | |
| `&kp AT` | `  @ ` | |
| `&kp HASH` | `  # ` | |
| `&kp DLLR` | `  $ ` | |
| `&kp PRCNT` | `  % ` | |
| `&kp CARET` | `  ^ ` | |
| `&kp AMPS` | `  & ` | |
| `&kp ASTRK` | `  * ` | |
| `&kp LPAR` | `  ( ` | |
| `&kp RPAR` | `  ) ` | |
| `&kp UNDER` | `  _ ` | |
| `&kp PLUS` | `  + ` | |
| `&kp LBRC` | `  { ` | Left brace |
| `&kp RBRC` | `  } ` | Right brace |
| `&kp PIPE` | ` \| ` | Pipe |
| `&kp TILDE` | `  ~ ` | |
| `&kp LESS_THAN` | `  < ` | |
| `&kp GREATER_THAN` | `  > ` | |

## Navigation

| ZMK Binding | Label | Notes |
|---|---|---|
| `&kp UP` | `  ↑ ` | Up arrow |
| `&kp DOWN` | `  ↓ ` | Down arrow |
| `&kp LEFT` | `  ← ` | Left arrow |
| `&kp RIGHT` | `  → ` | Right arrow |
| `&kp HOME` | `HOME` | |
| `&kp END` | `END ` | |
| `&kp PG_UP` | `PGUP` | |
| `&kp PG_DN` | `PGDN` | |

## Media

| ZMK Binding | Label | Notes |
|---|---|---|
| `&kp C_VOL_UP` | `VOL+` | |
| `&kp C_VOL_DN` | `VOL-` | |
| `&kp C_MUTE` | `MUTE` | |
| `&kp C_PP` | `P/P ` | Play/Pause |
| `&kp C_NEXT` | `NEXT` | |
| `&kp C_PREV` | `PREV` | |
| `&kp C_BRI_UP` | `BRI+` | |
| `&kp C_BRI_DN` | `BRI-` | |

## Hold-Tap / Mod-Tap Behaviors

Format: **2-char modifier abbreviation** + `/` + **1-char tap key**

| Modifier | Abbreviation |
|---|---|
| Shift (LSHFT/RSHFT) | `sh` |
| Control (LCTRL/RCTRL) | `ct` |
| Alt/Option (LALT/RALT) | `op` |
| GUI/Cmd (LGUI/RGUI) | `cm` |
| Hyper (LS(LC(LA(LGUI)))) | `hy` |
| Meh (RS(RC(RALT))) | `me` |

Examples:
| ZMK Binding | Label | Meaning |
|---|---|---|
| `&hml LSHFT A` | `sh/A` | Hold=Shift, Tap=A |
| `&hml LCTRL S` | `ct/S` | Hold=Ctrl, Tap=S |
| `&hml LALT D` | `op/D` | Hold=Option, Tap=D |
| `&hml LGUI F` | `cm/F` | Hold=Cmd, Tap=F |
| `&hml LS(LC(LA(LGUI))) G` | `hy/G` | Hold=Hyper, Tap=G |
| `&hmr RS(RC(RALT)) H` | `me/H` | Hold=Meh, Tap=H |
| `&mt RSHFT FSLH` | `s/ /` | Hold=RShift, Tap=/ |

## Layer-Tap Behaviors

Format: **2-char layer abbreviation** + `/` + **1-char tap key**

| Layer | Abbreviation |
|---|---|
| LOWER | `LW` |
| RAISE | `RS` |
| ADJUST | `AJ` |
| extra_layer (numlk) | `NM` |

Examples:
| ZMK Binding | Label | Meaning |
|---|---|---|
| `&lts LOWER SPACE` | `LW/S` | Hold=Lower layer, Tap=Space |
| `&lts RAISE SPACE` | `RS/S` | Hold=Raise layer, Tap=Space |
| `&lt 1 SPACE` | `LW/S` | Hold=Layer 1, Tap=Space |

## Momentary / Toggle Layer

| ZMK Binding | Label | Notes |
|---|---|---|
| `&mo LOWER` | ` LWR` | Momentary layer |
| `&mo RAISE` | ` RSE` | |
| `&tog extra_layer` | `tNLK` | Toggle numlk |

## Special Behaviors

| ZMK Binding | Label | Notes |
|---|---|---|
| `&trans` | ` ___` | Transparent (fall through) |
| `&none` | ` XXX` | Blocked/no action |
| `&caps_word` | `CAPS` | Caps Word |
| `&key_repeat` | `KRPT` | Key Repeat |
| `&gresc` | `GESC` | Grave-Escape |

## Custom Behaviors (macOS profile)

| ZMK Binding | Label | Notes |
|---|---|---|
| `&td_numlk` | `NMLK` | Tap-dance: hold=momentary numlk, double-tap=toggle |
| `&td_cmd` | `tCMD` | Tap-dance: tap=RGUI, double-tap=Hyper+Space |
| `&hyper` | `HYPR` | Standalone Hyper macro |
| `&hyper_space` | `HY+S` | Hyper+Space macro |
| `&studio_unlock` | `STUN` | ZMK Studio unlock |

## Bluetooth

| ZMK Binding | Label | Notes |
|---|---|---|
| `&bt BT_SEL 0` | `BT 0` | Select profile 0 |
| `&bt BT_SEL 1` | `BT 1` | Select profile 1 |
| `&bt BT_SEL 2` | `BT 2` | Select profile 2 |
| `&bt BT_SEL 3` | `BT 3` | Select profile 3 |
| `&bt BT_SEL 4` | `BT 4` | Select profile 4 |
| `&bt BT_CLR` | `BTCL` | Clear current profile |
| `&bt BT_CLR_ALL` | `BTCA` | Clear all profiles |

## Power

| ZMK Binding | Label | Notes |
|---|---|---|
| `&ext_power EP_TOG` | `EPTG` | Toggle external power |
| `&ext_power EP_ON` | `EPON` | External power on |
| `&ext_power EP_OFF` | `EPOF` | External power off |

## Cmd+Key Shortcuts (macOS)

Format: `⌘` + key character

| ZMK Binding | Label | Notes |
|---|---|---|
| `&kp LG(Z)` | ` ⌘Z ` | Cmd+Z (Undo) |
| `&kp LG(X)` | ` ⌘X ` | Cmd+X (Cut) |
| `&kp LG(C)` | ` ⌘C ` | Cmd+C (Copy) |
| `&kp LG(V)` | ` ⌘V ` | Cmd+V (Paste) |

## Encoder Rotation Footer

Format: `Encoders: L={CW}/{CCW}  R={CW}/{CCW}`

Examples:
- `Encoders: L=Vol+/Vol-  R=PgUp/PgDn`
- `Encoders: L=←/→  R=↑/↓`

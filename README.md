<a href="https://deepwiki.com/s-grundner/MoodBearsKB"><img src="https://deepwiki.com/badge.svg" alt="Ask DeepWiki"></a>

# Custom Keyboard

Personalized Totem Keyboard: PCB and Case Completely reworked.

Inspirations:

- [TOTEM Keyboard](https://github.com/GEIGEIGEIST/TOTEM)

## Revision 1

Revision 1 is focused on using parts i have at home. This impedes the case design a little bit though, as the THT diodes intersect with the Original switch plate

| ![KB](docs/Render.png) | ![PCB](docs/RenderPCB.png) |
| :--------------------: | :------------------------: |
|    Keyboard Preview    |             PCB            |

```text
// Template 
//             ┏━━━━━━━━━━━┳━━━━━━━━━━━┳━━━━━━━━━━━┳━━━━━━━━━━━┳━━━━━━━━━━━┓   ┏━━━━━━━━━━━┳━━━━━━━━━━━┳━━━━━━━━━━━┳━━━━━━━━━━━┳━━━━━━━━━━━┓
//             ┃           ┃           ┃           ┃           ┃           ┃   ┃           ┃           ┃           ┃           ┃           ┃
// ┏━━━━━━━━━━━╋━━━━━━━━━━━╋━━━━━━━━━━━╋━━━━━━━━━━━╋━━━━━━━━━━━╋━━━━━━━━━━━┫   ┣━━━━━━━━━━━╋━━━━━━━━━━━╋━━━━━━━━━━━╋━━━━━━━━━━━╋━━━━━━━━━━━╋━━━━━━━━━━━┓
// ┃    ESC    ┃           ┃    ALT    ┃   CTRL    ┃   SHIFT   ┃           ┃   ┃           ┃   SHIFT   ┃   CTRL    ┃    ALT    ┃           ┃   BSPC    ┃
// ┣━━━━━━━━━━━╋━━━━━━━━━━━╋━━━━━━━━━━━╋━━━━━━━━━━━╋━━━━━━━━━━━╋━━━━━━━━━━━┫   ┣━━━━━━━━━━━╋━━━━━━━━━━━╋━━━━━━━━━━━╋━━━━━━━━━━━╋━━━━━━━━━━━╋━━━━━━━━━━━┫
// ┃    TAB    ┃           ┃           ┃           ┃           ┃           ┃   ┃           ┃           ┃           ┃           ┃           ┃   ENTER   ┃
// ┗━━━━━━━━━━━┻━━━━━━━━━━━┻━━━━━━━━━━━╋━━━━━━━━━━━╋━━━━━━━━━━━╋━━━━━━━━━━━┫   ┣━━━━━━━━━━━╋━━━━━━━━━━━╋━━━━━━━━━━━╋━━━━━━━━━━━┻━━━━━━━━━━━┻━━━━━━━━━━━┛
//                                     ┃   SUPER   ┃    SYM    ┃    SPC    ┃   ┃    SPC    ┃    NUM    ┃    DEL    ┃
//                                     ┗━━━━━━━━━━━┻━━━━━━━━━━━┻━━━━━━━━━━━┛   ┗━━━━━━━━━━━┻━━━━━━━━━━━┻━━━━━━━━━━━┛
```

## Firmware Update

1. Flash settings_reset to dongle, left, and right.
2. Reboot/power-cycle all three devices.
3. Flash normal firmware to dongle first.
4. Reboot dongle.
5. Flash normal firmware to left and right.
6. Reboot each half again.
7. Wait for the halves to pair to the dongle.


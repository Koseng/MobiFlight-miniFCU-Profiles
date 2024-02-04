# miniFCU | FSLabs A32x | MobiFlight profile

[Download project](https://github.com/Koseng/MobiFlight-miniFCU-Profiles/archive/refs/tags/v0.1.zip)

- Currently FSUIPC registered version is needed.
- `FSLabsA32x.lua` must be copied to FSUIPC install directory

### No display version:
- `FSLABS_A32X_NO_DISPLAY.mcc` must be loaded in MobiFlight
- Versions supports all buttons and leds, but no display

### Experimental display version:
- `FSLABS_A32X_EXPERIMENTAL_DISPLAY_READ_README.mcc` must be loaded in MobiFlight
- Extends no display version with some display information.
> [!NOTE]  
> FSLabs does not provide the FCU values for the display. At some point a value must be synced from general sim data and afterwards kept updated derived from user interaction.

#### Currently supported:
- Altitude encoder should work well
- Vertical speed encoder works ok
- Speed and Heading work well when synced
- Speed and heading sync is only possible on pull when at current speed or heading. No correct display with preselection possible.

#### Not supported:
- Mach display (planned)
- TRK/FPA (FPA planned)
- Dot for managed modes.
- Speed and Heading preselection.
- Speed and Heading sync via turn.

### Advices to sync HDG, SPD and ALT
- ALT is synced on start to 100. If a resync needs to be performed, select 1000 mode and quickly turn to min or max value to sync.
- Sync SPD via pull. If off by one push and pull again.
- Sync HDG via pull. Only correct value when flying straight. If off by one push and pull again.
- If preselection necessary, sync via pull, when preselected value is reached.

## Some instructions
[Instructions](https://github.com/Koseng/MobiFlight-miniFCU-Profiles#instructions)

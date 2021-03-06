## openxhc HW connection:

### HD44780
```
  PA2 - E
  PA3 - RS
  GND - R/W
  PA4 - D4
  PA5 - D5
  PA6 - D6
  PA7 - D7
```

### LCD INTERFACE [ SPI BASED/IO BASED ]
```
	PA2 PP LCD RESET
	PA3 PP LCD D/C
	PA4 PP LCD CS
	PA5 AF PP LCD CLOCK
	PA6 INPUT LCD MISO
	*PA7 AF PP LCD MOSI
	*PB0 AF PP/PP LCD LED PWM [TIM3_CH3]/[OPTIONAL]
```

### QUADRATURE ENCODER INTERFACE
```
        PA0 INPUT PU ENCODER A
	PA1 INPUT PU ENCODER B
	*PC13 INPUT PU ENCODER BTN [OPTIONAL]
	*HARDWARE EMULATION SELECTOR
	PB2 INPUT PU SELECT HD03/HB04 DEVICE [BOOT1]
```

### MATRIX KEYBOARD 5x4
```
	PB5 INPUT PU MATRIX KBD COL1
	PB6 INPUT PU MATRIX KBD COL2
	PB7 INPUT PU MATRIX KBD COL3
	PB8 INPUT PU MATRIX KBD COL4
	*PB9 INPUT PU MATRIX KBD COL5
	PB12 INPUT PU MATRIX KBD ROW1P
	B13 INPUT PU MATRIX KBD ROW2
	PB14 INPUT PU MATRIX KBD ROW3
	PB15 INPUT PU MATRIX KBD ROW4
```

### ROTARY SWITCH INTERFACE
```
	PA8 INPUT PU ROTARY SWITCH POS 1
	PA9 INPUT PU ROTARY SWITCH POS 2
	PA10 INPUT PU ROTARY SWITCH POS 3
	PB10 INPUT PU ROTARY SWITCH POS 4
	PB11 INPUT PU ROTARY SWITCH POS 5
	PB1 INPUT PU ROTARY SWITCH POS 6
```

### POSITION SWITCH
```	*PC13 INPUT PD WC MC POSITION SWITCH```
### ```* NOT USED```

## keyboard:
```
  reset   stop         m1      m2
  GoZero start/pause rewind Probe-Z
  Spind  =1/2        =0     Safe-Z
  Home   Step+     MPG mode M3
  not used
```

## default keymap:
```
	RESET
	Stop           Pause/Run     Rewind       ProbeZ
	GotoZ          X/2           Y/2          Go SafeZ
	ZeroX[X=0]     ZeroY[Y=0]    ZeroZ[Z=0]   Go Home
	Jog inc[Step]  Jog/MPG[Mode] Spin On/Off
```

## display
```
01234567890123456789
STATUS: 0000
POS: X    MPG: 9999
S: 9999  F: 9999
O:  999  O:  999
     MC       WC
X - 999.99 - 999.99
Y - 999.99 - 999.99
X - 999.99 - 999.99
```

## my keys
```
RST      Stop       Start/Pause  ...
SafeZ    probeZ     probeLen     ...
X=0      Y=0        Z=0          Home
Step     ...        Spindel      ...
```


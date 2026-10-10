## Components

- U1: NE555P timer IC (astable mode)
- R1: 1 kΩ resistor
- R2: 680 Ω resistor
- R3: 1 kΩ resistor (LED current limiting)
- C1: 1000 µF (1 mF) electrolytic capacitor (timing)
- C2: 10 nF capacitor
- D1: LED
- Power supply: +9 V

## Timing

For an NE555 in astable mode:

- Frequency: f = 1.44 / ((R1 + 2 x R2) x C1)
- On time (HIGH): t_high = 0.693 x (R1 + R2) x C1
- Off time (LOW): t_low = 0.693 x R2 x C1

With R1 = 1 kΩ, R2 = 680 Ω and C1 = 1000 µF:

- Frequency: about 0.61 Hz
- On time: about 1.16 s
- Off time: about 0.47 s

Values are calculated from the formula. Actual timing varies with component tolerances.

# Test Application for Tibbit #52 16bit ADC

ADC characteristics:

- Each channel measures signals from -10V to +10V.
- A measure of the voltage level on one channel is about 140ms.
- Four channels of effective flicker-free resolution that is better than 13 bits.
- Zero offset error is within 0.005% of the input signal's scale (20V, from -10V to +10V).
- Full-scale nonlinearity error is around 1% (after the range correction).Both Tibbits are tested in the same project.

You will need:

- TPP2, TPP2(G2), TPP3, or TPP3(G2) board
- One Tibbit #20 (9 terminal blocks)
- Optionally, one Tibbit #9 or #10 (12V->5V regulator)
- Optionally, one Tibbit #18 (power jack)

*The last two Tibbits is necessary if you are going to power your rig from a 12V power adaptor. Alternatively, you can supply regulated +5V power directly to the TPP.*

The pin configuration is in +/- pairs, meaning, on a Tibbit#20, pin 1 (+) & 2 (2) are paired for channel one, and 3 (+) & 4 (-) are paired for channel two, etc.

The readouts are displayed using sys.debugprint. Therefore, you must run this program in the debug mode.